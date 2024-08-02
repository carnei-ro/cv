# Leandro Carneiro

## Who am I

I'm a nerd who loves new tech. I started my career working with open-source software, and now I love it. Constantly testing a new OSS solution and probably helping to improve it by opening "Pull Requests" to their code. Enjoys Cloud, Containers, Kubernetes, Proxies, and the community.

## Objective

I am looking for a company that solves people's life problems to work remotely in SRE / DevOps / Platform Engineer areas.

## Contact

- **Address:** Jundiaí / SP / Brazil
- **E-mail:** leandro@carnei.ro
- **GitHub:** @carnei-ro
- **LinkedIn:** https://www.linkedin.com/in/leandro-souza-carneiro-5762ba96

## Academic Background

- **Course:** Computer Engineering <br/>
  **Degree:** Bacharel - B.S. <br/>
  **Conclusion:** Dec/2012 <br/>
  **Institution:** Universidade São Francisco

- **Course:** Computer Technician <br/>
  **Degree:** Technical <br/>
  **Conclusion:** Dec/2007 <br/>
  **Institution:** Colégio Divino Salvador

## Exchange Courses

- **Course:** English for non-Americans <br/>
  **Duration:** 1 month <br/>
  **Conclusion:** Mar/2014 <br/>
  **Institution:** ELS Language School - Silicon Valley

## Certifications

- **Title:** Terraform Associate <br/>
  **Company:** HashiCorp <br/>
  **Issued:** Sep/2019 <br/>
  **Valid Until:** Sep/2021

- **Title:** Kong Champion <br/>
  **Company:** Kong <br/>
  **Issued:** Apr/2023 <br/>
  **Valid Until:** N/A

## Languages

- **Portuguese**: Native
- **English**: Fluent

## Professional Background

- Senior Site Reliability Engineer @ **Namely** - From: Mar/2023 Until: Present
- Staff SRE @ **iFood** - From: Oct/2018 Until: Mar/2023
- Senior IT Infrastructure Analyst II @ **ADTsys Software** - From: Mar/2018 Until: Sep/2018
- IT Infrastructure Analyst @ **Programarte (simplesmenteUse)** - From: Jul/2010 Until: Mar/2018

### Work Accomplishments at Namely / PrismHR

- Revamp the Infrastructure as Code using Terraform/OpenTofu and Terragrunt to deploy the resources in AWS and Azure. The project was based on the "everything as code" concept, and it was a significant improvement in infrastructure management, helping also in SOC compliance.
- Implanting Atlantis to automate the Terragrunt changes. Using Atlantis also allowed the automation of Kubernetes changes made by Kapitan.dev and Helm.
- Observability project: Substitution of SignalFX agents by OpenTelemetry Collector to receive, process, and ship traces and metrics.

### Work Accomplishments at iFood

- Research and Implanting the iFood Service Mesh. Based on Istio, using the "multi-primary on different networks" architecture, the mesh had more than eight Kubernetes Clusters connected and thousands of services. The use of Istio "Sidecar" objects to control the number of hosts the proxy would watch was necessary from the beginning (this is an advanced technique). The team I was part of was responsible for building the mesh from the ground and delivering, at least, the same functionalities iFood already had, such as Authentication (PeerAuthentication and RequestAuthentication), Authorization (AuthorizationPolicy), Canary (via VirtualService) and observability.
- Creation of an Authentication and Authorization mechanism to be used between microservices and users calling microservices. It was based on the NGINX Ingress Controller, Lua, and JWTs. This project was before iFood Service Mesh, and it was fundamental to iFood internal APIs security, starting the "zero trust" culture for those APIs, also, avoiding internal DDoS caused by a bad functional application / script.
- Adoption of Atlantis (runatlantis.io) to automate, not just Terraform / Terragrunt code, but other projects that can be used following the "plan/apply" mode, such as Helm (with Helmfile) and "istioctl". This adoption created a standardized interface for our developers to interact with multiple layers of our infrastructure.
- Creation of an API Platform based on Kong supporting up to 100k Requests Per Second in peak hours; Using the concept of "everything as code", the infrastructure relies on AWS Ec2 instances, with Autoscaling Groups and Application Load Balancers. Those API Gateways clusters have been configured by the developers in a GitFlow fashion by submitting plain Kong Configuration to the pipeline, which validates, tests, and deploys those changes with minimal human interaction. The observability stack was based on Prometheus metrics, OpenSearch logs, and traces.
- Developed several Kong plugins in Lua to solve many problems, such as authentication, authorization, rate-limiting, logging, and metrics. I gave back to the community some of those codes, and it has been part of Kong. Contributions to the "Rate-Limiting", "Zipkin" and "Prometheus" plugins.
- Secrets management project: Implanting from scratch HashiCorp Vault with High Availability, fully "infrastructure as code" using Terraform, monitored with Prometheus Stack, and audit with ElasticSearch. Simplifying the management of the secrets and giving more autonomy to developers. In the very early stage of the project, I could contribute to HashiCorp's Vault K8s CSI Provider.
- Research and implantation of HashiCorp Consul to be used as the "backbone" of the iFood "feature flag" system, also following all the best practices and infrastructure as code.
- Participation in migrating almost all iFood resources from one AWS Region to another, using only "infrastructure as code". The process involved the creation of Terraform modules, understanding legacy infrastructure, and creating parse scripts for the automation of the task. During the day of the migration, I set up a Wi-Fi network with Bind9 with RPZ, allowing people to test everything before we change the DNS records.

