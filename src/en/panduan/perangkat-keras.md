---
title: Hardwares
type: panduan
order: 111
---

## Multiple Driver Restrictions

### Why are some drivers limited?

Restricted Drivers are driver limitations for a hardware device because they are not available freely or open source.

Most devices (hardware) installed on your computer can function normally in TeaLinuxOS. These devices tend not to have driver limitations, which means drivers can be modified and problems with devices can be corrected.

When some hardware can not run smoothly in TeaLinuxOS it can be because the device has Restricted Driver. Usually hardware makers have not released the details of the hardware itself that allows for developers to create drivers of their own. Devices like this have limited functionality or may not work at all.

### Enabling Driver Restrictions

If Driver Restrictions are available for multiple devices, you can install them to enable your device to work properly.

If multiple drivers available for your device can be installed from the Software Source dialog:

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Settings Manager → Software & Updates`
- Available drivers will appear in the Additional Drivers tab, select and Apply Changes
- You will, if necessary, enter the administration password
- You may be prompted to reboot your computer after the installation process is complete

### Disabling Driver Restrictions

If Driver Restrictions cause problems, you can disable, follow these steps

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ Settings Manager → Software & Updates`
- Click Additional Drivers
- Find the drivers to disable and press the Deactivate button
- You will be asked to enter a password administration



## Disk and Partition


### Check how much disk space is left

An easy way to check the available disk space is to use File Manager. Here are some steps to take

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ Accessories → File Manager`
-   Double-click in File System or Home icon on Desktop
-   Click the home folder in Lancher Panel

The status bar at the bottom of the window shows the available space of the selected drive or disk. If you have more than one drive installed or connected, you can click on the side pane and you will see the free space on the drive or disk.

### Increasing disk space

Some easy ways to give more space:

- Empty the trash by right clicking on Trash icon on Desktop or Launcher Panel and select Empty Trash
- Remove the unused software package again.
- Delete unneeded files.

### Partitioning your Device

You can use GParted (GNOME Partition Editor) to partition the storage device. Click ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Settings Manager → GParted` to start the partition editor

### Free the space for the new partition

To create a new partition on a device that has been partitioned, you must resize the available partitions. If you already have an empty space, skip this step and go to Create a new partition. If not, follow the steps below:

-   Select the device to be partitioned from the drop-down list located at the top right of the main window
-   The partition list will appear in the main window. Select the partition you want to resize and from the menu select `Partition → Unmount`
-   To change the partition select `Partition → Resize / Move.` Resize / Move dialog will appear. You can use the Free Space Following (MiB) box to choose how much space will be emptied after the partition, or Free Space Preceding (MiB) to empty space before this partition.
-   Click `Resize / Move`
-   To apply the changes, click `Edit → Apply All Operations`

### Creating a new Partition

To create a new partition:

-   Select the device to be partitioned from the drop-down list at the top-right of the main window.
-   List of partitions will appear. Select unallocated, right click and click New
-   From File system: pick list, choose the type of filesystem to use.
-   If required, enter the partition description in the Label: field
-   Click the Add button
-   To apply the changes, click `Edit → Apply All Operation`

### Formatting Partitions

To delete a partition, do the following:

-   Select a device from the drop-down list at the top right of the main window
-   List partition will appear. Select the partition and select `Partition → Unmount`
-   Select the partition to be formatted and select `Partition → Format to` and select fil type
-   To apply the changes, click `Edit → Apply All Operations`

### Mounting and Unmounting devices

When you install a removable storage (ex: Flashdisk) to your computer, the device should be mounted by the operating system that allows you to access files on that device

To find how to mount and unmount storage devices manually and/or automatically, see the Ubuntu community wiki page for [mount command](https://help.ubuntu.com/community/Mount).

When you copy files from removable storage devices, they are not always written on the device directly. Instead the device will be stored in a queue so that they can all be transferred to the device at the same time (for efficiency reasons).

## Laptop

### Power management settings

You may want to change your laptop's power management settings to help conserve battery life.

- ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ Settings Manager → Power Manager`
-   Change the settings accordingly
-   Changes applied can be directly viewed

### Touchpads

Most laptops have a touchpad, which is used to control the mouse pointer. There are many ways to change how the touchpad works; basic touchpad settings can be configured in the following ways:

- ![menu] (https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ Settings Manager → Mouse and Touchpad`
- On the `Device` tab: select` touchpad`
- You can change the touchpad settings to your liking.

## Suspending and Hibernating

To save power, you can switch your computer to one of a number of power-saving modes when you are not using it:

`Suspend` is a command to make your computer asleep. The computer will still be activated and all work will be left open, using less power. You can wake the computer by pressing the button or clicking the mouse.

`Hibernate` is shutting down the computer completely while saving the state of the computer (like keeping all open documents). When you restart the computer after Hibernate, all your work must be restored as it was before Hibernate. No power is used when the computer hibernate.

`Shutting Down` is shutting down the computer completely without saving the state while the computer is still alive. No power is used when the computer is turned off.

`Resumming` takes the computer out of the power saving mode and returns to normal operation.

You can manually switch the computer to power saving mode by pressing `Menu → logout` and then select the appropriate mode button.

### My computer is not suspended or hibernated correctly

Some computers can not Suspend or hibernate properly in TeaLinuxOS. You may notice some of the following symptoms:

- The computer does not die after you click to hibernate it.
- When you turn on the computer after hibernating it, your previously open programs are not live.
- The computer does not wake up after the suspend process.
- Certain programs or hardware stops working correctly after resuming from hibernate or suspend.

If you encounter this problem, you must [report the bug](http://tealinuxos.org/support/bug.tealinuxos.org). The problem will hopefully be fixed in the next version of TeaLinuxOS. If your hardware does not work properly after suspend or hibernate the computer, restart your computer. If the program is not working correctly, try closing the program and then starting again.

## Mouse and keyboard

When you install TeaLinuxOS you are given the option to choose the keyboard type and language. During installation, the pointing device must be automatically detected and configured. If you want or need to change the settings of each of these devices after installation, you can do so by clicking ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13. png)
    `→ Settings Manager → Mouse and Touchpad` or ![menu] (https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Settings Manager → Keyboard .`

Options for mouse and touchpad include:

-   Key orientation
-   Speed ​​of pointer and sensitivity
-   Double-click sensitivity
-   Cursor Theme



Some options for configuring your keyboard include:

-   State of the Num Lock key on startup
-   Key repeat speed and delay
-   Cursor blinking speed
-   Application keyboard shortcuts
-   Keyboard layout and language









