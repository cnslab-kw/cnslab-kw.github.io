---
title: "CNS Lab - Research"
layout: textlay
excerpt: "CNS Lab -- Research"
sitemap: false
permalink: /research/
---

# Research Area

<!--Click for Korean descriptions-->

## I. Software-Defined Networking (SDN) Security

Over the past decades, SDN has been advocated as a next-generation Internet architecture by both academia and industry.
By separating the control plane from the data plane, it is possible to perform network management and monitoring in a centralized manner (i.e., controller), facilitating the emergence of new applications.
Indeed, we have seen that numerous innovative applications have been proposed, such as network virtualization (e.g., FlowVisor, VMware NSX), software-defined measurement (e.g., OpenSketch, DREAM), and WAN traffic optimization (e.g., Google B4).

[(<i class="fa-solid fa-hand-point-right"></i> See Lumezanu's SDN reading list if you're interested in more.)](https://sites.google.com/site/sdnreadinglist/)

### 1) Security *by* SDN

Meanwhile, from a security perspective, SDN also brings us great opportunities to design a novel security application for addressing timely security issues.
With SDN, security systems can be easily developed by utilizing the SDN benefits: i) direct control and ii) centralized monitoring \[[Shin *et al.*, ICCCN '16](https://nss.kaist.ac.kr/papers/SDNSok-ICCCN16.pdf)\]. 
Thus, in this project, we aim to design new SDN-based security systems that can reactively or proactively prevent network threats.
So far, we have designed two SDN-based proactive defense systems:

#### BottleNet: Hiding Network Bottlenecks Using SDN-Based Topology Deception (TIFS '21)

BottleNet is a network topology deception system that exposes a fake node and link information to protect network bottlenecks.
It is widely known that there are a few critical nodes and links, i.e., network bottlenecks, that tie small networks to a larger network.
Attackers could discover those nodes and links with network scanning tools (e.g., traceroute) and target them to incur significant damage to the network at a low cost.
BottleNet helps operators find those potential network bottlenecks with diverse metrics and deploy virtual nodes and links to prevent an attacker from discovering them.

#### EqualNet: A Secure and Practical Defense for Long-term Network Topology Obfuscation (NDSS '22)

EqualNet is another network topology deception system we have designed to hide network bottlenecks in a more fine-grained way.
It generates fake responses from SDN switches when attackers send probes to a target network, thereby preventing attackers from distinguishing any critical link.
Meanwhile, it also achieves the practicality of fake responses by considering the IP range the target network belongs to so that network operators could obtain correct subnet information.

### 2) Security *of* SDN

Till now, a security of SDN has been a major concern because such a new architecture is likely to expose a new attack surface as well.
This project aims to investigate security issues by exploring all potential SDN attack surfaces.

#### Finding potential threats in multi-controller SDN environments (ongoing work)

Recently, many WAN operators have adopted multi-controllers in their SDN network architecture to guarantee robustness and high-performance of a control plane.
To build a physically separated but logically centralized control plane, communicating between controllers via East and West interfaces is necessary.
In this context, we posit that it is possible to have the presence of a malicious or misbehaved controller in a controller cluster.
Based on this hypothesis, this project aims to reveal such potential threats in multi-controller environments. 

## II. Cloud Computing Security

Cloud computing is a rapidly evolving area that adopts new and diverse virtualization technologies to realize multi-tenant environments. 
As many different technologies, such as Linux kernel, Docker, Kubernetes, and OVS, intertwine each other, unexpected attack surfaces could be exposed to remote attackers.
Thus, our goal is to reveal potential security issues in modern cloud environments.

### 1) Security *of* OS-level Virtualization

<!--#### Finding potential threats in container environments (ongoing work)-->

Nowadays, OS-level virtualization---also known as *containers*---is widely employed in cloud data centers. In contrast to the traditional VM (Virtual Machine)-based solutions, it facilitates a lightweight and low-cost server virtualization.
However, recent research has shown that a minor vulnerability of a malicious container could affect other containers due to the fact that all containers share the same kernel. 
In this project, we aim to broadly explore all threats a malicious container could perform in container environments.

### 2) Security *of* Network Virtualizaiton

*(to be updated)*



<!--#### Building a secure and reconfigurable virtual network (ongoing work)-->


<script src="https://kit.fontawesome.com/392aa12767.js" crossorigin="anonymous"></script>
