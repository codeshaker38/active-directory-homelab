# Network Sharing

Make sure to enable network sharing on for your users on your client device. To do this, Open **File Explorer**, select **Network**, and select **Turn on network discovery and file sharing**. You will have to put in your admin username and password to enable this.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_16_08_2026_15_28_03" src="https://github.com/user-attachments/assets/b618a742-a7c8-411c-8355-3a8cd98af20e" />

Going to back to the server machine, go to **File Explorer**, select **Local Disk (C:)** and create a new folder.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_15_05_03" src="https://github.com/user-attachments/assets/02abc077-8e11-4ccd-93ac-62f495ead5f3" />

Right-click on the folder and select **Properties**, where you can go to sharing and select **Advanced Sharing**. Here you can customize permissions on who has access to the folder.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_15_06_17" src="https://github.com/user-attachments/assets/756637cd-0c79-42be-8a71-cb8df9a35345" />

You can add and/or remove who you want access to the folder. Here, we can allow only Kyle to have access to the folder.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_15_50_19" src="https://github.com/user-attachments/assets/69bec5b1-d475-48b5-894f-be5582ef3382" />

If we log in to Kyle's account, we can see that he has access to the folder.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_16_08_2026_15_57_17" src="https://github.com/user-attachments/assets/71c7acd0-4492-40a2-bfe8-a755f7c227c0" />

Whereas Justin does not have access to the account.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_16_08_2026_15_59_35" src="https://github.com/user-attachments/assets/0c87fc71-b97e-4dc0-b5f7-65ae9f279b2e" />

## Mapping a Network Drive

Another way of sharing files is through mapped drives.

If we go back to Group Policy Management, we can further edit the Default Domain Policy to include a mapped drive. Selecting **Preferences** under **User Configurations**, we can access **Windows Settings**, where we can access **Drive Maps**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_16_01_49" src="https://github.com/user-attachments/assets/3250c4bd-7ae5-44f9-9b81-607982a56b46" />

Right-clicking **Drive Maps**, we can select **New**, then **Mapped Drive**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_16_02_17" src="https://github.com/user-attachments/assets/b3019586-8545-490d-81f5-a5321e808f57" />

You can assign a letter to the drive, paste in the path location of the folder (located in the **Sharing** tab) and give it a descriptor name that will be the name that appears when locating the drive.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_16_03_03" src="https://github.com/user-attachments/assets/03a93fa0-0b66-4d03-8dc8-f315619e63c7" />

Now that the drive is made, it will be accessible to those have permission to access it.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_16_08_2026_16_06_24" src="https://github.com/user-attachments/assets/20592542-c9d4-42d1-8477-a9197d2edf40" />






