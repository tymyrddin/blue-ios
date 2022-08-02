# Change MAC address

A MAC address identifies the device connected to a network and allows the network to track, restrict or allow access 
based on it. Routers identify and assign static IP addresses based on the MAC addresses of devices. Before you try to 
change the MAC address, you need to know the value that you want to use.

Set the 2's place bit (the "locally administered" bit) in the first byte, to differentiate it from a guaranteed 
globally unique MAC address. Usually the first three bytes an unicast MAC address is an 
"Organizationally Unique Identifier" (OUI) that the IEEE assigned to the manufacturer of your Ethernet device. 
Manufacturers are required to make sure they keep the last 3 bytes unique. 

Avoiding all of that knowledge, the [MAC address generator tool](https://miniwebtool.com/mac-address-generator/) can 
generate a valid address for you.

Not possible with <14. The iOS 14 update brought with it the Private Address feature that lets you hide your original 
MAC Address of iPhone. You can enable the private address on your iOS for a Wi-Fi connection. When enabled, your 
iOS will always use a private MAC for that (public) Wi-Fi network.

* Connect to the Wi-Fi network you want to hide the iPhone MAC address from.
* Open Settings.
* Tap on Wi-Fi.
* Tap the "i" icon next to the connected Wi-Fi network.
* Toggle on "Private Address".
* Reconnect to the Wi-Fi network.
