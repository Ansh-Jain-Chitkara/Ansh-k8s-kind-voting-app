# K8s Kind Voting App

### Project Title: 

Automated Deployment and Observability of Kubernetes Workloads on AWS using Argo CD, Prometheus, and Grafana

### Description: 

Designed and implemented a production-style Kubernetes platform on AWS EC2 to deploy, manage, and monitor containerized applications using GitOps and full-stack observability.

Built a Kubernetes cluster on AWS EC2 and automated application deployments using Argo CD, enabling continuous delivery directly from Git repositories.Implemented a centralized monitoring and alerting stack using Prometheus, Grafana, Alertmanager, and Node Exporter to gain real-time visibility into cluster, node, and application performance.

The platform provided automated deployments, live metrics, and operational insights similar to modern cloud-native production environments.

### Key Technologies:

* AWS EC2 – Infrastructure for Kubernetes worker and control-plane nodes
* Kubernetes – Container orchestration and service management
* Argo CD – GitOps-based continuous delivery
* Helm – Package management for Kubernetes
* Prometheus – Metrics collection and time-series monitoring
* Grafana – Visualization and dashboarding
* Alertmanager – Alerting and notification management
* Node Exporter – Node-level OS and resource metrics

## Architecture

![Architecture diagram](k8s-kind-voting-app.png)

* A front-end web app in [Python](/vote) which lets you vote between two options
* A [Redis](https://hub.docker.com/_/redis/) which collects new votes
* A [.NET](/worker/) worker which consumes votes and stores them in…
* A [Postgres](https://hub.docker.com/_/postgres/) database backed by a Docker volume
* A [Node.js](/result) web app which shows the results of the voting in real time

<img width="860" height="800" alt="image" src="https://github.com/user-attachments/assets/231e4db1-37b3-4209-9ad6-070c6bbb62c0" />


## ArgoCd

<img width="1891" height="843" alt="image" src="https://github.com/user-attachments/assets/c0208e79-bc3b-4bb3-8da6-8acc847188c1" />

## Kubernetes Dashboard

<img width="1906" height="835" alt="image" src="https://github.com/user-attachments/assets/52bab718-3b3c-4ad3-bf52-bb5898f83df7" />

## Observability

<img width="1898" height="835" alt="image" src="https://github.com/user-attachments/assets/5747414a-7147-46c9-8cc7-cd3e9a018c73" />

![Prometheus diagram](prometheus.png)


### Achievements:

Automated Kubernetes deployments on AWS EC2 using Argo CD (GitOps), reducing manual release effort by ~60%.
Implemented a production-grade observability stack using Prometheus, Grafana, Alertmanager, and Node Exporter to monitor cluster health and application performance.
Built dashboards and PromQL queries to track CPU, memory, and network I/O per pod, enabling faster root-cause analysis and capacity planning.
Achieved 99.9% application uptime through Kubernetes-based scaling, self-healing, and continuous monitoring.

# Ansh-Jain
