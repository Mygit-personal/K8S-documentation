# 📦 Container Tools & Kubernetes Overview

## 📑 Table of Contents

- [📦 Container Tools \& Kubernetes Overview](#-container-tools--kubernetes-overview)
  - [📑 Table of Contents](#-table-of-contents)
  - [🐳 Container Tools](#-container-tools)
  - [☸️ Kubernetes Overview](#️-kubernetes-overview)
    - [Key Features:](#key-features)
  - [⚙️ Containerization vs Orchestration](#️-containerization-vs-orchestration)
  - [🏗️ Kubernetes Cluster Architecture](#️-kubernetes-cluster-architecture)
  - [🔀 Types of Kubernetes Clusters](#-types-of-kubernetes-clusters)
    - [1️⃣ Single Node Cluster](#1️⃣-single-node-cluster)
      - [Used For:](#used-for)
      - [Examples:](#examples)
    - [2️⃣ Multi Node Cluster](#2️⃣-multi-node-cluster)
      - [Used In:](#used-in)
      - [Provides:](#provides)
  - [🖥️ Self-Hosted Kubernetes Cluster](#️-self-hosted-kubernetes-cluster)
      - [Tools:](#tools)
  - [☁️ Cloud Hosted Kubernetes Services](#️-cloud-hosted-kubernetes-services)
  - [✅ Summary](#-summary)

---

## 🐳 Container Tools

Container tools are used to create and run containers. The most common tools include:

* **Docker**

  * Full container platform
  * Used to build, package, and run containers

* **containerd**

  * Lightweight container runtime
  * Extracted from Docker
  * Commonly used by Kubernetes

* **CRI-O**

  * Kubernetes-native container runtime
  * Directly implements CRI (Container Runtime Interface)

* **rkt (Rocket)**

  * Alternative container engine
  * Focused on security

---

## ☸️ Kubernetes Overview

Kubernetes is a container orchestration platform that helps manage containers across multiple servers.

### Key Features:

* Load balancing
* Auto-scaling
* Self-healing
* Zero-downtime deployments
* Rolling updates

---

## ⚙️ Containerization vs Orchestration

* **Containerization**

  * Creating containers
  * Done using tools like Docker

* **Orchestration**

  * Managing containers at scale
  * Done using Kubernetes

---

## 🏗️ Kubernetes Cluster Architecture

* **Master Node (Control Plane)**

  * Manages the cluster
  * Responsible for scheduling, API, and control

* **Worker Node**

  * Runs applications (containers)

---

## 🔀 Types of Kubernetes Clusters

### 1️⃣ Single Node Cluster

* Only one node
* Acts as both **master + worker**
* Control plane and applications run on the same machine

#### Used For:

* Learning
* Testing

#### Examples:

* Minikube
* K3s
* Kind

---

### 2️⃣ Multi Node Cluster

* Multiple nodes

  * One or more master nodes
  * Multiple worker nodes

#### Used In:

* Production environments

#### Provides:

* High availability
* Scalability
* Fault tolerance

---

## 🖥️ Self-Hosted Kubernetes Cluster

A **self-hosted cluster** is when we manually install and configure Kubernetes on our own infrastructure.

#### Tools:

* kubeadm
* KOPS
* kube-spray

👉 If a company is not using cloud, it is called **on-premises**.

---

## ☁️ Cloud Hosted Kubernetes Services

Managed Kubernetes services provided by cloud providers:

* **AWS → EKS (Elastic Kubernetes Service)**
* **Azure → AKS (Azure Kubernetes Service)**

---

## ✅ Summary

* Docker → Containerization
* Kubernetes → Orchestration
* containerd / CRI-O → Container runtimes
* Clusters → Single-node (learning) & Multi-node (production)
* Deployment → Self-hosted (on-prem) or Cloud-hosted

---
