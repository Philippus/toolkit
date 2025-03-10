# The Scala Toolkit
The batteries-included Scala. Read about the Scala Toolkit in [scala-lang tutorials](https://docs.scala-lang.org/toolkit/introduction.html).

## Using the Scala Toolkit

You can already use it from [Scala CLI](https://scala-cli.virtuslab.org/):
```scala
//> using toolkit latest
```

Or by including the latest Toolkit artifact in your build file: `org.scala-lang::toolkit:0.2.0`

## Dependencies changelog
In the `changelog` directory you can find a list of changes in the dependencies of the Scala Toolkit, including transitive ones.

### Generate or update changelog
To generate or update the changelog, run the following command:
```shell
scala-cli checks -- --module-name toolkit --file Toolkit.scala --skip js --overwrite
scala-cli checks -- --module-name toolkit --file Toolkit.js.scala --skip jvm --skip native --overwrite
scala-cli checks -- --module-name toolkit-test --file ToolkitTest.scala --overwrite --module-dep toolkit
```
