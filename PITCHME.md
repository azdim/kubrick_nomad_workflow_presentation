---
marp: true
title: Marp CLI example
description: Hosting Marp slide deck on the web
theme: uncover
style: |
    section{
          font-size: 30px;
    }
paginate: true
_paginate: false
---

![bg](#123)
![](#fff)

###### <!--fit--> Deploying Nomad jobs using a CI/CD pipeline
![width:800px height:5cm](assets/tools.png)

---
![bg](#123)
![](#fff)
# What is [Nomad](https://www.hashicorp.com/solutions/workload-orchestration)?
* A lightweight application orchestrator.
* Can manage both containers as well as legacy applications.
* Get started with [Nomad](https://learn.hashicorp.com/collections/nomad/get-started).
---

![bg](#123)
![](#fff)

## Nomad vs Kubernetes

![width:800px height:12cm](assets/nomad_kube.png)

###### source: [Nomad docs](https://www.nomadproject.io/docs/nomad-vs-kubernetes#nomad-vs-kubernetes)
---

##### Architecture of a typical Nomad cluster

![width:800px height:12cm](assets/architecture.png)


![bg](#123)
![](#fff)

---
![bg](#123)
![](#fff)
##### What does each component do?

* Load balancer: Distributes incoming traffic across servers.
* Nomad Servers: Distribute incoming workload based on Job specification and client capacity.
* Nomad Clients: Execute workload.

---
![bg](#123)
![](#fff)
# Useful docs

* [How do I know the number of servers?](https://www.nomadproject.io/docs/internals/consensus#raft-protocol-overview)
* [How do servers and clients interact?](https://learn.hashicorp.com/tutorials/nomad/production-deployment-guide-vm-with-consul#overview)
* [What drivers does Nomad support?](https://www.nomadproject.io/docs/drivers#task-drivers)
* [What is a Nomad Job?](https://www.nomadproject.io/docs/job-specification#job-specification)

---
###### <!--fit--> The problem

![bg](#123)
![](#fff)

---
##### How does a developer deploy Jobs that require underlying infrastructure to mutli-DC Nomad clusters and minimise downtime?

![width:700px height:12cm](assets/job.png)



![bg](#123)
![](#fff)

---
###### <!--fit--> Pipelines!
![bg](#123)
![](#fff)

---
#### Why Pipelines?
* Provide dev, test and prod environments.
* Deploy underlying infrastructure and build nomad variables file.
* Dynamically construct Nomad job file based on variables and environment.
* Stop dev, test Jobs and clean up infrastructure.
* Manage secrets within pipeline.
![bg](#123)
![](#fff)

---
#### [Pipeline overview](https://excalidraw.com/#room=cf09ef76f2f233f01317,YQTHALCf_qRCrGKTpADqMg)

![width:1100px height:9cm](assets/pipeline.png)

![bg](#123)
![](#fff)

---
###### <!--fit--> Demo time 🥳
![bg](#123)
![](#fff)

---
# Fun Fact
* This presentation was built using Markdown and GitHub actions pipeline. If you would like to give it a try check [this repository](https://github.com/yhatt/marp-cli-example).
![bg](#123)
![](#fff)

---
# [Checkout my blog page](https://azdim.github.io) 🤓

![width:1000px height:12cm](assets/blog.png)
![bg](#123)
![](#fff)

---
###### <!--fit--> Thank you
![bg](#123)
![](#fff)

