---
title: TealinuxOS Installation
type: panduan
order: 102
---


## TealinuxOS Installation Guid
There is two ways for installing TealinuxOS to your device :
- Installing with bootable flashdisk
- Installing with bootable CD
If you use your CD you can skip the download TealinuxOS ISO and make bootable flashdisk.

### Download TealinuxOS
Tealinux ISO can download [here](http://pinguin.dinus.ac.id/iso/tealinuxos/).

### Make Bootable TealinuxOS ISO to Flashdisk
To make bootable to flashdisk you can use Third Party software such as [Universal USB Installer](https://universal-usb-installer.en.uptodown.com), [Unetbootin](http://unetbootin.github.io) or [Rufus](https://rufus.akeo.ie/). here is steps for making bootable TealinuxOS ISO using Universal USB Installer.
![Bootable_1](https://cloud.githubusercontent.com/assets/22718275/23578142/c4eae682-0102-11e7-9d76-69cd286a4406.png)

![Bootable_2](https://cloud.githubusercontent.com/assets/22718275/23578146/d6ebc932-0102-11e7-94c9-993dee8bcbe2.png)
About how to use, installation and more you can see at each official software  

### How to make hardisk partition for TealinuxOS
To make hardisk partition you can use `Create and format hard disk partition` for windows, `GParted` for Linux, or another tools usual to make partition.
There are 2 kinds of partition for TealinuxOS :
- Partition with format 'ext4'. This partition is working to store TealinuxOS system.
  for example we make 50 GB or 50000Mb partition. Right click on the disk that you want to shrink. Why 50GB? Because 50GB is ideal, and minimal size for linux is 20GB.
  ![Partition_1](https://cloud.githubusercontent.com/assets/22718275/23578147/e2c49112-0102-11e7-868e-611db63be0a2.png)

  ![Partition_2](https://cloud.githubusercontent.com/assets/22718275/23578150/f11bd6d0-0102-11e7-815c-b4648866def9.png)

- Partition with format `linux-swap`. This partition works to help RAM manage memory for swap recondtion partition.


### TealinuxOS Installation Process
1. After you have bootable, make sure you connect the bootable to your device.
2. Restart your device to start TealinuxOS installation process.
3. Change booting option to your bootable. you can enter to BIOS and change BIOS mode to Legacy (if using UEFI/EFI mode).
4. Then change boot priority USB HDD(): to the first place if you use flashdisk or change boot priority CD(): to the first place if you use CD.
5. Save your settings and restart.
6. Wait a moment until it appears the menu as the following :
   ![menu-install](https://cloud.githubusercontent.com/assets/22718275/23685947/5be6f430-03d9-11e7-89c0-d55cfb593f9e.png)
7. Choose `Try TealinuxOS` to try or Install TealinuxOS` to install directly. If you choose install TealinuxOS then you can skip step 6 and 7
8. Wait for a while until TealinuxOS Desktop appears as follows :
   ![try-install](https://cloud.githubusercontent.com/assets/22718275/23685964/736151be-03d9-11e7-9b11-23af4063ab3b.png)
   If you agree, you can try all the features on TealinuxOS before installing. Then choose Install TealinuxOS icon on the desktop to install
9. You will see the interface as below:
   ![language](https://cloud.githubusercontent.com/assets/22718275/23685988/96e996fa-03d9-11e7-9cc0-b5664ed27a17.png)
   You are asked to choose the language to further use, choose OK to continue.
11. Next you are asked to choose to download third party software or not. Click ok to go on.
    ![preparing](https://cloud.githubusercontent.com/assets/22718275/23685998/a811ae18-03d9-11e7-8c6f-1900f9a85b7d.png)
12. Next you are prompted to select the installation procedure as follows :
    - Install TeaLinuxOS Alongside Them
      This option can save file like document, etc.
    - Erase disk and Install TeaLinuxOS
      This option will erase all data on disk. (This option  is reserved for those of you who do not want dual boot, because this option will delete all the existing OS and data.)
    - Something else
      This option is for you who want dual boot. Because in this option you can set the partition that we created earlier. Pilihan ini dikhususkan bagi anda yang ingin dualboot.
    ![instalaltion](https://cloud.githubusercontent.com/assets/22718275/23686028/cd308aac-03d9-11e7-9fa7-217fd1f7ac08.png)
    Pilih something else lalu klik ok.
13. You will get an interface like the following :
    ![partiton_1](https://cloud.githubusercontent.com/assets/22718275/23686041/e39d8f38-03d9-11e7-8836-e749fb8b0794.png)
    As you can see on the interface, there is 2 partition that you made on previous step and that is `/dev/sda1` which sized 50GB and `/dev/sda5` which is 2GB in size. For information the partition name may differ between this tutorial and your device.
14. Change the partition type `/dev/sda1` by clicking the change button. Set it to `ext4`, format the partition and move mount point to '/'. Choose OK to continue. format partisi dan juga arahkan mount point ke `/`. Klik OK untuk lanjut.
    ![Partition_2](https://cloud.githubusercontent.com/assets/22718275/23686049/f5030230-03d9-11e7-8834-7ecac4b9b6bb.png)
    ![partition_3](https://cloud.githubusercontent.com/assets/22718275/23686061/03f969f0-03da-11e7-8bda-eb56c7c8cf04.png)
15. CChange the partition type `/dev/sda5` by clicking the change button again, and set it to `swap area`. Choose OK to go to next step.
    ![Partition_4](https://cloud.githubusercontent.com/assets/22718275/23686081/1fbf6266-03da-11e7-8daa-4a60c06703e5.png)
    ![partition_5](https://cloud.githubusercontent.com/assets/22718275/23686146/6dbf052a-03da-11e7-85e3-e844b273f694.png)
16. There will be agreement screen as follows :
    ![Partition_6](https://cloud.githubusercontent.com/assets/22718275/23686161/857a51e2-03da-11e7-8011-a9fb063761b4.png)
    Click continue to proceed.
17. You will be asked to choose the time and place.
    ![time-and-region](https://cloud.githubusercontent.com/assets/22718275/23686187/a58ca03e-03da-11e7-827a-01f86abe8ec3.png)
18. You are asked to choose keyboard type also.
    ![keyboard](https://cloud.githubusercontent.com/assets/22718275/23686208/b682f4ce-03da-11e7-8dcb-85c8ef2cbbad.png)
19. You have to fill your personal data.
    ![whoru](https://cloud.githubusercontent.com/assets/22718275/23686238/d5fdd5e4-03da-11e7-8387-626587c4ede8.png)
20. Wait a few moments until the installation process is complete.
    ![installaltion](https://cloud.githubusercontent.com/assets/22718275/23686286/31ab73ec-03db-11e7-8292-173401c6851a.png)
21. Restart and you can enjoy TealinuxOS
    ![success](https://cloud.githubusercontent.com/assets/22718275/23686381/df3fda20-03db-11e7-9ee1-a811f1646f36.png)
