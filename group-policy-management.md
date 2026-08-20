# Group Policy Management
The objective is to provide a comprehensive overview of Group policy management and how it affects users and computers on the domain
## Active Directory Users and Computers
Go to **Tools** on the top right menu and select **Active Directory Users and Computers**. There you will find a series of **Organizational Units**, which are objects that organizes and controls groups of users and/or devices. They are created in order to apply selective policies and settings to only those within those units.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_15_45_00" src="https://github.com/user-attachments/assets/06e1250e-0205-4822-bade-32b7a9ed60e0" />

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_11_09" src="https://github.com/user-attachments/assets/bf46f348-74b1-47ab-a6b2-b8aacb7c2dda" />

## Creating Organizational Units
To create a new OU (Organizational Unit), right-click on **local-server.com**, select **New**, and select "Organization Unit".

 <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_13_14" src="https://github.com/user-attachments/assets/34ef1a4e-250c-48e4-a797-bcd2699ce539" />


You can create a new OU, provided that it doesn't already exists. Here you can add additional Users, Groups, and even other OUs within the OU.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_16_01" src="https://github.com/user-attachments/assets/3fd7debe-bc51-40dd-96c2-5f830ac773f2" />

## Creating Group Policy Objects
You can create Group Policy Objects (GPO) to apply either generally to the whole server or to specific OUs.

Go to **Group Policy Management** under **Tools** and right click on any OU you have created. Select **Create a GPO in this domain, and Link it here**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_32_25" src="https://github.com/user-attachments/assets/31098384-ee4a-4c1a-8ad8-28224981b6ae" />

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_33_54" src="https://github.com/user-attachments/assets/4dcceb18-9086-4a66-8902-22d510b7d2a5" />

Once the GPO is created, you can edit by right-clicking it and selecting **Edit**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_39_00" src="https://github.com/user-attachments/assets/c70a0cd0-e39f-4ee6-91b2-d650e3f1dc51" />

Here you customize the GPO, deciding whether you want it configured only to users or computers, and whether it's a policy (can't be changed) or preference (can be customized by the user).

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_06_08_2026_16_43_35" src="https://github.com/user-attachments/assets/fdfe5ee4-723f-4552-8282-dacf5763a0f1" />

## Applying Group Policy
Now that we've covered the basics, we can apply some simple GPOs to a sample OU.

In **Sample OU**, create a new GPO named **Wallpaper**, since we're going to change the wallpaper for the users in this OU. Select **Edit** to make the changes.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_20_08_2026_19_31_54" src="https://github.com/user-attachments/assets/febc8ae1-1b63-403f-8e30-fe21394d63f6" />

Select **Desktop Wallpaper** and select **Enabled**. Using a UNC path to paste the image file's location, copy and paste the address from the sharing tab of the file's folder location and add the image file's name at the end, i.e. **beach.jpg**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_20_08_2026_19_41_38" src="https://github.com/user-attachments/assets/e8760aed-8b49-4d5b-81e8-6fddaa21e5b0" />

After enforcing the policy, make sure that the folder containing the file is shared with the users.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_20_08_2026_19_45_04" src="https://github.com/user-attachments/assets/bfe54cc8-9d1e-4977-9694-da9c12d54365" />

After this, the desktop wallpaper should be changed **ONLY** for the users within the applied OU.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_20_08_2026_19_49_35" src="https://github.com/user-attachments/assets/bdb17fbc-9304-47e1-b1ec-0acabd962df5" />


















