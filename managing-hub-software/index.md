---
title: "Managing MagneTag Hub Software"
excerpt: "The MagneTag Hub is the software that powers your system."
toc: true
---

The MagneTag Hub is the software that powers the MagneTag system.

## Controllers Overview

A controller is a view for working with a specific part of the MagneTag Hub or for working in a specific way.

There are four main controller types, each with a different purpose. These are:
* **[Self-Service (Kiosk) Controller](self-service-controller)**: The self-service controller lets games run without a staff attendant. It's designed to work with a touch screen, allowing customers to start their own games.
* **[Full-Service (FEC) Controller](full-service-controller)**: The full-service controller is designed for use in a staffed environment. The staffer uses the controller to operate games.
* **[Tournament Controller](tournament-controller)**: The tournament controller manages tournaments. It creates a seeded single-elimination bracket, keeps track of players, and manages game play.
* **[Admin Controller](admin-controller)**: The admin controller is for administering the system. This includes configuring the Hub, configuring armor vests and other devices, managing users, and basic troubleshooting.

## Devices and Controllers

Each armor vest (and any other devices used for game play) must be assigned to a specific controller or controllers. This allows a single MagneTag Hub to run multiple game stations. For instance, there may be two separate full-service controllers, each with four armor vests assigned to them. This would allow two different sets of games to be operated simultaneously, with each one having up to four players.

Devices can also be used among multiple controllers. For example, you could have two full-service controllers that share eight armor vests. This would allow two separate matches at a time, but also allow a single match with eight players.

## Users

A MagneTag system has multiple users. Each user has their own credentials (username and password). Like devices, users need to be assigned to controllers. Each user has specific permissions on a controller:
* **Interact**: Interact permissions allow the user to interact with the controller. This means that they see things like buttons and game configuration options that they can choose.
* **View**: View permissions allow the user to view the controller but not interact. This is generally used for displays (like an overhead projector, TV, etc.) that show the progress of a game, but don't need to show things like buttons.

## Common Scenarios

* One station, one controller
* One station, multiple controllers
