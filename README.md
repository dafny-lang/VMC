# VMC: a Library for Verified Monte Carlo Algorithms

The `DafnyVMC` module introduces utils for probabilistic reasoning in Dafny. At the moment, the API is intentionally limited in scope, and only supports compilation to Java. For the future, we plan to extend both the functionality and the range of supported languages.

# Dafny Examples

To run the examples in the `docs/dafny` directory, use the following commands:

```bash
# Dafny Examples
$ dafny build docs/dafny/ExamplesRandom.dfy --target:java src/interop/java/Random.java dfyconfig.toml --no-verify
$ java -jar docs/dafny/ExamplesRandom.jar
```

# Java Examples

To run the examples in the `docs/java` directory, use the following command:

```bash
# Java Examples
$ bash scripts/build.sh 
$ bash build/java/run.sh  
```

# Testing

To run the statistical tests in the `tests` directory, use the following commands:

```bash
# Dafny Tests
$ dafny test --target:java src/interop/java/Random.java tests/TestsRandom.dfy tests/Tests.dfy dfyconfig.toml --no-verify
```



