<p align="center">
  <img
    src="https://github.com/user-attachments/assets/56eee73e-e17e-4c10-be11-e7825e1b8a7f"
    alt="Project 1: Setting Up My VirtualBox Home Lab"
    width="75%"
  />
</p>

<p align="center">
  <strong> DIFFICULTY LEVEL:</strong>
  <span style="color: #00C853;"><strong>🟢 EASY</strong></span>
</p>

# Welcome to My VirtualBox SOC Home Lab

**Status:** Completed

## Objective

The objective of this project is to build my own virtual lab environment using Oracle VirtualBox for cybersecurity learning and practice.

I will document the entire process from scratch, walking through each step of setting up my Home Lab. This includes installing and configuring the necessary applications, configuring the virtual network, and verifying that the lab environment is working as intended.

## Project Scope

This project focuses **only on the setup and configuration** of my VirtualBox Home Lab. You will see documents of the steps I followed, the configurations I applied, and the challenges I encountered along the way.

My main goal is to provide a clear, step-by-step guide showing how I built my own Home Lab, from the initial setup through completion.

## Tools Used
<div>
  <img src="https://img.shields.io/badge/Oracle%20VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white" alt="Oracle VirtualBox" />
</div>

## Operating Systems
<div>
  <img src="https://img.shields.io/badge/Windows%2010-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows 10" />
  <img src="https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Kali Linux" />
</div>


## Table of Contents
1. [Downloading the Required Files](#01-downloading-the-required-files)
2. [Installing VirtualBox and the Operating System](#02-installing-virtualbox-and-the-operating-system)
3. [Configuring the Virtual Network](#03-configuring-the-virtual-network)



## 01. Downloading the Required Files

Before setting up my VirtualBox Home Lab, I downloaded the necessary software and installation files required for the setup.
These files will be used to install VirtualBox, create virtual machines, and configure the lab environment in the following steps.

### Download Sources
- **Oracle VirtualBox:** https://www.virtualbox.org/wiki/Downloads
- **Windows ISO:** https://www.microsoft.com/software-download/
- **Kali Linux ISO:** https://www.kali.org/get-kali/
<img width="566" height="166" alt="image" src="https://github.com/user-attachments/assets/f16cd76f-0119-4aec-9095-29896d3c45a3" />

## 02. Installing VirtualBox and the Operating System

In this step, I installed Oracle VirtualBox on my host computer and prepared the operating systems for my Home Lab.

### 2.1 Installing Oracle VirtualBox

I chose Oracle VirtualBox because, based on my research, it is beginner-friendly and easier to use.

After installation, I opened VirtualBox Manager to verify that it was working correctly.

<p align="center">
  <img src="https://github.com/user-attachments/assets/c50ce70a-abec-499d-af09-d128060b706c" alt="Oracle VirtualBox Manager" width="600" />
</p>

### 2.2 Installing the Operating Systems

After setting up VirtualBox, I proceeded with installing the operating systems inside virtual machines. This involved creating the virtual machines, allocating hardware resources, and following the operating system installation process.

**Operating Systems:** Windows 10 and Kali Linux

<p align="center">
  <img src="https://github.com/user-attachments/assets/a2c4cbc4-0d97-4276-ac2c-b578c77b7605" alt="VirtualBox operating system setup" width="700" />
</p>

### 2.3 Verifying the Operating Systems

After installing both operating systems, I started each virtual machine to verify that Windows 10 and Kali Linux were running successfully.

<table>
  <tr>
    <th>Kali Linux</th>
    <th>Windows 10</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/5fa2ecfe-9a53-4b60-9952-83bd97841e77" alt="Kali Linux running in VirtualBox" width="400" />
    </td>
    <td align="center">
    <img src="https://github.com/user-attachments/assets/008d0d53-7529-4444-89e9-24dc69ea239d" alt= "Windows 10 running in VirtualBox" width="400" />   </td>
  </tr>
</table>

## 03. Configuring the Virtual Network
 In this step, I configured the network settings of my virtual machines to allow them to communicate as required for my Home Lab.
 Based on my research, I identified three network scenarios for my Home Lab.

**Scenario 1: NAT Network**
By default, the NAT Network is set. This will allow my Windows 10 and Kali Linux virtual machines to communicate with each other while accessing the internet.
<p align="center">
  <img src="https://github.com/user-attachments/assets/74e30486-073a-40c7-8f3c-baeb1c1150a5" alt="VirtualBox NAT Network configuration" width="550" />
</p>


**Scenario 2: Internal Network**
For this scenario, I will use Internal Network to allow my Windows 10 and Kali Linux virtual machines to communicate with each other without direct access to the internet or my host network. This provides a safe environment for testing tools that require communication between my virtual machines.

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/e293a5d5-03a7-4162-865e-e8438b8cb0dc" alt="VirtualBox Internal Network configuration" width="600" />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d8cac17c-d130-4500-a5af-4f8144dca04e" alt="Kali Linux Internal Network configuration" width="600" />
    </td>
  </tr>
</table>

Once I'm done with the settings, I now ran both VMs and statically assigned the IP settings manually.

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/638721fe-2174-4a9d-8beb-ba2e41089db5" alt="IP configuration for Windows 10" width="600" />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/6488411c-217a-4fc3-9a73-dc066cbb4f69" alt="IP configuration for Kali Linux" width="600" />
    </td>
  </tr>
</table>

And just to check if both VMs communicated with each other, I tried pinging Windows 10 to Kali Linux.

<p align="center">
  <img src="https://github.com/user-attachments/assets/47741a2d-06ba-4f7e-9bba-e21a691aae40" alt="Ping test between Windows 10 and Kali Linux" width="600" />
</p>

**Scenario 3: Isolated Environment for Malware Testing**

I also explored this network configuration for malware testing to reduce the risk of exposing my host computer and other devices to malicious activity.
<p align="center">
  <img src="https://github.com/user-attachments/assets/2c22fa39-2d64-4fad-903a-67db4ebd2c40" alt="VirtualBox network configuration for an isolated testing environment" width="600" />
</p>


## 🎉 Project Summary
<p align="center">
<img width="200" alt="Image" src="https://github.com/user-attachments/assets/0915b684-e613-44b3-8e16-e8ed90d78a13" />
</p>

Hooray, you made it to the end! That's how I installed, set up, and configured my VirtualBox Home Lab, from preparing the required files to configuring the virtual network and testing connectivity between my virtual machines. This Home Lab will serve as the foundation for my future cybersecurity projects.
<br></br>
[⬅️ Go back to my Cybersecurity Portfolio](../../README.md)










