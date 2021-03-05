# view.DO DXP Platform

This repository holds the source code for the seven domains that make up the DXP platform, including web-applications, APIs, a scheduler and message processors.

This file is an overview of the repository and solution. For more detailed information, see:

* [Architectural Overview](https://docs.google.com/presentation/d/10xuJ3HSV4haCYwY_Ab5V1Catc83gvhNHT22Sl5e5C_w/edit?usp=sharing)
* [Run Docs](./README-RUN.md)
* [Development Docs](./README-DEVELOP.md)
* [Deployment Docs](./README-DEPLOY.md)
* [Secret Management Docs](./README-DEPLOY-SECRETS.md)
* [Package Licenses](./src/.licenses)
* [API Usage Docs](https://api.view.do/index.html)

## Service Dependencies

The view.DO DXP platform depends on these services to run.

* **Auth0** authentication as a service for API JWTs
* **Kubernetes** workload orchestration
* **RabbitMQ** cross-application messaging
* **RavenDB** document store (materialized views)
* **Redis** caching layer, global-locks and batch-processing
* **MySQL** data-store for reporting and system message error-handling
* **SEQ** centralized logging and aggregation
* **Traefik** reverse proxies and certificate management
* **Kubeless** hosted functions used as actions within a story's workflow-configuration
* **Sealed-Secrets** for storing encrypted secrets in Git for dev-ops style deployments

## Code Organization

The applications and services that make up the platform are partitioned into domains based on their role within the system. Each domain has a set of applications found in this repository.

### Common

These are libraries used by more than one domain.

Source Root: ./src/common

### Administration

This is the management around the primary business models meant to describe logic in a common vocabulary with a focus on DDD-style nomenclature.

Docs: <https://api.view.do/v4/admin/docs/index.html>

Primary Models:

* Attachment
* Batch
* Experience
* Organization
* Story
* Story Schema
* User

#### Admin Components

Source Root: ./src/admin

* Admin API
* Admin Migrations
* Admin Processor

#### Admin Services

* Raven DB: dxp

### Analytics

This domain is focused on the collection and reporting on data as it changes over time. This system is eventually consistent and should not be used for 'real-time' accuracy.

Docs: <https://api.view.do/v4/analytics/docs/index.html>

#### Analytics Components

Source Root: ./src/analytics

* Analytics API
* Analytics Migrations
* Analytics Processor

#### Analytics Services

* MySQL DB: dxp-analytics

### Authentication & Authorization

This domain is focused user-identity and managing the permissions associated with users of the APIs.

Docs: <https://api.view.do/v4/auth/docs/index.html>

#### Authentication Components

Source Root: ./src/auth

* Authentication API

#### Auth Services

* Auth0 namespace-specific instance-configs: .auth0/

### Experiences

This domain is focused on rendering one web-application configured precisely for one person as well as the collection of events and data-mutations occurred during the end-user's journey through the application.

Docs: <https://xapi.view.do/v4/docs/index.html>

#### Experiences Components

Source Root: ./src/experiences

* Experiences API
* Experiences Processor

#### Experiences Services

* Raven DB: dxp
* Redis DB: namespace specific ID

### Services (External)

This domain is focused on third-party integrations, usually an action that is fired based on a story's configured workflow. Actions that are scheduled for later execution are also managed through this domain.

Docs: <https://api.view.do/v4/services/docs/index.html>

#### Services Components

Source Root: ./src/services

* Services API
* Services Contracts
* Services Migrations
* Services Processor

#### Services

* MySQL DB: dxp-services
* Postmark
* SendGrid
* SparkPost
* Twilio
* Webhooks

### Systems

This domain is focused on the overall deployment, scheduled jobs and message management. It's a self-monitoring system with automatic errored-message retries, failed-message management and service-subscription management.

Docs: <https://api.view.do/v4/systems/docs/index.html>

#### Systems Components

Source Root: ./src/systems

* Systems API
* Systems Migrations
* Systems Scheduler

#### Systems Services

* MySQL DB: dxp-systems

### URLs

This domain is focused on URL shortening, customization as well as Personalized URLs (or PUrls). This system is used to create easy-to-transcribe short-urls for the millions of unique experience-sites distributed through the platform.

Docs: <https://api.view.do/v4/urls/docs/index.html>

#### URLs Components

Source Root: ./src/urls

* URLs API
* URLs Contracts
* URLs Redirect App
* URLs Migrations
* URLs Processor

#### Urls Services

* MySQL DB: dxp-urls
* Redis DB: namespace specific ID
