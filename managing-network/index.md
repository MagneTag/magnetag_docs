---
title: "Managing the MagneTag Network"
excerpt: "Manage the network that the MagneTag system uses"
toc: true
---

The MagneTag system runs on TCP/IP.

## On-Premises Hub

In a on-premises scenario, there's a dedicated wireless network for the MagneTag system. There's a router for the network and, optionally, a bridge device that connects that router to the public-facing internet. The devices on the network include:
* MagneTag Hub PC
* Armor vests
* Credit/pulse devices (coin-op, card-swipe, etc.)
* Display PCs

## Cloud Hub

When using a cloud hub, there is no dedicated network for MagneTag. All the devices use existing networks on-site, and all connect to a cloud-based hub.

## Firewall and Ports

MagneTag devics need to be able to interact through the ports listed below:

* **UDP 4701**: The hub listens for devices on UDP 4701. Each device opens a single UDP port, usually in the 4710-4730 range.
* **TCP 4702**: The hub exposes this port for display clients. Transport on this port is always encrypted with TLS.
* **TCP 4703**: The display client is served on this port. The hub runs a web server on this port, and traffic is encrypted with TLS.
* **TCP 4704**: The hub runs an HTTP web server on this port that contains software updates. This is just used when performing over-the-air firmware updates on devices.
