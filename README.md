## A steb-by-step guide to hosting Codalab-v2 instance and compute workers in de.NBI cloud

### Contents

- [1. Introduction](#1-introduction)
  - [1.1 Acknowledgements](#acknowledgements)
  - [1.2 Understand some lingo](#before-we-start)
  - [1.3 Prerequisites](#prerequisites)
- [2. deNBI dashboard](#2-deNBI dashboard)
  - [2.1 SSH-keys](#ssh-keys)
  - [2.2 Resource modification](#resource-modification)
  - [2.3 Wiki help](#wiki-help)
  - [2.4 OpenStack login](#openstack-login)
- [3. Create VM instances](#3-create-vm-instances-using-the-openstack-dashboard)
  - [3.1 Create a network router `dmz-int`](#create-a-network-router)
  - [3.2 Codalabv2 main instance](#codalabv2-main-instance)
  - [3.3 Codalab worker instance](#codalab-worker-instance)
  - [3.4 Check final network topology](#check-final-network-topology)
- [4. SSH into your VM](#4-ssh-into-your-vm)
  - [4.1 Ping test and change netplan](#ping-test-and-change-netplan)
  - [4.2 Download Docker](#download-docker)
  - [4.3 Download Docker Copmpose](#download-docker-compose)
  - [4.4 Change Docker MTU value](#change-docker-mtu-value)
- [5. Install Codalabv2 competition instance](#5-install-codalabv2-competition-instance)
  - [5.1 Installation](#installation)
  - [5.2 Edit `.env` file](#edit-env-file)
- [6. Install Codalabv2 worker instance](#5-install-codalabv2-competition-instance)
  


## 1. Introduction

[TO DO]

---

### Before we start

- ** What is COMETH ?**

- ** What is Codalab ?**

- ** What is de.NBI ?**

- ** What is ELIXIR ?**

- ** What is de.NBI cloud ?**

- ** What is OpenStack ?**

----

### Prerequisites

This tutorial presumes that you have already performed these steps -

- Created a valid functioning deNBI cloud account
- Requested and obtained the necessary computational resources for setting up a virtual machine (VM)

---

If not, fulfil these prerequisites by following these steps - 

- **Create an ELIXIR account**

An ELIXIR account can be most simply created if you have a valid account for any of these participating [German institutions](https://elixir-europe.org/about-us/who-we-are/nodes/germany). Alternatively, if you do not belong to these institutions, ELIXIR accounts can also be created through - 

- Google account
- Linkedin
- ORCID

> **NOTE:** During the ELIXIR account registration process kindly note down your _Elixir username_. This will be needed and will come handy later on.

- **Create a deNBI account**

Perform your account registration and request for a project resources allocation (#CPU, memory, storage etc) by following the instructions provided here - 

1. [Getting started](https://cloud.denbi.de/get-started/)
2. [Registration](https://cloud.denbi.de/wiki/registration/)
3. [Resource allocation](https://cloud.denbi.de/wiki/portal/allocation/)

> **NOTE:** Your project request will be approved by the Admins only if you (are a PI) or your PI belongs to deNBI participating German institute. You can of course add as many memebers from participating or non-participating institutes.

Ok, so now you have a deNBI cloud account and the Admins have sanctioned your project resources. Let's continue with the next steps.

[Back to top](#contents)

---

## 2. deNBI dashboard

### SSH Keys
Goto https://cloud.denbi.de/ and login (click PORTAL LOGIN)
Under Project Management (on the left), click on your (1) project name and (2) click login URL

### Resource modification

### Wiki help

### OpenStack login

[Back to top](#contents)
---

## 3. Create VM instances using the OpenStack dashboard

> A detailed explaination of the various aspects of the OpenStack dashboard in Learn more about [OpenStack dashboard](https://docs.openstack.org/horizon/latest/user/index.html)

[Back to top](#contents)
---

## 4. SSH into your VM

