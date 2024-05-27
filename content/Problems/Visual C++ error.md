---
share: "true"
modified: 2024-04-27T16:11:29-07:00
---

# PROBLEM

The feature you are trying to use is on a network resource that is unavailable.  
![](attachments/vc1.png)

# ANSWER

https://answers.microsoft.com/en-us/windows/forum/all/cannot-install-microsoft-visual-c-2015-2022/b7eeba00-cae6-4900-87f4-fc404aae3961?page=2  
![](attachments/vc2.png)
1. Open regedit
2. Go to `Computer\HKEY_CLASSES_ROOT\Installer\Products`
3. Press `Ctrl+F` and search `Visual C`
4. Delete all folders that contain that keyword
5. Try installing again (Probably don't need to reboot)
