# Polybar-NetworkStatus

![](https://i.imgur.com/keE3Y8h.png)    ![](https://i.imgur.com/Br6ZkC2.png)    ![](https://i.imgur.com/CKmyza0.png)

A very simple network status module for polybar, replacing the polybar's default one.

## Features
- Dynamically showing wifi and ethernet connection (with the default network module, you have to create 2 seperate modules to show both wifi and ethernet status).
- Showing download speed in KB/s and MB/s, just like the default one.
- Supporting ramp format for wifi strength signals.

## Installation
First, put the network_status.sh in ~/.config/polybar.

After that, add these lines to the polybar config file:
```
[module/network-custom]
type = custom/script
interval = 1
exec = bash ~/.config/polybar/network_status.sh
```
Finally, add the module to bar and reload to see the result.

Note: You can change the colors of the icons and network speed, just edit them in the script.
