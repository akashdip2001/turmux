# turmux
Turmux all comments 

# You should run these commands if you are a first time user

```
$: pkg update

$: pkg upgrade

$: apt update

$: apt upgrade

$: pkg install python

$: pkg install python2

$: pkg install git

$: pkg install nano

$: pkg install php

$: pkg install curl

$: pkg install openssh

$: termux-setup-storage
```
# kali Linux install 
```
- apt update

- apt upgrade

- termux-setup-storage

- apt install wget

- wget -O install-nethunter-termux https://offs.ec/2MceZWr

- chmod +x install-nethunter-termux

- ./install-nethunter-termux
```
# starting Kali Linux 
```
- nh 
$: sudo su 
password: kali 

#: sudo apt update 
#: sudo apt upgrade 
```
# VS Cord install 
Downloading code server

```
wget https://github.com/cdr/code-server/releases/download/v3.10.2/code-server-3.10.2-linux-arm64.tar.gz
tar -xvf ./code-server-3.10.2-linux-arm64.tar.gz
cd code-server-3.10.2-linux-arm64
```
Set up a password and start using VS Code

```
export PASSWORD="password"
code-server
```

# How to use Nmap in termux

Install and use Nmap in Termux



NMAP (Network Mapper) is a free and open-source network scanning tool widely used by network administrators and cybersecurity professionals to discover and map devices on a network. It can scan a range of IP addresses or a single host to identify the services and operating systems running on it. In this article, we will discuss how to install and use NMAP in Termux.

nmap in termux

Installing NMAP in Termux

1. Open Termux on your Android device and update the package repository by running the following command:
```
pkg update && pkg upgrade -y
```
2. Install the Nmap package by running the following command:
```
pkg install nmap 
```
3. To verify the installation, you can run the nmap command with the --version option
```
nmap --version 
```
nmap in termux

Using NMAP in Termux

NMAP provides a wide range of options for scanning networks and hosts. Here are a few examples of how to use NMAP in Termux:

Scanning a range of IP addresses

To scan a range of IP addresses, you can use the -sL option followed by the range of IP addresses you want to scan. For example, to scan the range 192.168.1.1-255, you can use the following command:
```
 nmap -sL 192.168.1.1-255
```
This will list all the IP addresses within the specified range.

Scanning a single host

To scan a single host, you can use the -sV option followed by the hostname or IP address of the host you want to scan. For example, to scan the host www.example.com, you can use the following command:
```
nmap -sV http://scanme.nmap.org/
```
This will scan the specified host and report the services and operating system running on it.

Scanning a range of ports

NMAP can also be used to scan a range of ports on a host. To do this, you can use the -p option followed by the range of ports you want to scan. For example, to scan the range of ports 1-1000 on the host www.example.com, you can use the following command:
```
 nmap -p 1-1000 www.example.com
```
This will scan the specified host and report the status of the ports within the specified range.

Performing an OS detection scan

NMAP can also be used to detect the operating system of a host. To do this, you can use the -O option followed by the hostname or IP address of the host you want to scan. For example, to detect the operating system of the host www.example.com, you can use the following command:
```
nmap -O www.example.com
```
This will scan the specified host and attempt to detect the operating system running on it.

