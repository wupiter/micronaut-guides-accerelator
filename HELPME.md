## Micronaut 3.1.0 Documentation

- [User Guide](https://docs.micronaut.io/3.1.0/guide/index.html)
- [API Reference](https://docs.micronaut.io/3.1.0/api/index.html)
- [Configuration Reference](https://docs.micronaut.io/3.1.0/guide/configurationreference.html)
- [Micronaut Guides](https://guides.micronaut.io/index.html)
---

## Feature http-client documentation

- [Micronaut HTTP Client documentation](https://docs.micronaut.io/latest/guide/index.html#httpClient)

## Run application
Run below command in terminal:
```
./gradlew run
```

Once application is started, you can test it using below command in terminal:
```
time curl http://localhost:8080/conferences/random
```

## Build native image using GraalVM
GraalVM is a polyglot virtual machine that can generate a native image of our Micronaut application.

Compiling native images ahead of time with GraalVM improves startup time and reduces the memory footprint of JVM-based applications.

1. Follow instructions to install GraalVM [here](https://www.graalvm.org/docs/getting-started/#install-graalvm).
2. Install `native-image` component using this command: `gu install native-image`
3. Generate native image using this command: `./gradlew nativeImage`, or
4. Generate docker container that runs our app's native image: `./gradlew dockerBuildNative`

## Guides
- [First Micronaut GraalVM Application](https://guides.micronaut.io/latest/micronaut-creating-first-graal-app-gradle-java.html)
- [Adding Git Commit Info](https://guides.micronaut.io/latest/adding-commit-info-gradle-java.html)
