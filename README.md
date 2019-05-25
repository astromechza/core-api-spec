# core-api-spec

OpenAPIv3 core specification of the API used between various clients (such as Typescript, Kotlin, Golang) and a server (such as a directory server).

- [View the spec in the swagger editor](https://editor.swagger.io/?import=https://raw.githubusercontent.com/aurelian-one/core-api-spec/master/spec/src/spec.yaml)

## Why separate the API spec?

This is done to separate the interface (the api) from the implementation (the api server itself). This helps to keep clients compatible with servers and prevent servers from making incompatible API changes.

For an example of generating a client see the [example-java-client](./example-java-client/pom.xml) which does the following as part of its build process:

1. Unpack swagger schema from core-api-schema dependency
2. Use openapi generator to generate java client code
3. Package as `example-java-client` module

## How to trigger a release from develop to master

Cut a branch off develop named `release-<whatever>` and push it, CircleCI should use this to trigger the release process if your user has the correct permissions.
