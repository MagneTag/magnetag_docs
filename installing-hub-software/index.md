---
title: "Installing MagneTag Hub Software"
excerpt: "The MagneTag Hub is the software that powers your system."
toc: true
---

## Installation Overview

Depending on your needs, you may need to install the MagneTag Hub on your own computer.

There are two components to the system:
* MagneTag Hub: This is the MagneTag software that powers your system.
* SQL Server Express: This is a database server that's used by the MagneTag Hub.

## Installing the Bootstrapper

To install the MagneTag Hub, you'll receive a file with a name like `MagneTag.InstallBootstrapper.n.exe`. Run this program, and it will install both SQL Server Express and the MagneTag Hub.

## Accessing the Hub

Once installed, you access the hub through a web browser. You'll need to know the name of your computer. If you don't know it, refer to https://support.microsoft.com/en-us/office/do-you-need-help-locating-your-computer-name-00384381-8aa9-4398-b81b-475f09fed618.

Once you know the name of your computer, open a web browser and navigate to `https://computername:4703/`. You should see a page asking you to log in. Here are the settings to use:
* Hub URL: https://computername:4702/
* Hub Instance: `Default`
* Hub Username: `admin`
* Hub Password: you'll be provided with an admin password

You can click the "Set Default" button to store these values so they'll be automatically populated in the future.

## Installing a License

After installing the MagneTag Hub, you'll need to obtain a license from MagneTag. In order to do this, you must provide your machine key. To do this:
* Log in to the hub
* On the "Select Controller" page, choose "Admin"
* On the right of this page, you'll see a table that lists the "Machine Key" -- it'll be around 30-40 characters
* Send this machine key to MagneTag, and we'll send you two files, `LicenseActivation.MagneTagLicense` and `LocationActivation.MagneTagLocation`
* Create a folder on your computer at `C:\Windows\ServiceProfiles\LocalService\AppData\Local\MagneTag\License` and copy those two files to that folder
* Reboot your computer
