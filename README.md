Sample implementation of the **Clean Architecture Principles with .NET Core**. Use cases as central organizing structure, decoupled from frameworks and technology details. Built by small components that are developed and tested in isolation.


Manga is a Virtual Wallet Solution in which the customer register an account then manage the balance by `Deposit`, `Withdraw` and `Transfer` operations.

We also support the React client

## Key echnologies
- .NET 5
- React
- Redux
- Docker
- Swagger
- Identity Server
- nginx

## Build & Run

To startup the whole solution, execute the following command:

Windows:

```ps1
PS cd .docker && ./setup.ps1
```

MacOS:

```sh
$ cd .docker && ./setup.sh
```

Then the following containers should be running on `docker ps`:

| Application 	      | URL                                                                           |
|-------------------- | ----------------------------------------------------------------------------- |
| NGINX 	          | https://wallet.local:8081                                                     |
| Wallet SPA 	      | https://wallet.local:8081                                                     |
| Accounts API 	      | https://wallet.local:8081/accounts-api                                        |
| Identity Server 	  | https://wallet.local:8081/identity-server	                                  |
| SQL Server 	      | Server=localhost;User Id=sa;Password=<YourStrong!Passw0rd>;Database=Accounts; |

Browse to [https://wallet.local:8081](https://wallet.local:8081) then click on Log In. If asked trust the [self-signed certificate](https://stackoverflow.com/questions/21397809/create-a-trusted-self-signed-ssl-cert-for-localhost-for-use-with-express-node).

## Motivation

> Learn how to design modular applications.
>
> Explore the .NET Core features.

### Learn how to design modular applications

Learning how to design modular applications will help you become a better engineer. Designing modular applications is the holy grail of software architecture, it is hard to find engineers experienced on designing applications which allows adding new features in a steady speed.

### Explore the .NET Core features

.NET Core brings a sweet development environment, an extensible and cross-platform framework. We will explore the benefits of it in the infrastructure layer and we will reduce its importance in the application and domain layers. The same rule is applied for modern C# language syntax.
