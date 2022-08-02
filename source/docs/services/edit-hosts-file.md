# Edit hosts file

The hosts file is a system file on a device that lets you map specific domain names to an IP address. If you want 
to add new entries to the hosts file, you’ll need the IP address of the server that you want to map a hostname to.

    XXX.XXX.XXX.XXX some.domain.name 

The hosts file lets you override DNS entries for any domain name. There are lists of common ad networks and 
tracking servers available online which you can use to keep an up-to-date list of sites to block. Blocking is achieved 
by setting the IP address of the ad networks to a loopback address like 127.0.0.1 which will not return anything. 
There are lists of common ad networks and tracking servers available online which you can use to keep an up-to-date 
list of sites to block. 

If your device is infected with malware, then your hosts file may be compromised to included unknown entries for known 
domain names. *That* is NOT the IP address of your bank! This type of DNS attack is known as DNS pharming, and checking 
your `hosts` file can uncover potential infection.

## Linux

* Open terminal application
* In the terminal, give the command `sudo nano /etc/hosts`
* Enter your administrator password after running the command
* Add as many entries as needed

## Windows

To edit the hosts file (`C:\Windows\System32\Drivers\etc\hosts`) on Windows, you will need Administrator access. 

* Right-click on your text editor’s icon (for example Notepad++) and choose Run as administrator.
* Go to File → Open in the text editor and navigate to `C:\Windows\System32\drivers\etc\`
* From the list, click on the hosts file and choose Open
* Add as many new entries as needed

## MacOS

* Open the Terminal application. (Click on the Finder icon and then go to Applications → Utilities)
* In the terminal, give the command `sudo nano /private/etc/hosts`
* Enter your administrator password after running the command
* Add as many entries as needed

## iOS

iOS devices, such as the iPhone and iPad, use a `hosts` file to map hostnames to IP addresses. It can not be changed 
unless you 
* Jailbreak the device
* Use a portable Wi-Fi router and set iOS cto get DNS from the router and the router will need the custom `hosts` set up. 
* Tether it to an Android with custom `hosts` file. 

And that is most likely not enough in situations where governments are using DNS poisoning to block sites, like 
in China.

## Android
For Android there is a way using [Android Debug Bridge (adb)](https://developer.android.com/studio/command-line/adb), 
a command-line utility included with Google’s Android SDK. `adb` can control a device over USB from a computer, copy 
files back and forth, install and uninstall apps, run shell commands, etc. It is part of the 
[SDK Platform Tools](https://developer.android.com/studio/releases/platform-tools)

1. Open a terminal window.
2. Pull the hosts file out of the phone to your PC.
3. Edit it.
4. disable READ_ONLY of SYSTEM

```text
$ su
# mount -o rw,remount /system
```

5. Push the file back.
6. Put SYSTEM back to READ_ONLY: 

```text
# mount -o ro,remount /system
```

