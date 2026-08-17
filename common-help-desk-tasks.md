# Common Help Desk Tasks
## Changing Passwords
A common issue that users may face when trying to log into their accounts is that their password is expired, or that they simply do not remember it. In order to assign a new password, go to **Active Directory Users and Computers** and right-click on the user's icon. Selecting **Reset Password** will give us access to reset their password.

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_15_43_09" src="https://github.com/user-attachments/assets/6b2ab5b4-20ec-4bc7-b3bd-a6d2871b4df5" />

  Simply enter their new password and that should resolve the issue.
  
   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_15_46_50" src="https://github.com/user-attachments/assets/2d871a7a-ced0-4513-b883-11100f5b0385" />

## Restricting Logon Hours
Another common task is configuring the logon window for the user, which we can access by accessing the user's **Properties**, where we can access the **Account** tab and adjust their **Logon Hours**

   <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_15_53_04" src="https://github.com/user-attachments/assets/9cceeceb-65ff-4766-a552-bfba05142714" />

We now have specific control of the logon hours allowed for their account. For example, if we wanted to restrict their logon hours to everyday but Monday and Tuesday, we simply select all hours of Monday and Tuesday and select **Logon Denied** on the right hand side.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_15_54_56" src="https://github.com/user-attachments/assets/ee3271ea-57ce-4370-a22d-32ce9e4058a5" />

This should result in the user being unable to log into their account.

   <img width="1024" height="768" alt="VirtualBox_Windows11Client_17_08_2026_16_20_34" src="https://github.com/user-attachments/assets/d8a9e471-6439-40cd-a80e-be15dd4a9815" />

## Account Lockout
If a user, for whatever reason, gets locked out of their account, it's simply a matter of going to the user's **Properties** and selecting **Unlock Account**.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_16_28_02" src="https://github.com/user-attachments/assets/55079e38-db4a-4d8b-9b35-812e094aae19" />

## Unable to Access Folders and/or Files
Sometimes, if a user is unable to access a certain folder and/or file, it's usually the case that the user simply doesn't have the same permissions as those with access. 

To fix this, we can go to the folder in **File Explorer** and examine its advanced sharing permissions. 

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_16_40_18" src="https://github.com/user-attachments/assets/b27a3775-a328-4b76-afa2-7f1f387bb28e" />

Selecting **Add** will allow you to select the users who don't already have access, in addition to customizing their permissions.

  <img width="1024" height="768" alt="VirtualBox_WindowsServers2022_17_08_2026_16_43_17" src="https://github.com/user-attachments/assets/70350b1a-4207-4f93-8048-e92c503dcbdc" />

After this, the user should now by be able to access and modify the folder by adding in additional files.

  <img width="1024" height="768" alt="VirtualBox_Windows11Client_17_08_2026_16_49_15" src="https://github.com/user-attachments/assets/8c40c36d-18e3-40b6-8f07-668bf2add87b" />




