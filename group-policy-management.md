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
Now that we've covered the basics, we can apply some simple GPOs to our users.

In our newly created group, **Workers**, we can apply GPOs to multiple users within the group at once.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_12_08_2026_19_58_09" src="https://github.com/user-attachments/assets/1ec65b67-9186-41a5-91ec-944f4361edc0" />

We can apply a new GPO to the OU in **Group Policy Management**

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_12_08_2026_20_00_25" src="https://github.com/user-attachments/assets/46a4f8bd-8cfe-4ae8-b247-01c5dd4aac99" />

Right-click on the GPO and select **Edit**, where you will configure a new policy to increase the minimum password length and enable account lockout after 3 failed attempts. Go to **Windows Settings** under **Computer Configuration**, and drop down to **Account Policies**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_12_08_2026_20_05_39" src="https://github.com/user-attachments/assets/3575250e-8939-4c61-9903-571663ce63eb" />

In **Password Policy**, select **Minimum password length** and define it to more characters than the users' current passwords.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_12_08_2026_20_08_13" src="https://github.com/user-attachments/assets/529b8e71-0ebe-49f9-99f9-c2fcab584116" />

In **Account Lockout Policy**, select **Account lockout threshold Properties** and define it to 3 invalid logon attempts.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_12_08_2026_20_10_38" src="https://github.com/user-attachments/assets/e1dc385b-2054-49ab-9187-d248f0d33e68" />

In **Group Policy Management**, right click on the policy and ensure it is **Enforced**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_12_08_2026_20_12_43" src="https://github.com/user-attachments/assets/fcdbed7e-b836-4a8d-82c5-2f5f3a08f130" />











