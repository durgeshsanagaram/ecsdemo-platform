## Overview

**ecsdemo-platform** serves as Phase 1 of the multi-part **Amazon ECS Workshop**. This repository provides the foundational automation scripts and configuration manifests required to provision the underlying platform—including VPCs, networking components, subnets, and security groups—necessary to deploy containerized microservices in subsequent workshop phases.

### Key Features & Infrastructure Tools

* **Foundational Layer:** Establishes the baseline cluster environment that hosts microservices like `ecsdemo-frontend` and `ecsdemo-nodejs`.
* **Infrastructure as Code (IaC):** Utilizes **Shell** scripting (100.0%) to programmatically configure environment variables, create security postures, and coordinate AWS resources.
* **Orchestration Configuration:** Features integration with **Mu** via `mu.yml` for simplified, declarative infrastructure lifecycle management.
* **CI/CD Integration:** Bundles an AWS CodeBuild specification file (`buildspec.yml`) to handle automated testing and provisioning hooks during deployment pipelines.

### Project Structure

* `/test` - Validation and sanity testing scripts to ensure the platform environment is correctly configured.
* `/images` - Diagrams or visual assets mapped to the workshop's architecture layout.
* `mu.yml` - Configuration blueprint defining the network, cluster settings, and pipeline parameters.
* `buildspec.yml` - Definition file mapping the steps for AWS CodeBuild execution.

# Amazon ECS Workshop

This is part of an Amazon ECS workshop at https://ecsworkshop.com
