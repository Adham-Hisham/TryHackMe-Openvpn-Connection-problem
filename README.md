# TryHackMe OpenVPM Connection Problem
In this tutorial you will be able to connect to TryHackMe OpenVPN server in Egypt without a problem
# The Problem Description
for some reason with the ISPs in Egypt you might have problems connection to an openVPN service with a [UDP](https://www.freecodecamp.org/news/tcp-vs-udp/) config
and for time being TryHackMe doesn't provide a [TCP](https://www.freecodecamp.org/news/tcp-vs-udp/) config file, we won't cover the differences between [UDP](https://www.freecodecamp.org/news/tcp-vs-udp/) and [TCP](https://www.freecodecamp.org/news/tcp-vs-udp/)
but it is an intersting topic anyway this is not a networking course so let's get into it
# Prerequisite
# Welocme to Cyper secuirty 
for this you will need to have a cup of coffee or something to drink before we begin
and we will need some hacker music so this will do [Watch Dogs](https://www.youtube.com/watch?v=OBRdjjRTt6c)
also i would like to mention Amr Mansour the requester of this tutorial and probably the only promoter as well
Thank you Amr
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
# Step 2 : Downloading FreeOpenVPN config
Download any config file you would like but make sure it is TCP
through [FreeOpenVPN](https://www.freeopenvpn.org/) but prefarably get the closest to you
# step 3 : connecting to the FreeOpenVPN service
navigate to the folder you downloaded the configeration file in

    cd Downlaods/
make sure you are in the right folder using Ls command

    ls
your output should conatain the name of the file we just downloaded
connect to it using this command

    openvpn REPLACE WITH THE NAME OF THE FILE
so it will look like this

    openvpn Germany_freeopenvpn.ovpn

# step 3 : connecting to the TryHackMe service
## downlaod the config file from TryHackMe
go to [TryHackMe](https://tryhackme.com/)
## after downloading the config file
now we are going to connect to it using the same way

    openvpn filename.ovpn
now you have successfully routed the connection through the first vpn making a small proxy chain and bypassed the issue
# Now you can close the first terminal and you won't lose your connection
and now you can go ahead and ssh into the machine in TryHackMe 

    ssh tryhackme@"THE GIVEN IP OF THE MACHINE"



