# TryHackMe OpenVPM Connection Problem
In this tutorial you will be able to connect to TryHackMe OpenVPN server in Egypt without a problem
# The Problem Description
for some reason with the ISPs in Egypt you might have problems connection to an openVPN service with a [UDP](https://www.freecodecamp.org/news/tcp-vs-udp/) config
and for time being TryHackMe doesn't provide a [TCP](https://www.freecodecamp.org/news/tcp-vs-udp/) config file, we won't cover the differences between [UDP](https://www.freecodecamp.org/news/tcp-vs-udp/) and [TCP](https://www.freecodecamp.org/news/tcp-vs-udp/)
but it is an intersting topic anyway this is not a networking course so let's get into it
# Step 1 : installing openVPN
## Installing on Windwos 
We will be using Winget package manager open the terminal and enter this command 

    winget install -e --id OpenVPNTechnologies.OpenVPN
## Installing on MacOS
We will be using homebrew package manager open the terminal and enter this command 

    brew install openvpn
## Installing on Linux (Debian)
We will be using APT package manager open the terminal and enter this command 

    sudo apt install openvpn


