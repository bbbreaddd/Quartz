---
modified: 2024-05-27T07:12:15-07:00
share: "true"
---
**Steps:**

# 1. DISABLE HIBERNATION

At a an elevated (admin) command prompt, run the command

powercfg /h off

# 2. DISABLE PAGEFILE

Open the System page in Control Panel (from “This PC”/“My computer”, open the Properties). Click “Advanced System Settings”, then in the “System Properties” dialog's “Advanced” tab, open the “Performance” settings, go to the “Advanced” tab, click “Change…” under “Virtual memory”, untick “Automatically manage paging file size for all drives”, select the drive you want to shrink, select “No paging file” and click the “Set” button.

# 3. DISABLE SYSTEM PROTECTION

In the “System Properties” dialog as above, go to the “System Protection” tab, click “Configure…” and select “Disable system protection”.

Restart.

Now the three files that were preventing partition reduction are gone. Reduce partition size, and then restore the three items.

If Disk Management complains that “There is not enough space available on the disk(s) to complete this operation.” even though you entered a size that should work according to Disk Management's own figures, see Cannot shrink C: partition: Not enough space

I have later found similar instructions at other places, all of them mentioning only these 3 items.

Try to shrink the volume again. If it still is unreasonably large, you will then have to look at Event Viewer to find which file is at the boundary. 1Right click on Computer => Manage => Event Viewer => Windows Logs => Application. 2Click on Filter Current Log, and put ’259′ for the Event ID 3Click on the latest event and look through the detail to find the problematic file. You can then attempt to delete that file (or set of files) manually. You may have to restart into safe mode to delete some files