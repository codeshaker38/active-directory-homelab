# Install Windows Server 2022

## Objective
The objective of this lab is to create a Windows Server 2022 virtual machine that functions as a Domain Controller and provide core network services for a Windows domain environment.

## Downloading Windows Server 2022 and Windows 11 Installation Media
Go to each website and download the respective installation media for both Windows Server 2022 and Windows 11, as seen in the screenshots below.

## Installing Oracle Virtual Box
If you don't already have Oracle Virtual Box installed on your device, make sure to download it from the website below. Don't forget to enable Virtualization on your device!

## Creating Your Windows Server 2022 Machine
Once you have the program running on your device, it's time to create the machines. 
1. First, click **"Machine"** in the upper menu and select **"New"**.
   <img width="1276" height="749" alt="image" src="https://github.com/user-attachments/assets/78643fc6-eeac-4c30-96ce-477a7aa40e01" />
2. Name the server machine to a proper name, like "WindowsServer2022", and select the **OS Version** to **Windows Server 2022 (64-bit)**.
   <img width="785" height="558" alt="Screenshot 2026-08-05 143008" src="https://github.com/user-attachments/assets/66e797a9-f41c-48a9-a71e-b71d977e92ba" />
3. After selecting **Finish**, power on the machine, the machine will be unable to boot without an ISO file. Select your Server 2022 download and try to reboot using your ISO.
<img width="720" height="486" alt="Screenshot 2026-08-05 143753" src="https://github.com/user-attachments/assets/7c0955c9-72c5-4b45-92ae-087faf6d4330" />

4. Once the virtual device has restarted, proceed through installation, selecting the **Language to install** to **English (United States)** and **Keyboard or input method** to **US**.
<img width="1024" height="851" alt="Screenshot 2026-08-05 144206" src="https://github.com/user-attachments/assets/aeff65a9-eb3a-40bd-b3e1-b4521cd4c7da" />

5. Proceed with installation, making sure to select **Windows Server 2022 Standard Evaluation (Desktop Experience)** to have GUI interface.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_14_46_22" src="https://github.com/user-attachments/assets/6fa6be9a-6231-43b5-8b00-10d6bd891707" />

6. Accept the **Microsoft Software License Terms** and select **Next**.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_14_50_15" src="https://github.com/user-attachments/assets/f07be987-046e-41ce-b716-7967c23d1f75" />

7. Select **Custom: Install Microsoft Server Operating System only (advanced)** as your type of installation.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_14_56_31" src="https://github.com/user-attachments/assets/b639baa9-c906-4c1f-ba8d-6a94529aebd6" />

8. Choose **Drive 0 Unallocated Space** as your destination for installing the operating system.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_14_58_41" src="https://github.com/user-attachments/assets/2d6fb2c5-46f7-466b-8510-2afbcb9735cf" />

9. Wait for installation to complete.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_14_59_30" src="https://github.com/user-attachments/assets/1085dc91-4ef8-442e-ae62-1cce7fd8c696" />

10. Once the device restarts a few times, enter a secure password.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_15_05_27" src="https://github.com/user-attachments/assets/3e869601-4051-4fd3-aefd-ffd52ea94187" />

11. Input **Ctrl-Alt-Del** using the **Input** menu and sign in.
<img width="1024" height="768" alt="VirtualBox_WindowsServers2022_05_08_2026_15_10_24" src="https://github.com/user-attachments/assets/c1e10ee8-c735-4034-ac8a-05b173f0beb4" />

Once you have Windows Server machine fully set up, set up a Windows 11 client device.

## Creating your Windows 11 Client Machine
1. Following the same steps as before, name the server machine to a proper name, such as "Windows11Client", set the **ISO Image** to your Windows 11 installation and your **OS Edition to Windows 11 Pro** to enable the device to be able to connect to a domain.
<img width="783" height="554" alt="Screenshot 2026-08-05 151711" src="https://github.com/user-attachments/assets/21f7daac-bc0b-4f0e-a144-98accf34baf0" />
2. In **Set up unattended guest OS installation**, place a temporary password in the box, this will only be used for initial access to the machine.
<img width="783" height="559" alt="Screenshot 2026-08-05 152423" src="https://github.com/user-attachments/assets/a3abbdef-a931-48df-9174-c719b324b7ff" />
3. Wait for Windows Installation to finish.
<img width="1024" height="768" alt="VirtualBox_Windows11Client_05_08_2026_15_25_41" src="https://github.com/user-attachments/assets/8a9e5193-69a6-456e-88d5-e9e7e36089d4" />






