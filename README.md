<h1>Active Directory Home Lab </h1>

<h2>Description</h2>
In this instructional guide, we will systematically guide you through the process of establishing an Active Directory home laboratory environment using Oracle Virtual Box. Engaging in the configuration and operation of this laboratory will significantly enhance your comprehension of Active Directory and Windows networking principles. I strongly recommend revisiting the tutorial multiple times, prompting yourself with questions when uncertainties arise, and ultimately attempting to replicate the setup independently, progressively reducing reliance on external guidance.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Powershell</b> 
- <b>Bash</b>
- <b>Python</b>
- <b>Windows Server</b>
- <b>Active Directory Users and Computers (ADUC)</b>
- <b>Active Directory Sites and Services</b>
- <b>Group Policy Management Consolo (GPMC)</b>
- <b>Virtualization Software (e.g., Hyper-V, VirtualBox, VMware)</b>

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

<h2>Install Windows Server 2019 on the virtual machine and assign IP addresses for the internal network.</h2>

