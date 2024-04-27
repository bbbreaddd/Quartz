# PROBLEM

![[attachments/123.png|500]]

# SOLUTION

## MAIN FIX

Just reinstall your GPU drivers

> [!NOTE]  
> Haven't tested in a while, may not work anymore. I also haven't had this issue in a while so not sure if it matters anymore.

## FIX 1

https://www.windowscentral.com/how-disable-automatic-driver-updates-windows-10
1. Use the **Windows key + R** keyboard shortcut to open the **Run** command.
2. Type **gpedit.msc** and click **OK** to open the **Local Group Policy Editor**.
3. Browse the following path:`Computer Configuration > Administrative Templates > Windows Components > Windows Update > Manage updates offered from Windows Update`
4. On the right side, double-click the **Do not include drivers with Windows Update** policy.
5. Enable it  
![[attachments/12.png|1000]]
6. Click **Apply**. 
7. Click **OK**.

## FIX 2

1. Use the **Windows key + R** keyboard shortcut to open the **Run** command.
2. Type **regedit**, and click **OK** to open the **Registry**.
3. Browse the following path:`HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows`**Quick Tip:** On Windows 10, you can now copy and paste the path in the Registry's address bar to quickly jump to the key destination.
4. Right-click the **Windows** (folder) key, select **New**, and click on **Key**.

![[attachments/17.png|1000]]

5. Name the key **WindowsUpdate** and press **Enter**.
6. Right-click the newly created key, select **New**, and click on **DWORD (32-bit) Value**.

![[attachments/122.png|1000]]

7. Name the key **ExcludeWUDriversInQualityUpdate** and press **Enter**.
8. Double-click the newly created DWORD and set the value from **0** to **1**.

![[attachments/18.png|1000]]

9. Click **OK**.