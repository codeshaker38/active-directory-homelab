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

In **Group Policy Objects**, right-click **Default Domain Policy** and select **Edit**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_14_21_41" src="https://github.com/user-attachments/assets/bf1882c9-e289-4a80-bb7a-fc62d8dedf42" />

Here you will configure a new policy to increase the minimum password length and enable account lockout after 3 failed attempts. Go to **Windows Settings** under **Computer Configuration** and drop down to **Account Policies**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_14_34_16" src="https://github.com/user-attachments/assets/dcb8b226-8d28-4130-bc4d-f5e053505793" />

In **Password Policy**, Right-click **Minimum password length** and select **Properties**, and define it to more characters than the users' current passwords.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_14_36_08" src="https://github.com/user-attachments/assets/3c01a184-05aa-4b07-8e7e-d8511d52b01d" />

In **Account Lockout Policy**, select **Account lockout threshold Properties** and define it to 3 invalid logon attempts.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_14_37_55" src="https://github.com/user-attachments/assets/ec022eef-76d8-4498-8921-cd1de216900b" />

Right-click **Default Domain Policy** and select **Enforced**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_14_41_56" src="https://github.com/user-attachments/assets/7acb5e1d-789a-473d-a68c-35d128f590e3" />

Now that our Group policy is enforced, we can test it out with our users on our client device.

If we try to log in as Kyle, after three failed attempts, it will show that our account is locked.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_16_08_2026_14_49_42" src="https://github.com/user-attachments/assets/90273b5e-d782-4317-8102-27c30d722f7e" />

To unlock his account, we can go to his account, select **Properties** and go to **Account**, and select **Unlock account**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_16_08_2026_14_56_22" src="https://github.com/user-attachments/assets/7e12ccb6-9220-4ddd-afed-8f46766af2c1" />















