# DXP & Open Source

This document outlines the OSS projects in use at view.DO to support the DXP platform.

> [view.DO OSS Policy](OSS-policy.md)

## Runtime Services

The following is a list of OSS-services required by DXP:

* **RabbitMQ**: MPL2 License 2.0\
  <https://github.com/rabbitmq/rabbitmq-server/blob/master/LICENSE>
* **Redis**: BSD-3 Clause\
  <https://github.com/redis/redis/blob/5.0/COPYING>
* **MySQL**: MIT License\
  <https://github.com/mysqljs/mysql/blob/master/License>

Other projects used for operations, but not required:

* **Kubernetes**: Apache License 2.0\
  <https://github.com/kubernetes/kubernetes/blob/master/LICENSE>
  
* **Traefik**: MIT 2.0 License\
  <https://github.com/traefik/traefik/blob/master/LICENSE.md>
* **Kubeless**: MIT 2.0 License\
  <https://github.com/kubeless/kubeless/blob/master/LICENSE>
* **Sealed-Secrets**: MIT 2.0 License\
  <https://github.com/bitnami-labs/sealed-secrets/blob/main/LICENSE>

## Code Packages

The list below are the Nuget.org packages used within DXP. The directory holds the licence info for each OSS component. This list contains the main package, which has a license identical to their sub-components. This list does not include the Microsoft components that are licensed through the .NET runtime. Their MIT license is here: <https://github.com/dotnet/runtime/blob/main/LICENSE.TXT>

Click to view license information.

* 📄 [Auth0.Core](./licenses/Auth0.Core.md)
* 📄 [AutoMapper](./licenses/AutoMapper.md)
* 📄 [CronExpressionDescriptor](./licenses/CronExpressionDescriptor.md)
* 📄 [Dapper](./licenses/Dapper.md)
* 📄 [DotLiquid](./licenses/DotLiquid.md)
* 📄 [EasyNetQ](./licenses/EasyNetQ.md)
* 📄 [FluentMigrator](./licenses/FluentMigrator.md)
* 📄 [Google.Cloud.Storage.V1](./licenses/Google.Cloud.Storage.V1.md)
* 📄 [HtmlAgilityPack](./licenses/HtmlAgilityPack.md)
* 📄 [KubernetesClient](./licenses/KubernetesClient.md)
* 📄 [MailKit](./licenses/MailKit.md)
* 📄 [MimeTypesMap](./licenses/MimeTypesMap.md)
* 📄 [MySqlConnector](./licenses/MySqlConnector.md)
* 📄 [NetEscapades.Configuration.Yaml](./licenses/NetEscapades.Configuration.Yaml.md)
* 📄 [Newtonsoft.Json](./licenses/Newtonsoft.Json.md)
* 📄 [Polly.Extensions.Http](./licenses/Polly.Extensions.Http.md)
* 📄 [Postmark](./licenses/Postmark.md)
* 📄 [Quartz](./licenses/Quartz.md)
* 📄 [RavenDB.Client](./licenses/RavenDB.Client.md)
* 📄 [RestSharp](./licenses/RestSharp.md)
* 📄 [Sendgrid](./licenses/Sendgrid.md)
* 📄 [Seq.Extensions.Logging](./licenses/Seq.Extensions.Logging.md)
* 📄 [Serilog](./licenses/Serilog.md)
* 📄 [StackExchange.Redis](./licenses/StackExchange.Redis.md)
* 📄 [Stateless](./licenses/Stateless.md)
* 📄 [Swashbuckle.AspNetCore](./licenses/Swashbuckle.AspNetCore.md)
* 📄 [Twilio](./licenses/Twilio.md)
* 📄 [UAParser](./licenses/UAParser.md)
* 📄 [dotless.Core](./licenses/dotless.Core.md)
* 📄 [index](./licenses/index.md)
* 📄 [libphonenumber\-csharp](./licenses/libphonenumber-csharp.md)

### Ancillary Testing Components

* 📂 [tests](./licenses/tests)
  * 📄 [AutoFixture](./licenses/tests/AutoFixture.md)
  * 📄 [Ensure.That](./licenses/tests/Ensure.That.md)
  * 📄 [FluentAssertions](./licenses/tests/FluentAssertions.md)
  * 📄 [Moq](./licenses/tests/Moq.md)
  * 📄 [RavenDB.Embedded](./licenses/tests/RavenDB.Embedded.md)

> For license URLs, component version numbers and other details, see [the full audit output here](./licenses/.audit-output.yam)
