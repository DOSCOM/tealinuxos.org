---
title: Network and Internet Connection
type: panduan
order: 107
---

## Connecting and Disconnecting networks

 ![menu] (https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
`→ Settings → Network Connection`
or click the ![networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager` icon located in panel` → Edit.`
The network connection in TealinuxOS Pappermint uses a network connection to manage networks using wired, wireless networks, mobile broadband, VPN and DSL connections. Network connection will connect your computer automatically with the network, but the first connection usually requires security information to connect to the network.

To disconnect the network click on the ![Networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
`NetworkManager` icon located on the panel then click` disconnect.`

## Configuring the connection

 If you want to configure your network, In the Netwok Connection dialog box you will see the existing network connections. Choose either to set the configuration or you can add a new network connection by selecting `Add.`

## Sharing the connection to another computer

 You can share a connection to another computer using an Ethernet cable. For the setting click the icon ![Networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager → Edit` then select` Add` in the dialog box select the type of connection you want, After clicking the create button on the tab `IPv4 Settings` select the method used.

## Troubleshooting on the network

If your network connection is not working perfectly you can use some way to find your connection error.

### Checking connection information

- Using the NetworkManager icon
 ![networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager → Information`. If the information is disabled it is probably because your computer is not connected to the network.
-    Using ifconfig
    Open terminal (short cut terminal guake: F12)
    Type the ifconfig command then enter.
    This ifconfig will show your connection information includes the connection name, IP address in inet addr, and MAC address in Hwaddr.


### Checking if the connection works

To check whether your chef is working or not you can test it through ping.

-    Open the terminal
-    type the command

            ping tealinuxos.org

-    then enter.

If the connection is successful you will receive a message in the form of the number of packet statistics transmitted. If you get the `ping: unknown host tealinuxos.org` then your computer may not be connected to the internet and can not reach the Domain Name System (DNS) server.