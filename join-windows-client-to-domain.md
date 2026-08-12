# Join Windows Client to Domain
The objective is to join a windows client to connect to the server domain by configuring the network to be able to connect to the server machine.

## Setting up Server Network
1. On the server machine, select **Devices** in the top menu, select **Network**, and select **Network settings**.

  <img width="1023" height="854" alt="Screenshot 2026-08-07 154145" src="https://github.com/user-attachments/assets/1993d604-a7fc-4e1d-9708-254640a076d7" />

   
2. In **Adapter 1**, set **Attached to** to **Host-only Adapter**.

   <img width="1021" height="850" alt="Screenshot 2026-08-07 154444" src="https://github.com/user-attachments/assets/e37d45b7-f37d-40c4-aa1a-7e9d8dde79c2" />

3. Go to **Control Panel** and select **Network and Internet**.
  
   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_47_11" src="https://github.com/user-attachments/assets/6231c1ab-d604-4755-919a-f1c5b2e6ecdf" />

4. Under **Network and Sharing Center**, select **View network status and tasks**, and go to **Change adapter settings**.
  
   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_49_35" src="https://github.com/user-attachments/assets/1e2e72f4-9a8b-40cb-a9ee-a8693d79be92" />

5. Right-click on **Ethernet** and go to **Properties**.
  
   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_50_20" src="https://github.com/user-attachments/assets/0ffa9a30-af7e-4cf2-92c4-75db7f6facac" />

6. Select **Internet Protocol Version 4 (TCP/IPv4)** and select **Properties**.

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_52_50" src="https://github.com/user-attachments/assets/4eccdf9b-efb8-4cd5-a4fd-352c5867052a" />

7. Switch the configuration to **Use the following IP address** and **Use the following DNS server addresses** in order for the server machine to be easily located in the network. Your IP Address will vary based on your address that is shown in the **ipconfig** command in **Command Prompt**

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_16_16_22" src="https://github.com/user-attachments/assets/122b915a-c14a-45a3-a4d3-eebfb75986c4" />

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_16_01_26" src="https://github.com/user-attachments/assets/6d00630b-fe7f-4e4f-a3ae-2682d394cd3c" />

## Join Windows Client to Domain
1. Repeat the process of setting up the network to connect, making sure to pick a different IP address that's within the same subnet mask.

 <img width="1024" height="768" alt="VirtualBox_Windows11Client_07_08_2026_16_29_22" src="https://github.com/user-attachments/assets/61edefbd-7eb6-43cd-9fec-0f225961057a" />

2. To make sure that the client is discoverable by the server, ping the server name in **Command Prompt**.

   <img width="1024" height="768" alt="VirtualBox_Windows11Client_12_08_2026_19_28_34" src="https://github.com/user-attachments/assets/f4dcedde-bd2f-432a-804f-731783b5eadd" />

3. Go to **File Explorer**, right-click **This PC** and go to **Properties**.

   <img width="1024" height="768" alt="VirtualBox_Windows11Client_12_08_2026_19_37_58" src="https://github.com/user-attachments/assets/a06ed569-7d68-409a-a330-48785fa360b3" />

4. In **System > About**, scroll down to **Domain or workgroup**, select it and select **Change**.

   <img width="1024" height="768" alt="VirtualBox_Windows11Client_12_08_2026_19_41_46" src="https://github.com/user-attachments/assets/c04d6122-c7a5-4266-83b9-b62dc8b51983" />

5. Under **Domain**, place the domain name in the text box, select **OK**, and put in the administrator username and password.

   <img width="1024" height="768" alt="VirtualBox_Windows11Client_12_08_2026_19_44_02" src="https://github.com/user-attachments/assets/d592c42a-6de8-4996-a5c3-31acf1c52c9f" />

6. After your machine restarts, the machine will be connected to the domain.

     <img width="1024" height="768" alt="VirtualBox_Windows11Client_12_08_2026_19_44_27" src="https://github.com/user-attachments/assets/49069423-a43f-4445-a73b-54c02d2c205c" />





  






