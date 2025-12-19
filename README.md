# enterprise-network-lab
This is a Enterprise Network and System Administrations lab that I improved upon from my old university course using cisco packet tracer. The core aim of the lab was to set up a star topology network where all devices are connected to a central device.

<img width="80" height="80" alt="image" src="https://github.com/user-attachments/assets/e642e642-7956-42f6-b217-47f9c7c7db0e" />

The new lab differs from the old lab in these key areas:
1) Added a router and the internet to the network instead of just having the devices and the switch.
2) Created virual devices using VirtualBox to simulate real-world devices on a network alongside a physical which held Windows 11 but was replaced with Ubuntu Linux to have different operating systems on the network.
3) Utilized Nagios to monitor the network paired with the simulation from cisco packet tracer to demonstrate end to end routing, and switching concepts.

## Table of Contents
- [Cisco Packet Tracer](#cisco-packet-tracer)
- [Nagios](#nagios)
- [Installing Linux](#installing-linux)

## Cisco Packet Tracer
In this part of the project, I created a simulated office environment using a Star Topology Network.
* I used Subnetting to organize the IP addresses efficiently.
* Multiple devices are connected to a switch which communicates with the company's local server. The LAN is connected to a router which allows them to access the internet.
* This video simulates ARP communication on a local network as well as acessing the internet (HTTP).
  
[![Watch the video](https://github.com/user-attachments/assets/8444873c-baad-4a16-8af4-8316035a765c)](https://youtu.be/4IRTN0SaSos)

## Nagios
This part of the project is a basic display of Nagios Core and Nagios Cross-Platform Agent.
* 3 Virtual Windows Machines have Nagios Cross-Platform Agent (NCPA) installed, the laptop is Linux and has Nagios Core installed.
* This video demonstrates a very basic display of using host groups in nagios to to identify cpu usage in the virtual machines.
  
[![Watch the video](https://github.com/user-attachments/assets/a0f586be-f48e-4b4b-bb2d-e346644dc0cf)](https://youtu.be/l43_DVRSUuo)

## Installing Linux
1) Normally, installing linux requires creating a bootable USB drive (usually 8GB or more) by flashing the OS ISO (burning the OS unto the USB). This allows you to replace the existing operating system cleanly. Since I didn't have access to a USB I decided to allocate disk space on my C drive to create a separate partition to install Linux wwith it's own dedicated storage.
   
2) Afterwhich I accessed the BIOS and disbaled Secure Boot which allos the system to boot up a non Windows operating system.
   
3) To complete this, I used the Machine Owner Key (MOK) to finish the Secure Boot configuration and finalized it by installing Ubuntu Linux using GRUB as the bootloader.
   
4) Once Linux was installed, I removed the remaining partitions holding Windows and merged the unused disk space with the Linux storage to reclaim memory.
