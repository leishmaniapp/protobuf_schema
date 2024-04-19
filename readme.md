# Protobuf shared schema definition between services in the Leishmaniapp project

This repository is intended to be used as a [Git Submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) in other Leishmaniapp related projects in order to maintain a common schema between services

## ✉️  Headers
The following headers might be required by one or more gRPC services and must always be sent by the client.

| Header | Content | Purpose |
| ------ | ------- | ------- |
| Authorization | Bearer _<jwt token>_ | Validate authentication |
| From | Specialist email (unique identification) | Identify resources owned by the user |
