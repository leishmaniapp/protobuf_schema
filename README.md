# Protobuf shared schema definition between services in the Leishmaniapp project

This repository is intended to be used as a [Git Submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) in other Leishmaniapp related projects in order to maintain a common schema between services

## 📡 gRPC
The _specialist_ field in some of the messages must be validated by the authentication provider or gateway for coherence with the [_Authorization Header_](#✉️-headers)

### ✉️  Headers
The following headers might be required by one or more gRPC services and must always be sent by the client.

| Header | Content | Purpose |
| ------ | ------- | ------- |
| Authorization | Bearer _\<jwt token>_ | Validate authentication via JWT tokens |