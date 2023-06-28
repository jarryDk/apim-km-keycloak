# Integrate Keycloak as a Third Party Key Manager for WSO2 API Manager

This Keycloak key manager implementation allows you to integrate the WSO2 API Store with an external Keycloak Identity and Access Management server (IAM) by using the Keycloak OAuth to manage the OAuth clients and tokens required by WSO2 API Manager. We have a sample client implementation that consumes the admin REST APIs exposed by keycloak.

## Getting Started

To get started, go to [Integrate WSO2 API Store with an external IAM using the Keycloak Open Source IAM](docs/config.md).

## Build

Use the following command to build this implementation

```bash
mvn clean install
```

## Updating the jar file

The jar file is location around this location `//wso2am-4.2.0/repository/components/plugins/keycloak.key.manager_2.1.0.jar` and
if the jar file  have changed size you will have to update the file `//wso2am-4.2.0/repository/components/artifacts.xml` too.

In `//wso2am-4.2.0/repository/components/artifacts.xml` search for `keycloak.key.manager` and update the value for `download.size`.

## How You Can Contribute

To contribute to the Keycloak key manager development, fork the github repository and send your pull requests to [https://github.com/wso2-extensions/apim-keymanager-keycloak](https://github.com/wso2-extensions/apim-keymanager-keycloak)
