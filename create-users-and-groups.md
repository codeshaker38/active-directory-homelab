# Creating Users and Groups
The objective is to demonstrate how users and groups can be created within Active Directory, as well as demonstrate how to configure their accounts to set various permissions.

In the top right menu, select **Tools** and select **Active Directory Users and Computers**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_15_45_00" src="https://github.com/user-attachments/assets/7ca92963-e5ef-4233-9df2-6e1e961a03f7" />

Right click on any group or OU and select **New** and then **User**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_08_31" src="https://github.com/user-attachments/assets/a63c794d-2e5e-4a99-b38d-0b79b6526a4c" />

Enter in the user's credentials and create their logon name, where they will be part of the server.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_10_43" src="https://github.com/user-attachments/assets/814c426e-aac8-4885-83d3-02f35b69a18b" />

Create a password for the user.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_14_51" src="https://github.com/user-attachments/assets/60c432c0-21f8-47ff-be74-874f356149bc" />

Once the process is complete, we can now start to create our group.

Once again, right-click on any group or OU and select **New** and then **Group**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_08_31" src="https://github.com/user-attachments/assets/ff155b24-ed05-4235-b977-9526870029e0" />

Enter in the group name, set the **Group scope** (let's do Global) and set the **Group type** (let's do **Security**)

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_20_10" src="https://github.com/user-attachments/assets/2c436e6e-f0f6-41bc-95dd-b063d4461330" />

Once the group is made, you can configure it to allow users to join it, as well as control what folders and files they have permission to access. Right-click on the group and select **Properties**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_21_36" src="https://github.com/user-attachments/assets/7d75122b-1c41-4477-87e2-8a0901ba6500" />

In properties, select **Members** and select **Add**, where you can enter in the name of an object (users, computers and others, you can also set the scope of object types in **Object Types**) and, provided that the object exists, they will be added to the group.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_07_08_2026_15_25_18" src="https://github.com/user-attachments/assets/2a9d5361-11c5-41e2-8ad1-baca1b94b19d" />
