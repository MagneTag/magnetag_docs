---
title: "Installation Troubleshooting"
excerpt: "Installation Troubleshooting"
toc: true
---

The troubleshooting here only applies if you have installed the MagneTag Hub on your own computer.

# Common Issues

Several issues can be verified by using the Config Utility. This file can be found at `C:\Program Files (x86)\MagneTag\ConfigUtility\MagneTag.ConfigUtility.exe`.

## Firewall

There are several ports used by the MagneTag Hub that must be open by your firewall. Refer to [Managing the MagneTag Network](managing-network) for more details.

You can use the Config Utility to create firewall rules:
`MagneTag.ConfigUtility.exe /action:openports`

## Certificates

MagneTag uses certificates to secure data being transmitted between various components.

To see if the certs are installed:
`MagneTag.ConfigUtility.exe /action:info`

To create the personal cert:
`MagneTag.ConfigUtility.exe /action:createpersonalcert`

To create the personal cert and install it as a trusted root:
`MagneTag.ConfigUtility.exe /action:createifnotexists`

## ACLs

ACLs need to be created, and certs assigned to those ACLs. You can use the Config Utility to create those ACLs:
`MagneTag.ConfigUtility.exe /action:executenetsh`

## SQL Server

A local SQL Server instance is required for the MagneTag Hub. By default, SQL Server Express is installed.