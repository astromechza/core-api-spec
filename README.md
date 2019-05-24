# core-api-spec

OpenAPIv3 core specification of the API used between various clients (such as Typescript, Kotlin, Golang) and a server (such as a directory server).

- [View the spec in the swagger editor](https://editor.swagger.io/?import=https://raw.githubusercontent.com/aurelian-one/core-api-spec/master/spec/src/spec.yaml)

## Why separate the API spec?

This is done to separate the interface (the api) from the implementation (the api server itself). This helps to keep clients compatible with servers and prevent servers from making incompatible API changes.

## Todo and task tracking

https://github.com/orgs/aurelian-one/projects/1?card_filter_query=repo%3Aaurelian-one%2Fcore-api-spec
