# 1. Cloud


"The cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world.


| # | Title | Link |
| -- | -- | -- |
| 1 | What Is the Cloud? | [Click Here](https://www.cloudflare.com/learning/cloud/what-is-the-cloud/) |
| 2 | What Is Multicloud? | [Click Here](https://www.cloudflare.com/learning/cloud/what-is-multicloud/) |
| 3 | What Is Hybrid Cloud? | |
| 4 | What Is a Cloud Firewall? | [Click Here](https://www.cloudflare.com/learning/cloud/what-is-a-cloud-firewall/) |
| 5 | What Is SaaS? | [Click Here](https://www.cloudflare.com/learning/cloud/what-is-saas/) | 
| 6 | What Is IaaS (Infrastructure-as-a-Service)? |
| 7 | What Is Cloud Migration? | [Click Here](https://www.cloudflare.com/learning/cloud/what-is-cloud-migration/) |
| 8 | What Is a Public Cloud? | |
| 9 | What Is a Private Cloud? | |
| 10 | What Is Multicloud Management? | |
| 11 | What Is a Virtual Machine? |
| 12 | What Is a Next-Generation Firewall (NGFW)? | |
| 13 | What Is Cloud Storage? | 
| 14 | What Is Digital Transformation? | 
| 15 | What Is Multitenancy? | 
| 16 | What Is Vendor Lock-In? | 
| 17 | What Is a Virtual Private Cloud (VPC)? |
| 18 | How Does Cloud Security Work? | |
| 19 | How Does Hybrid Cloud Architecture Work? | |
| 20 | Multicloud vs. Hybrid Cloud: What's the Difference? |

## 1.1 Cloud Design Patterns

### 1.1.1 Data Management

| # | Title | Summmary |
| -- | :-- | :-- |
| 1 | [Cache-Aside](https://docs.microsoft.com/en-us/azure/architecture/patterns/cache-aside) | Load data on demand into a cache from a data store |
| 2 | [CQRS](https://docs.microsoft.com/en-us/azure/architecture/patterns/cqrs) | Segregate operations that read data from operations that update data by using separate interfaces. |
| 3 | [Event Sourcing](https://docs.microsoft.com/en-us/azure/architecture/patterns/event-sourcing) | Use an append-only store to record the full series of events that describe actions taken on data in a domain. |
| 4 | [Index Table](https://docs.microsoft.com/en-us/azure/architecture/patterns/index-table) | Create indexes over the fields in data stores that are frequently referenced by queries. |
| 5 | [Materialized View](https://docs.microsoft.com/en-us/azure/architecture/patterns/materialized-view) | Generate prepopulated views over the data in one or more data stores when the data isn't ideally formatted for required query operations. |
| 6 | [Sharding](https://docs.microsoft.com/en-us/azure/architecture/patterns/sharding) | Divide a data store into a set of horizontal partitions or shards. |
| 7 | [Static Content Hosting](https://docs.microsoft.com/en-us/azure/architecture/patterns/static-content-hosting) | Deploy static content to a cloud-based storage service that can deliver them directly to the client. |
| 8 | [Valet Key](https://docs.microsoft.com/en-us/azure/architecture/patterns/valet-key) | Use a token or key that provides clients with restricted direct access to a specific resource or service. |

### 1.1.2 Design and Implementation

| # | Title | Summmary |
| -- | :-- | :-- |
| 1 | [Ambassador](https://docs.microsoft.com/en-us/azure/architecture/patterns/ambassador) | Create helper services that send network requests on behalf of a consumer service or application. |
| 2 | [Anti-Corruption Layer](https://docs.microsoft.com/en-us/azure/architecture/patterns/anti-corruption-layer) | Implement a façade or adapter layer between a modern application and a legacy system. |
| 3 | [Backends for Frontends](https://docs.microsoft.com/en-us/azure/architecture/patterns/backends-for-frontends) | Create separate backend services to be consumed by specific frontend applications or interfaces. |
| 4 | [CQRS](https://docs.microsoft.com/en-us/azure/architecture/patterns/cqrs) | Segregate operations that read data from operations that update data by using separate interfaces. |
| 5 | [Compute Resource Consolidation](https://docs.microsoft.com/en-us/azure/architecture/patterns/compute-resource-consolidation) | Consolidate multiple tasks or operations into a single computational unit |
| 6 | [External Configuration Store](https://docs.microsoft.com/en-us/azure/architecture/patterns/external-configuration-store) | Move configuration information out of the application deployment package to a centralized location. |
| 7 | [Gateway Aggregation](https://docs.microsoft.com/en-us/azure/architecture/patterns/gateway-aggregation) | Use a gateway to aggregate multiple individual requests into a single request. |
| 8 | [Gateway Offloading](https://docs.microsoft.com/en-us/azure/architecture/patterns/gateway-offloading) | Offload shared or specialized service functionality to a gateway proxy. |
| 9 | [Gateway Routing](https://docs.microsoft.com/en-us/azure/architecture/patterns/gateway-routing) |  Route requests to multiple services using a single endpoint. |
| 10 | [Leader Election](https://docs.microsoft.com/en-us/azure/architecture/patterns/leader-election) | Coordinate the actions performed by a collection of collaborating task instances in a distributed application by electing one instance as the leader that assumes responsibility for managing the other instances. |
| 11 | [Pipes and Filters](https://docs.microsoft.com/en-us/azure/architecture/patterns/pipes-and-filters) | Break down a task that performs complex processing into a series of separate elements that can be reused. |
| 12  | [Sidecar](https://docs.microsoft.com/en-us/azure/architecture/patterns/sidecar) | Deploy components of an application into a separate process or container to provide isolation and encapsulation. |
| 13  | [Static Content Hosting](https://docs.microsoft.com/en-us/azure/architecture/patterns/static-content-hosting) | Deploy static content to a cloud-based storage service that can deliver them directly to the client. |
| 14  | [Strangler Fig](https://docs.microsoft.com/en-us/azure/architecture/patterns/strangler-fig) | Incrementally migrate a legacy system by gradually replacing specific pieces of functionality with new applications and services. |

### 1.1.3 Messaging

| # | Title | Summmary |
| -- | :-- | :-- |
| 1 | [Asynchronous Request-Reply](https://docs.microsoft.com/en-us/azure/architecture/patterns/async-request-reply) | Decouple backend processing from a frontend host, where backend processing needs to be asynchronous, but the frontend still needs a clear response. |
| 2 | [Claim Check](https://docs.microsoft.com/en-us/azure/architecture/patterns/claim-check) | Split a large message into a claim check and a payload to avoid overwhelming a message bus. |
| 3 | [Choreography](https://docs.microsoft.com/en-us/azure/architecture/patterns/choreography) | Have each component of the system participate in the decision-making process about the workflow of a business transaction, instead of relying on a central point of control. |
| 4 | [Competing Consumers](https://docs.microsoft.com/en-us/azure/architecture/patterns/competing-consumers) | Enable multiple concurrent consumers to process messages received on the same messaging channel. |
| 5 | [Pipes and Filters](https://docs.microsoft.com/en-us/azure/architecture/patterns/pipes-and-filters) | Break down a task that performs complex processing into a series of separate elements that can be reused. |
| 6 | [Priority Queue](https://docs.microsoft.com/en-us/azure/architecture/patterns/priority-queue) | Prioritize requests sent to services so that requests with a higher priority are received and processed more quickly than those with a lower priority. |
| 7 | [Publisher-Subscriber](https://docs.microsoft.com/en-us/azure/architecture/patterns/publisher-subscriber) | Enable an application to announce events to multiple interested consumers asynchronously, without coupling the senders to the receivers. |
| 8 | [Queue-Based Load Leveling](https://docs.microsoft.com/en-us/azure/architecture/patterns/queue-based-load-leveling) | Use a queue that acts as a buffer between a task and a service that it invokes in order to smooth intermittent heavy loads. |
| 9 | [Scheduler Agent Supervisor](https://docs.microsoft.com/en-us/azure/architecture/patterns/scheduler-agent-supervisor) | Coordinate a set of actions across a distributed set of services and other remote resources. |
| 10 | [Sequential Convoy](https://docs.microsoft.com/en-us/azure/architecture/patterns/sequential-convoy) | Process a set of related messages in a defined order, without blocking processing of other groups of messages. |

# 2. DDoS


In a distributed denial-of-service (DDoS) attack, a network of computers work in tandem to overflow an access point and prevent legitimate users from accessing a service.


| # | Title | Link |
| -- | :-- | -- |
| 1 | What is a DDoS Attack? |
| 4 | What is a DDoS Botnet? |
| 5 | What is DDoS Mitigation? |
| 6 | What is Blackhole Routing? |
| 7 | What is a Denial-of-Service (DoS) Attack? |
| 8 | What is IP Spoofing? |
| 9 | What Is The OSI Model? |
| 10 | What is TCP/IP? |
| 11 | What is the Internet Control Message Protocol (ICMP)? |
| 12 | What is Layer 7? - How Layer 7 of the Internet Works |
| 13 | What is a WAF? - Web Application Firewall explained |
| 14 | What is Malware? |
| 15 | What is UDP? |
| 16 | Famous DDoS attacks - The largest DDoS attacks of all time |

## 2.1 Common DDoS Attacks

| #  | Title | Link |
| -- | -- | -- |
| 1 | Memcached DDoS Attack |
| 2 | NTP Amplification DDoS Attack |
| 3 | DNS Amplification Attack |
| 4 | SSDP DDoS Attack |
| 5 | What is a DNS Flood? - DNS Flood DDoS Attack |
| 6 | HTTP Flood Attack |
| 7 | SYN Flood Attack |
| 8 | UDP Flood Attack |
| 9 | Ping (ICMP) Flood DDoS Attack |
| 10 | What is a low and slow attack? |
| 11 | Application Layer DDoS Attack |
| 12 | How Do Layer 3 DDoS Attacks Work? - L3 DDoS |
| 13 | Cryptocurrency DDoS Attacks |
| 14 | What Is an ACK Flood DDoS Attack? - Types of DDoS Attacks |
| 15 | What Is a QUIC Flood DDoS Attack? - QUIC and UDP Floods |
| 16 | What is a ransom DDoS attack?  |
| 17 | Smurf DDoS Attack |
| 18 | Ping of Death DDoS attack | 

## 2.2 DDoS Attack Tools

| #  | Title | Link |
| -- | -- | -- |
| 1 | How to DDoS - DoS and DDoS Attack tools |
| 2 | What Is The Low Orbit Ion Cannon (LOIC)? |
| 3 | What Is The High Orbit Ion Cannon (HOIF)? |
| 4 | R U Dead Yet? (R.U.D.Y.) Attack |
| 5 | Slowloris DDoS Attack |
| 6 | What is a DDoS Booter/IP Stresser? - DDoS Attack Tools |

# 3. Microservice


Microservices - also known as the microservice architecture - is an architectural style that structures an application as a collection of services that are

-   Highly maintainable and testable
-   Loosely coupled
-   Independently deployable
-   Organized around business capabilities
-   Owned by a small team

The microservice architecture enables the rapid, frequent and reliable delivery of large, complex applications. It also enables an organization to evolve its technology stack.


## 3.1 Patterns

[How to apply the patterns](https://microservices.io/articles/applying.html)

### 3.1.1 Application Architecture Patterns 

| # | Title | Summary |
| -- | :-- | :-- |
| 1 | [Monolithic architecture](https://microservices.io/patterns/monolithic.html) |emphasized text
| 2 | [Microservice architecture](https://microservices.io/patterns/microservices.html) |

### 3.1.2 Decomposition

| # | Title |
| -- | :-- |
| 1 | [Decompose by business capability](https://microservices.io/patterns/decomposition/decompose-by-business-capability.html) |
| 2 | [Decompose by subdomain](https://microservices.io/patterns/decomposition/decompose-by-subdomain.html) |
| 3 | [Self-contained Service](https://microservices.io/patterns/decomposition/self-contained-service.html) |
| 4 | [Service per team](https://microservices.io/patterns/decomposition/service-per-team.html) |

### 3.1.3 Refactoring to Microservices

| # | Title |
| -- | :-- |
| 1 | [Strangler Application](https://microservices.io/patterns/refactoring/strangler-application.html) |
| 2 | [Anti-corruption layer](https://microservices.io/patterns/refactoring/anti-corruption-layer.html) |

### 3.1.4 Data Management

| # | Title |
| -- | :-- |
| 1 | [Database per Service](https://microservices.io/patterns/data/database-per-service.html) |
| 2 | [Shared database](https://microservices.io/patterns/data/shared-database.html) |
| 3 | [Saga](https://microservices.io/patterns/data/saga.html) |
| 4 | [API Composition](https://microservices.io/patterns/data/api-composition.html) |
| 5 | [CQRS](https://microservices.io/patterns/data/cqrs.html) |
| 6 | [Domain event](https://microservices.io/patterns/data/domain-event.html) |
| 7 | [Event sourcing](https://microservices.io/patterns/data/event-sourcing.html) |

### 3.1.5 Transactional Messaging

| # | Title |
| -- | :-- |
| 1 | [Transactional outbox](https://microservices.io/patterns/data/transactional-outbox.html) |
| 2 | [Transaction log tailing](https://microservices.io/patterns/data/transaction-log-tailing.html) |
| 3 | [Polling publisher](https://microservices.io/patterns/data/polling-publisher.html) |

### 3.1.6 Testing

| # | Title |
| -- | :-- |
| 1 | [Service Component Test](https://microservices.io/patterns/testing/service-component-test.html) |
| 2 | [Consumer-driven contract test](https://microservices.io/patterns/testing/service-integration-contract-test.html) |
| 3 | [Consumer-side contract test](https://microservices.io/patterns/testing/consumer-side-contract-test.html) |

### 3.1.7 Deployment Patterns

| # | Title |
| -- | :-- |
| 1 | [Multiple service instances per host](https://microservices.io/patterns/deployment/multiple-services-per-host.html) |
| 2 | [Service instance per host](https://microservices.io/patterns/deployment/single-service-per-host.html) |
| 3 | [Service instance per VM](https://microservices.io/patterns/deployment/service-per-vm.html) |
| 4 | [Service instance per Container](https://microservices.io/patterns/deployment/service-per-container.html) |
| 5 | [Serverless deployment](https://microservices.io/patterns/deployment/serverless-deployment.html) |
| 6 | [Service deployment platform](https://microservices.io/patterns/deployment/service-deployment-platform.html) |

### 3.1.8 Cross cutting concerns

| # | Title |
| -- | :-- |
| 1 | [Microservice chassis](https://microservices.io/patterns/microservice-chassis.html) |
| 2 | [Service Template](https://microservices.io/patterns/service-template.html) |
| 3 | [Externalized configuration](https://microservices.io/patterns/externalized-configuration.html) |

### 3.1.9 Communication Style

| # | Title |
| -- | :-- |
| 1 | [Remote Procedure Invocation](https://microservices.io/patterns/communication-style/rpi.html) |
| 2 | [Messaging](https://microservices.io/patterns/communication-style/messaging.html) |
| 3 | [Domain-specific protocol](https://microservices.io/patterns/communication-style/domain-specific.html) |
| 4 | [Idempotent Consumer](https://microservices.io/patterns/communication-style/idempotent-consumer.html) |

### 3.1.10 External API

| # | Title |
| -- | :-- |
| 1 | [API gateway](https://microservices.io/patterns/apigateway.html) |
| 2 | [Backend for front-end](https://microservices.io/patterns/apigateway.html) |

### 3.1.11 Service Discovery

| # | Title |
| -- | :-- |
| 1 | [Client-side discovery](https://microservices.io/patterns/client-side-discovery.html) |
| 2 | [Server-side discovery](https://microservices.io/patterns/server-side-discovery.html) |
| 3 | [Service registry](https://microservices.io/patterns/service-registry.html) |
| 4 | [Self registration](https://microservices.io/patterns/self-registration.html) |
| 5 | [3rd party registration](https://microservices.io/patterns/3rd-party-registration.html) |

### 3.1.12 Reliability

| # | Title |
| -- | :-- |
| 1 | [Circuit Breaker](https://microservices.io/patterns/reliability/circuit-breaker.html) |

### 3.1.13 Security

| # | Title |
| -- | :-- |
| 1 | [Access Token](https://microservices.io/patterns/security/access-token.html) |

### 3.1.14 Observability

| # | Title |
| -- | :-- |
| 1 | [Log aggregation](https://microservices.io/patterns/observability/application-logging.html) |
| 2 | [Application metrics](https://microservices.io/patterns/observability/application-metrics.html) |
| 3 | [Audit logging](https://microservices.io/patterns/observability/audit-logging.html) |
| 4 | [Distributed tracing](https://microservices.io/patterns/observability/distributed-tracing.html) |
| 5 | [Exception tracking](https://microservices.io/patterns/observability/exception-tracking.html) |
| 6 | [Health check API](https://microservices.io/patterns/observability/health-check-api.html) |
| 7 | [Log deployments and changes](https://microservices.io/patterns/observability/log-deployments-and-changes.html) |

### 3.1.15 UI Patterns

| # | Title |
| -- | :-- |
| 1 | [Server-side page fragment composition](https://microservices.io/patterns/ui/server-side-page-fragment-composition.html) |
| 2 | [Client-side UI composition](https://microservices.io/patterns/ui/client-side-ui-composition.html) |
