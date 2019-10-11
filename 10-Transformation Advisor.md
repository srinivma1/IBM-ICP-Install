


<div style="background-color:black;color:white; vertical-align: middle; text-align:center;font-size:250%; padding:10px; margin-top:100px"><b>
 Installing IBM TransformationAdvisor on IBM Cloud Private
 </b></a></div>

---
# Installation of Transformation Advisor on ICP Cloud
---

![ICP Logo](./images/logoicp.png)



# Table of Content
---
- [Installation of Transformation Advisor on ICP Cloud](#Installation of TransformationAdvisor on ICP Cloud)
- [Table of Content](#table-of-content)
- [1. Prerequisites](#1-prerequisites)
- [2. Install TA on icp](#2-install TA on ICP)
    + [Task 1 : Create secret](#task-1---create secret)
    + [Task 2 : Add Docker’s official GPG key](#task-2---add-docker-s-official-gpg-key)
    + [Task 3: Add a repo to get the Docker](#task-3--add-a-repo-to-get-the-docker)
    + [Task 4: Get Docker](#task-4--get-docker)
    + [Task 5: Download IBM Cloud Private](#task-5--download-ibm-cloud-private)
    + [Task 6: SSH Keys setup](#task-6--ssh-keys-setup)
    + [Task 7: Customize ICP](#task-7--customize-icp)
    + [Task 7: Install ICP](#task-7--install-icp)
    + [Task 8: Install and configure CLIs](#task-8--install-and-configure-clis)
    + [Task 9: Adding persistent storage to Kubernetes](#task-9--adding-persistent-storage-to-kubernetes)
    + [Task 10: End of installation](#task-10--end-of-installation)
- [5. Second Option: Using Vagrant and VirtualBox](#5-second-option--using-vagrant-and-virtualbox)
- [6. Conclusion](#6-conclusion)
    + [Results](#results)
- [End of Lab](#end-of-lab)
- [appendix A : Preparing your VM (VMWare) with Ubuntu](#appendix-a---preparing-your-vm--vmware--with-ubuntu)
    + [Task A1 - Download Ubuntu](#task-a1---download-ubuntu)
    + [Task A2 - Create a VM](#task-a2---create-a-vm)
    + [Task A3 - Set the language](#task-a3---set-the-language)
    + [Task A4 - Set the keyboard](#task-a4---set-the-keyboard)
    + [Task A5 - Install Ubuntu Server](#task-a5---install-ubuntu-server)
    + [Task A6 - Select Location](#task-a6---select-location)
    + [Task A7 - Select locales](#task-a7---select-locales)
    + [Task A8 - Choose a hostname](#task-a8---choose-a-hostname)
    + [Task A9 - Choose a username](#task-a9---choose-a-username)
    + [Task A10 - Type a password](#task-a10---type-a-password)
    + [Task A12 - Partition your disk](#task-a12---partition-your-disk)
    + [Task A13 - No Proxy](#task-a13---no-proxy)
    + [Task A14 - Launch the installation](#task-a14---launch-the-installation)
    + [Task A15 - Add some packages](#task-a15---add-some-packages)
    + [Task A16 - GRUB](#task-a16---grub)
    + [Task A17 - Login for the first time](#task-a17---login-for-the-first-time)
    + [Task A18 - Get the IP address](#task-a18---get-the-ip-address)
    + [Task A19 - SSH to the VM](#task-a19---ssh-to-the-vm)
    + [Task A20  - Update the OS](#task-a20----update-the-os)
    + [Task A21 - Define the network interface](#task-a21---define-the-network-interface)
    + [Task A22 - You are now ready to start the ICP installation](#task-a22---you-are-now-ready-to-start-the-icp-installation)
- [appendix B : Changing ICP admin password](#appendix-b---changing-icp-admin-password)
    + [Task B1 - Login to your ICP cluster using ssh](#task-b1---login-to-your-icp-cluster-using-ssh)
    + [Task B2 - Generate your new ICP password in base64](#task-b2---generate-your-new-icp-password-in-base64)
    + [Task B3 - Edit ICP secrets](#task-b3---edit-icp-secrets)
    + [Task B4 - Delete the auth pods](#task-b4---delete-the-auth-pods)
    + [Task B5 - Test the new password](#task-b5---test-the-new-password)
- [appendix C : How to connect to a cluster](#appendix-c---how-to-connect-to-a-cluster)
- [End of Appendix](#end-of-appendix)
---


# 1. prerequisites

Install IBM Private cloud on Ubuntu VM. If not done  already, please follow the instructions below:
   
        https://github.com/srinivma1/IBM-ICP-Install/blob/master/1-ICPInstallationLab.md
        
        
# 2. install TA on ICP

Install IBM Private cloud on Ubuntu VM. If not done  already, please follow the instructions below:
   
        https://github.com/srinivma1/IBM-ICP-Install/blob/master/1-ICPInstallationLab.md        
        
        

