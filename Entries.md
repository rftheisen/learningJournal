# Learning Goals for the rest of 2020
    1. Pass CEH by May 15th *Scheduled* 
    2. Pass OSCP by August 20th 
    3. Finish Cisco CCNA video series on YouTube by June 1st 
    4. Pass CCNP Enterprise Core by December 11th 
    5. Obtain my BSIT Degree by the end of Fall semester 



# Goal Accomplishment Strategy 
    1. Doing HacktheBox, Tryhackme challenges, reading Mike Walkers book, and completing Practical Ethical Hacking Course 
    2. Find funding to purchase, go through training course on Offensive Security's site, practice bash and powershell skills,
        and use platforms from first goal.
    3. Schedule time in the week to work on recording the content
    4. Complete CBTNuggets course, Read Cisco Press CCNP book, and setup GNS3 lab in VMware esxi and upgrade server memory
    5. Take summer courses and keep doing well in class

# Accomplished:

-  Build hyperconverged home lab by March 20th 
-  Build remote access lab functionality for classes by March 20th


## Setting up and testing Ubuntu Client in GNS3 with nested virtualization: 

- Must upload a VMDK file from client to server when creating the appliance 
    https://www.osboxes.org/ubuntu/#ubuntu-19-04-vmware
- Then you must specify the ISO that is going to be used to book the VM into Ubuntu
- GNS3 has tightvnc integrated for graphical terminal access to the OS
- When using ssh to connect to the router Ubuntu returns an error that indicates an older cipher suite is being used on the router, this prevents successful connection
- Trying telnet worked, we will comeback to the ssh
    https://www.openssh.com/legacy.html
- dsqst found that we needed to use a less secure cipther to connect via Ubuntu so we used this command: 

    ``` ssh -c aes128-cbc ltn@192.168.0.1 ```
- In the industry it would recommended that we upgrade the IOS image on the device to an images with up to date ciphers and methods with SSH 

## Setting up and testing Windows Server 2016 in GNS3: 
- The Windows Server appliance on GNS3s Marketplace does not work properly
- Must get .gns3a code from Github repo, and create your own file.Make sure to give it .gns3a extension
- Download qemu config file straight from appliance import screen
- Once all the file are uploaded make sure you turn on the device :p!
    - I spent far too much time trying to troubleshoot an error message when really I needed to just power the appliance on.
