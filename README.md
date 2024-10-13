<h1>Active Directory Home Lab </h1>

<h2>Description</h2>

This instructional guide, inspired by [Josh Makador's](https://www.youtube.com/@JoshMadakor) content, will walk you through the process of setting up an Active Directory home laboratory environment using Oracle VirtualBox. By configuring and working with this lab, you will deepen your understanding of Active Directory and Windows networking concepts. I encourage you to revisit the guide as needed, actively question any areas of uncertainty, and eventually try replicating the setup on your own while gradually minimizing your reliance on this documentation.

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Windows Server 2019</b>

<h2>Diagram</h2>

![image alt](https://github.com/CarlGoc/ActiveDirectoryLab/blob/559c8f44ad1d79d95b803d8aa07443839d10cd83/active_directory_diagram.jpg)

<h2>Download and install Oracle VirtualBox from the official website.</h2>

[Oracle Virtual Box](https://www.virtualbox.org/)

<h2>Download the ISO files for Windows 10 and Windows Server 2019.</h2>

[Windows 10 ISO](https://www.microsoft.com/en-us/software-download/windows10) [Windows 2019 Server](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

<h2>Create a new virtual machine in VirtualBox by clicking 'New,' naming it 'Domain Controller,' and selecting the Windows Server 2019 ISO file as the boot media.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/4eb4fe5d440527da2824173046d33c794ce666ab/image.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/4eb4fe5d440527da2824173046d33c794ce666ab/image2.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/4eb4fe5d440527da2824173046d33c794ce666ab/image3.png)

<h2>Configure the virtual machine with two network adapters: one for internet access and another for the private network.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/4eb4fe5d440527da2824173046d33c794ce666ab/image4.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/4eb4fe5d440527da2824173046d33c794ce666ab/image5.png)

<h2>Install Windows Server 2019 on the virtual machine and configure IP addressing for the internal network.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/14de7616a1ac79595e33a78645d4664cd9adfec5/image6.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/14de7616a1ac79595e33a78645d4664cd9adfec5/image7.png)

<h2>Name the server and install Active Directory to set up the domain</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/14de7616a1ac79595e33a78645d4664cd9adfec5/image8.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/14de7616a1ac79595e33a78645d4664cd9adfec5/image9.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/14de7616a1ac79595e33a78645d4664cd9adfec5/image10.png)

<h2>Configure routing to enable clients on the private network to access the internet through the domain controller.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/10498a66b31c2daf76c5b73b2c43237b9829841f/image11.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/10498a66b31c2daf76c5b73b2c43237b9829841f/image12.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/10498a66b31c2daf76c5b73b2c43237b9829841f/image13.png)

<h2>Setting up DHCP on the Domain Controller</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/10498a66b31c2daf76c5b73b2c43237b9829841f/image16.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/10498a66b31c2daf76c5b73b2c43237b9829841f/image14.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/10498a66b31c2daf76c5b73b2c43237b9829841f/image15.png)

<h2>Execute the PowerShell script to generate 1,000 user accounts in Active Directory.</h2>

[PowerShell Script for creating users](https://github.com/joshmadakor1/AD_PS)

<h2>Set up a new virtual machine named "Client1" and install Windows 10 on it.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/00d9d3a878f1afa2ea351e6071d0f40570e6b73b/image19.png)

<h2>Connect the client machine to the private network and join it to the domain.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/00d9d3a878f1afa2ea351e6071d0f40570e6b73b/image17.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/00d9d3a878f1afa2ea351e6071d0f40570e6b73b/image18.png)

<h2>Log into the client machine with the domain account you've created.</h2>

![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/00d9d3a878f1afa2ea351e6071d0f40570e6b73b/image20.png)
![image](https://github.com/CarlGoc/ActiveDirectoryLab/blob/00d9d3a878f1afa2ea351e6071d0f40570e6b73b/image21.png)
