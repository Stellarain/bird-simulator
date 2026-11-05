# bird-simulator

A small Java lesson on the strategy pattern. A `Duck` does not implement flying or quacking itself: it holds a `FlyBehavior` and a `QuackBehavior` and passes each call to them, so `BasicDuck` and `FancyDuck` differ only in which behaviours they are given. `BirdSimulator` makes one of each and has them fly and quack.

## Build and run

You need a JDK and [Maven](https://maven.apache.org/). `pom.xml` targets Java 8 (`maven.compiler.source` and `maven.compiler.target` are `1.8`), so use JDK 8 or later.

```bash
mvn package
java -jar target/BirdSimulator-1.0-SNAPSHOT.jar
```

It prints:

```
[Flying]
Quack!
[Flying]
Gentlemanly Quack!
```

These steps were last run on 5 November 2026, with Maven 3.9.11 on JDK 17 and on JDK 21.