### Work Accomplishments at ADTsys

- Development of a Python tool to bid Spot Instances on AWS Cloud and register them in OpsWorks stack/layers based on CloudWatch alerts.
- Creation and management of Chef 'recipes' for machine configuration via OpsWorks.
- Development of 'manifests' in Puppet to code our clients' environments, legacy and new.
- Translation of Ansible 'playbooks' to Puppet 'manifests' to equalize the environment.
- Development of 'pipelines' at Jenkins for automation of application deployments in CI/CD environments.

### Work Accomplishments at Programarte

- Research, implementation, and documentation of WildFly cluster, containerized and orchestrated by docker swarm, geo-redundant and scalable. The project was developed from scratch for a high availability environment for product "simplesmenteUse - NEO" in AWS infrastructure or on-premises.
- Email servers migration to Zimbra. Configuration of Zimbra itself, besides the DNS and firewall. The project has increased availability, stability, and log analysis.
- Shell script, in Jenkins "freestyle mode" job, for automation of various processes such as product deploy, server checking, backup / restore files from file servers and databases (Oracle, SQL Server, MySQL, and MongoDB). These automatons have decreased human error.
- Develop proof of concept online store project. Built with Angular 5 and Firebase, the project has been used to practice new technologies and to present the DevOps culture to the company coworkers. In these projects, it has configured the git pre-commit tool to run the lint and some tests before the push. After the push,  GitLab triggered Jenkins declarative pipeline, via webhook,  that checks out the code, runs the test (using json-server to mock the Firebase), builds the SaSS and modules, creates a Docker Image that was pushed to GitLab registry, then updates the server.

## Hard Skills

- **Container Orchestration:** Kubernetes
- **Cloud:** AWS and Azure. GCP per inference, helps if it is "as code".
- **Languages:** Python, Lua, Golang, Shell, Groovy
- **Automation:** Atlantis, GitHub Actions, GitLab CI/CD, Terraform, OpenTofu, Terragrunt, Helm, Helmfile, Packer, Jenkins, Vagrant.
- **Operational Systems:** Mainly Linux. It has been a long time since I heavily used Windows.
- **Secrets Manager:** HashiCorp Vault, AWS Secrets Manager, Azure Key Vault
- **Proxies:** Kong API Gateway, Istio, OpenResty, Nginx
- **CDN / WAF:** Akamai, CloudFlare
- **Virtualization:** QEMU KVM
- **Configuration Managers:** Chef, Ansible

## Soft Skills

- Fast Learning
- Resilience & Perseverance
- Problem-Solving
- Adaptability

## OpenSource Contributions

- Kong/kong-plugin-prometheus
- Kong/kong-plugin-zipkin
- Kong/kong
- Kong/kubernetes-ingress-controller
- Kong/deck
- hashicorp/vault-csi-provider
- hashicorp/consul-helm
- terraform-aws-modules/terraform-aws-iam
- terraform-aws-modules/terraform-aws-s3-bucket
- OpenIPC/firmware
- dyrkin/tasmota-exporter
- kovetskiy/mark
- helmfile/vals
- helmfile/helmfile
- asdf-vm/asdf-plugins
