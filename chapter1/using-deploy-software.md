# AX3 Download/Deployment Software

## Getting Started


### Hardware

For 3x laptops:

1. Connect laptop to power.

2. Connect 2x USB docks to power.

3. Connect 2x USB docks to the computer over USB.

4. Connect barcode scanner to the computer over USB.

5. Verify that the laptop has a working internet connection at all times (otherwise the laptop will not be able to upload the data files, and it does not have much spare capacity).


### Installing the software

If the software is not already installed, it is available from: [https://openlab.ncl.ac.uk/gitlab/public-pages/ax3-deploy/](https://openlab.ncl.ac.uk/gitlab/public-pages/ax3-deploy/).  To install, click the *AX3 Deployment Tool Setup* link, and run the downloaded *setup.exe* program.  If told *Windows protected your PC* then click *More info* and *Run anyway* -- you will also need to install the *AX3 Driver* from the same site.


### Starting the software

Double-click the *Deploy* icon from the desktop (or press the *Start* button and type `Deploy` to find the launch shortcut):

![Deploy icon](../assets/launch-icon.png)


### Interface Overview

The user interface is split into several areas:

![User interface](../assets/interface-areas.png)

1. *Configuration setting*: This should be scanned in by the barcode reader, but can be typed if needed.

2. *Configuration information*: Provides information, success messages, and error messages.

3. *Device details*: Lists each attached device grouped by status, including the device id, battery level and status detail.

4. *Diagnostic log*: Typically ignored in normal use, can be checked for further details in the event of a problem.

5. *Cloud upload progress*: which file it is uploading and how many other files are queued for upload.

6. *Available space*: the approximate number of downloads that the drive currently has capacity for.


### Device Status

The status of each device is indicated by the device's LED colour:

| LED Colour  | Status  | Notes  |
|:------------|:--------|:-------|
| <span style="font-color: black;">&#9676;&nbsp;White</span>  | Downloading  | The data from the device is downloading.  You must wait for the download to complete.  Afterwards, the device will be automatically cleared then enter the charging or charged category. |
| <span style="font-color: cyan;">&#9679;&nbsp;Cyan</span>  | Recharging  | The device is cleared but not yet fully charged.  Wait until the device is fully charged. |
| <span style="font-color: magenta;">&#9679;&nbsp;Magenta</span>  | Charged  | The is fully charged (and cleared).  This device can be configured now, or is ready to be removed for later configuration.  |
| <span style="font-color: cyan;">&#9788;&nbsp;Flashing (Cyan/Off)</span>  | Outbox  | The device is configured.  Disconnect the flashing device, scan the barcode and place in the envelope. |
| <span style="font-color: red;">&#9679;&nbsp;Red</span>  | Unexpected  | This device was not expected on the dock, as it has been configured for recording and that recording has not yet finished.  If you are certain that the device was configured in error, use *Device* / *Destroy Recording* to manually clear it.  The firmware may temporarily light the LED red while it is clearing or configuring.  |
| <span style="font-color: blue;">&#9679;&nbsp;Blue</span>  | Error  | There was a problem with communicating with, or downloading from the device.  If it is a comms. error, press `F9`, `Y` to reset.  If it is a download error, check the drive has enough free space (waiting for uploads to complete may free-up capacity).  |
| <span style="font-color: yellow;">&#9679;&nbsp;Yellow</span> / <span style="font-color: green;">&#9679;&nbsp;Green</span>  | USB Error  | This device is not communicating with the computer (but is powered or fully charged). Check the hub's connection and reconnect the device.  |
| <span style="font-color: black;">&#9677;&nbsp;Fading Yellow / White</span>  | Unclassified  | This device has not been given a status by the software.  If this persists, try reconnecting the device, restarting the computer and ensuring the drivers are installed.  |
| <span style="font-color: red;">&#9788;&nbsp;Flashing Red</span>  | Starting  | The device is starting.  Technically, either in a low-battery pre-charge state, or in the 'bootloader'.  If it persists and fails to start properly, then remove the device from circulation.  |


## Operation: Download, Clearing and Recharging

Steps:

1. Fill all free spaces on the docks with devices from the *incoming* bucket.

2. After the devices settle, you expect to see LEDs which are: **white** (downloading) and **cyan** (cleared and recharging).  Downloading of 14 devices in parallel takes approximately 18 minutes, recharging could take a little longer.

3. When devices turn **magenta** they are fully charged and should be removed to a *charged* bucket.

4. If any devices turn **blue**: check if it is a download error (confirm the free space on the laptop, waiting for uploads to complete may free-up capacity), or a communication error (press `F9`, `Y` to reset these devices).

5. Repeat from step 1 while devices remain in the *incoming* bucket.


## Operation: Configuring

Steps:

1. Fill free spaces on one or more docks with devices from the *charged* bucket.

2. After the devices settle, you expect to mainly see LEDs which are **magenta** (charged), and perhaps some **cyan** (recharging).  

3. On a laptop with at least one **magenta** (charged) device, scan the barcode from the letter.  The configuration numbers should appear at the top, and one of the devices (the most charged) will be configured and start to flash.

4. Remove the flashing device from the dock.

5. Scan the device you have removed (this double-checks the device is the configured one).

6. Place the device in the envelope (with the letter).

7. Repeat from step 3, or step 1 if you need more devices.


