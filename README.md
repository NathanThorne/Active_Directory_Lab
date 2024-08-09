# Basic Home Lab Running Active Directory

This repository contains steps on how i set up a basic home lab running Active Directory

## Diagram
![image](https://github.com/user-attachments/assets/9c5f13a1-63bb-44fa-a6ba-0b508db57dbe)


## Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)
## Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)
[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

## Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.
![image](https://github.com/user-attachments/assets/6480fa99-bb35-428f-a62f-ca3f0f59fde9)

![image](https://github.com/user-attachments/assets/d15e40f4-1a86-41b0-9161-98d932796aff)

##  Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

![image](https://github.com/user-attachments/assets/408fd769-845e-444e-9a4a-61dbfb3359b1)

![image](https://github.com/user-attachments/assets/9914c05a-bb19-43ec-b138-3297f6042468)


##  Install Server 2019 on the virtual machine and assign IP addressing for the internal network.
![image](https://github.com/user-attachments/assets/202c7d19-dc01-4543-a045-199704753621)
![image](https://github.com/user-attachments/assets/65ed8397-b1b3-4b59-9271-ac0f8b0c2e30)

##  Name the server and install Active Directory to create the domain.
![image](https://github.com/user-attachments/assets/d9f3b8a4-a6eb-4536-adc5-f07072d3acc8)
![image](https://github.com/user-attachments/assets/3383f7da-e868-4f76-858e-7994a435607d)

##  Configure routing so that clients on the private network can access the internet through the domain controller.
![image](https://github.com/user-attachments/assets/7d989a10-62e0-4f58-bc55-ca7019aa9f70)
![image](https://github.com/user-attachments/assets/303c21d3-d38d-4a37-9cdc-7fb646907d4a)
![image](https://github.com/user-attachments/assets/12c9d5d5-4a39-4cd4-8c14-e15253679d02)

##  Set up DHCP on the domain controller.
![image](https://github.com/user-attachments/assets/eda9ff89-cd51-4f75-9b6a-d02ffccca84b)
![image](https://github.com/user-attachments/assets/bda3ac8d-25e2-4205-b251-0381426b49e8)
![image](https://github.com/user-attachments/assets/9d48c2f7-74df-4a60-9360-f30c732ce27b)

##  Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

##  Create a new virtual machine named "Client1" and install Windows 10 on it.
![image](https://github.com/user-attachments/assets/5abe5cce-a0f1-451a-a455-51580f20ac44)

##  Connect the client machine to the private network and join it to the domain.
![image](https://github.com/user-attachments/assets/8b4ea84d-fee0-4291-9405-86cd0ac2f6a2)

##  Log into the client machine with a domain account.
![image](https://github.com/user-attachments/assets/35a17d3f-8406-46f8-804a-ed7003dff0bb)
![image](https://github.com/user-attachments/assets/296be511-10ab-4210-adc0-334ae58f01fb)
