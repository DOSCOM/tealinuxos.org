---
title: Managing Installed Apps
type: panduan
order: 109
---

## Installing Software


### Installing applications using the internet

Make sure your computer is connected to a computer network because the installation will directly download the application package you want to install from ubuntu repository. The easiest way is through the Software Center.

Click ![menu] (https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Software`
 ![software-center](https://cloud.githubusercontent.com/assets/26142091/23578129/6d894e06-0102-11e7-8672-2a7212299881.png)


Or through terminal, Open terminal and
Type command:

    sudo apt-get install name_of_the_package

Enter your computer password.
When there is dialog `" Do you want to continue? (Y / n) "` type `" y "`
Wait until the download and installation process is complete.
Run the app by calling the package_name in the terminal or you can look it up in the menu.

### Installing applications without internet
If you have an application with extension .tar.gz, .deb or .tea you can install it without an internet connection.

-    Installing .tar.gz apps
    Open your terminal then type the command

        tar xzvf nama_file.tar.gz
        
    (command to extract the file)
    Go to the extracted folder
    
        cd file_name
        
        ./configure

        make
        
        sudo su
            
        #make install
    Generally tar.gz files are installed using the above commands but if the application is not installed or an error occurs, you should read the README or INSTALL file which is usually included in the application file for installation guide.

-    Installing .deb apps
    If you want to install an application with extension .deb which is a debian package there are two steps.
     - Using Package Installer
       Double click on the .deb file
       click the Install Package button
       Enter your password
       Wait until the Installation finished message appears.
     - Using Terminal
       Open the terminal type command

            sudo dpkg -i nama_file.deb

- Installing the .tea app
    Installing the .tea app package using the Tea Package Installer
    
    ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ System → Tea Package Installer`
    Select `Find`
    Do a search where you put the .tea file
    Select `Install`
    Select `Continue` to finish.

- Installing via the Tea Module Installer
    To install the application via the Tea Module Installer you can view it [here](http://tealinuxos.org/support/tea-mudule-installer).

## Uninstalling Software

 To install certain software you can do it in the following way:
 Open the terminal and make sure first the package name you want to uninstall by using the command:
 
    dpkg -list

After you're certain with the package that you want to uninstall type command:

    sudo apt-get remove package_name

Enter password
Wait until the uninstall process is complete.

## Adding a Repository
Repository is a set of application packages or programs for an operating system (Linux) that is used to support the performance of an application, program and so forth obtained from the mirror server website packages. There are two ways to add the repository to the system.
 
  - Via Terminal
    Open a terminal, then type the command:

        sudo add-apt-repository ppa:creator_name/package_name

        sudo apt-get update

        sudo apt-get install nama_paket

  - Through the System
  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ Settings → Software & Updaters`
    In the Software & Updaters window select the `Other Software` tab
    Click the `Add` button
    Fill in the repository you want to add
    Click the `Add Source` button

## Installing via Tealinuxos IDE Installer
 
You can install your package using the TeaLinux IDE Installer as follows:

- Insert IDE Installer CD
- Run TeaLinux IDE Installer ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Accessories → tealinux-idea-installer`
- Select the package you want to install
- Click the `Install` button

## Updating software

 ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `Settings → Software Updater`
Updating the software can be done through Software Updater service, the system will check the software update and will download from internet and install the updates for the software.