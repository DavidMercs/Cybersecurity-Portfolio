# Welcome to My VirtualBox SOC Home Lab

**Status:** In Progress

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
3. [Creating and Configuring the Virtual Machines](#03-creating-and-configuring-the-virtual-machines)
4. [Installing the Operating Systems and Required Tools](#04-installing-the-operating-systems-and-required-tools)
5. [Network Configuration and Testing](#05-network-configuration-and-testing)


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




