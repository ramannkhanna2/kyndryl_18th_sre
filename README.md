# SRE related terms glossary :

```

SRE (Site Reliability Engineering) – discipline of applying software engineering principles to operations to ensure reliability, scalability, and efficiency.

Reliability – ability of a system to consistently meet its expected function (uptime, availability).

Availability – percentage of time a service is up and accessible (e.g., “four nines” = 99.99%).

Latency – time taken to respond to a request.

Throughput – number of requests a system can handle per unit time.

Error Rate – fraction of requests that fail.

Capacity Planning – forecasting resources (CPU, memory, storage) to handle load.

Load Balancing – distributing traffic across servers to improve performance and resilience.

Failover – automatic switch to backup systems when the primary fails.

SLI (Service Level Indicator) – measurable metric showing service performance (e.g., request success rate).

SLO (Service Level Objective) – target threshold for an SLI (e.g., 99.9% uptime).

SLA (Service Level Agreement) – contractual promise to customers, often with penalties if violated.

Error Budget – allowed amount of failure (1 - SLO); balance between innovation speed and reliability.

Monitoring – collecting metrics, logs, and traces to check system health.

Observability – ability to infer internal system state from external outputs (metrics, logs, traces).

Metrics – numerical measurements (CPU usage, request rate).

Logs – time-stamped event records (errors, state changes).

Traces – record of a request’s journey across services (useful in microservices).

Dashboards – visual representation of metrics.

Alerts – notifications triggered when metrics cross thresholds.

Blackbox Monitoring – monitoring from the outside (simulating user perspective).

Whitebox Monitoring – monitoring internal metrics of a system.

Incident – unplanned disruption or degradation of service.

Postmortem – documented analysis of an incident, focusing on learning, not blame.

On-Call – rotation of engineers responsible for handling incidents.

Runbook – documented procedure for diagnosing and fixing known issues.

Toil – repetitive manual operational work that doesn’t scale.

Blameless Culture – addressing failures without personal blame; encourages transparency.

Chaos Engineering – deliberately injecting failures to test system resilience.

Load Testing – testing system under expected traffic conditions.

Stress Testing – testing system under extreme traffic beyond expectations.

Canary Release – releasing new code to a small set of users before full rollout.

Blue-Green Deployment – two environments (blue=live, green=staging) for safe switchovers.

Rolling Deployment – gradually updating services with zero downtime.

Circuit Breaker – design pattern that stops calls to failing services to prevent cascading failures.

Retry with Backoff – retrying failed requests but with increasing delays.

Infrastructure as Code (IaC) – managing infrastructure via code (Terraform, Ansible).

Configuration Management – tools to define and maintain server/app states (Puppet, Chef).

Orchestration – automated management of containers and services (Kubernetes).

Service Mesh – layer managing service-to-service communication with observability and resilience (Istio, Linkerd).

Secrets Management – secure handling of passwords, tokens, certs (Vault).

Resource Utilization – how efficiently CPU, memory, etc., are used.

Autoscaling – automatically adjusting resources based on load.

Cost Optimization – monitoring and reducing unnecessary cloud expenses (Kubecost, FinOps).

```









#SRE related popular tools :


```
Prometheus – metrics collection and monitoring.

Grafana – visualization and dashboards.

Alertmanager – alert routing/management (pairs with Prometheus).

ELK Stack (Elasticsearch, Logstash, Kibana) – log aggregation, search, and visualization.

Fluentd / Fluent Bit – log forwarding and processing.

Jaeger – distributed tracing.

Zipkin – distributed tracing (lighter alternative to Jaeger).

OpenTelemetry – standardized instrumentation for metrics, traces, and logs.

PagerDuty – incident management and on-call alerting.

Opsgenie – alerting and on-call scheduling.

VictorOps (Splunk On-Call) – incident management and alerting.

ServiceNow – ITSM and incident/change management.

Kubernetes – container orchestration and self-healing infrastructure.

Istio / Linkerd – service mesh for traffic control, resilience, and observability.

Envoy – high-performance proxy for service mesh and edge routing.

Consul – service discovery and configuration management.

Terraform – infrastructure as code and provisioning.

Ansible – configuration management and automation.

Puppet / Chef – infrastructure automation and config management.

SaltStack – event-driven automation and orchestration.

Vault – secret management and encryption.

Sensu – monitoring and observability pipeline.

Nagios – traditional monitoring and alerting.

Zabbix – monitoring of infrastructure, networks, and servers.

Datadog – SaaS monitoring, metrics, traces, and logs.

New Relic – application performance monitoring and observability.

AppDynamics – APM and business transaction monitoring.

Dynatrace – AI-driven full-stack monitoring.

Splunk – log analysis and security/observability.

Honeycomb – observability with focus on high-cardinality event data.

Thanos – scalable, long-term storage for Prometheus metrics.

Cortex / Mimir – horizontally scalable Prometheus backend.

Kiali – observability dashboard for service meshes.

Chaos Monkey (and Chaos Toolkit) – chaos engineering for resilience testing.

Gremlin – SaaS chaos engineering platform.

Statuspage / Better Uptime – incident communication and status dashboards.

Checkly / Pingdom – synthetic monitoring of APIs and websites.

Blackbox Exporter – probing/endpoint monitoring for Prometheus.

Node Exporter – system metrics exporter for Prometheus.

cAdvisor – container resource usage and performance metrics.

KEDA – event-driven autoscaling for Kubernetes.

Kubecost – cost monitoring and optimization in Kubernetes.

Sentry – error tracking and application monitoring.

Bugsnag – error monitoring and stability management.

Rollbar – real-time error monitoring.

```

This is the "big league" toolbox — some teams use a slice, some stitch together many.





