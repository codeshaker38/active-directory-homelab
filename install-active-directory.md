# Install Active Directory
## Objective
The objective is to install Active Directory on the server machine and configure it to be a domain controller for the network.
## Installing Active Directory
To make locating your device easier in the network, go to **Local Server**, click **Computer name** and click **Change** in order to change the name of your machine to whatever you like. 

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_14_46_50" src="https://github.com/user-attachments/assets/cc8114f7-be48-454c-b08a-319439e0770c" />

Once your computer has restarted, the changes will have taken effect.

1. In the **Server Manager - Dashboard**, go to **Manage** and then **Add Roles and Features**.
   
   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_14_39_18" src="https://github.com/user-attachments/assets/b047dc09-01b5-4b4e-93ed-7b23cb47fa6b" />

2. Proceed with installation until you reach **Select server roles** and select **Active Directory Certificate Services**, selecting **Add Features**.

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_14_51_17" src="https://github.com/user-attachments/assets/7e5073c1-fb9f-4dab-886d-bf4697c95aaf" />

3. Proceed with installation and then **Install**

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_14_54_11" src="https://github.com/user-attachments/assets/070192ad-edd2-4aaa-9372-77c07f826ef4" />

4. Select **Promote this server to a domain controller**

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_15_04_39" src="https://github.com/user-attachments/assets/5af88abe-ebfe-43fc-8cfb-83ce2ea82697" />

5. Select **Add a new forest** and enter your domain name, consisting of a second-level domain (localserver) and an extension (.com, .org. etc.).
  
   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_15_09_35" src="https://github.com/user-attachments/assets/752dd291-f965-4baf-b080-57aa58e7e047" />

6. Leave **Forest functional level** set to **Windows Server 2016** and enter in your password.

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_15_13_39" src="https://github.com/user-attachments/assets/484e19fd-555c-43ba-87b6-117a9db6209d" />

7. Proceed with installation.
   
8. After your computer restarts, the process should be complete.





