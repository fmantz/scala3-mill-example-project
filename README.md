# Example mill project that compiles using Scala 3

## Usage

This is a normal mill project. You can compile code with `mill examples.compile` and run it
with `mill examples.run`, `mill -i examples.console` will start a Scala 3 REPL.

In addition, you can also create a running jar file with the mill4scala plugin, that
is reduced in its size. Either run `mill examples.assembly` or `mill examples.jar`.
Since there are no test cases or dependencies the result will be basically the same.

```bash
./mill examples.assembly

java -jar ./out/examples/assembly.dest/out.jar
```

### IDE support

It's recommended to either use [Metals](https://scalameta.org/metals/) with the
editor of your choice or [the Scala Plugin for
IntelliJ](https://blog.jetbrains.com/scala/).

## Using Scala 3 in an existing project

### build.sc

```scala
def scalaVersion = "3.8.4"
```

### Getting your project to compile with Scala 3

For help with porting an existing Scala 2 project to Scala 3, see the
[Scala 3 migration guide](https://docs.scala-lang.org/scala3/guides/migration/compatibility-intro.html).

## Need help?

https://www.scala-lang.org/community/ has links.
