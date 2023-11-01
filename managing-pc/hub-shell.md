---
title: "MagneTag Hub Shell"
excerpt: "The MagneTag Hub Shell is an application for running the MagneTag Hub."
toc: true
---

When turned on, the MagneTag PC automatically runs an application called the "MagneTag Hub Shell". This is essentially an embedded web browser that's set to run a specific controller.

On self-service systems, the Hub Shell runs a self-service (kiosk) controller; on full-service systems, the Hub shell runs a full-service (FEC) controller.

The Hub Shell is designed to run as an alternative shell in Windows; when run this way, it means no other Windows applications (like Windows Explorer) are running. There's usually a user on the PC (called "Kiosk") that's designed to use the Hub Shell as its shell.

## Exiting/Rebooting

There are several hot keys available within the Hub Shell:
* Ctrl+Alt+F9: Closes the Hub Shell. If the Hub Shell is running as the Windows shell, this will mean there aren't any other applications (like Windows Explorer) running. At this point, you need to do a Ctrl+Alt+Delete to log out or shutdown.
* Ctrl+Alt+F10: Logs out the current user. This closes the Hub Shell, any other running applications, and returns to the Windows login screen.
* Ctrl+Alt+F11: Shuts down the computer.
* Ctrl+Alt+F12: Reboots the computer.

## Automatic Rebooting

The Hub software monitors the Hub Shell and, if it crashes or is closed, automatically reboots the PC. So if you close the app or log off, you have a small window of time (5 minutes by default) before the machine is restarted. Once the Hub Shell closes, you can run `shutdown /a` from a command-line to abort the pending reboot.

## Credentials

The Hub Shell stores credentials for the Hub, allowing a Hub user to be logged in automatically. There are some additional settings stored, like a URL for the Hub and a default controller to use.

These settings are stored in a file called "settings.json" in the user's application data folder. Assuming the Hub Shell is running for a user named "Kiosk", this file is at `C:\Users\Kiosk\AppData\Local\MagneTag\Shell`.

The following settings are available:
* `StartUrl`: the URL to load when the Hub Shell starts.
* `HubUrl`: the URL of the Hub to connect to.
* `HubInstance`: the Hub instance to connect to.
* `HubUsername`: the username of a Hub user to log in as.
* `HubPassword`: the password of the Hub user.
* `DefaultController`: the default controller to connect to.
* `FullScreen`: if set to true, the Hub Shell will run full screen; if false, it will run inside a resizable window.
* `AllowUserClose`: if set to true, allows the user to close the application.
* `ShowDevTools`: if set to true, shows the Chrome Developer Tools for the embedded browser running within the Hub Shell.

