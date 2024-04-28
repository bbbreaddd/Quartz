---
share: "true"
modified: 2024-04-27T16:12:06-07:00
---

# **REQUIREMENTS:**

- **USB Drive, 500MB or more (Everything on it will be erased)**
- **2 Drives**

**In this tutorial, I will be cloning a 20GB drive to a 30GB drive**

---

# **1. SETTING UP THE USB DRIVE**

---

**a. Download the latest [Rufus release here](https://rufus.ie/en/)**

**[https://rufus.ie/en/](https://rufus.ie/en/)**

![[attachments/image.png|attachments/image.png]]

Save it anywhere **except the USB drive**

![[attachments/D2Ximage.png|attachments/D2Ximage.png]]

**b. Download the latest [Clonezilla release here](https://clonezilla.org/downloads/download.php?branch=stable)**

Change file type to **ISO** and press **Download**

![[attachments/5CNimage.png|attachments/5CNimage.png]]

Once it's done downloading, it should look like this

![[attachments/izpimage.png|attachments/izpimage.png]]

**c. Open Rufus**

Press **No** if it asks to check for updates

![[attachments/ZzIimage.png|attachments/ZzIimage.png]]

You should see this menu

![[attachments/To3image.png|attachments/To3image.png]]

Press the blue **SELECT** button on the right and select the Clonezilla ISO that you downloaded

![[attachments/n1eimage.png|attachments/n1eimage.png]]

Rufus should now look like this, it may be different but it doesn't matter. Just use the defaults.

![[attachments/ibHimage.png|attachments/ibHimage.png]]

Press the blue **START** button on the bottom

> [!NOTE]  
> If it says **ISOHybrid image detected**, just press the blue **OK** button

![[attachments/K22image.png|attachments/K22image.png]]

> [!NOTE]  
> If it says **Download required**, press the blue **Yes** button

![[attachments/1nuimage.png|attachments/1nuimage.png]]

Rufus will tell you everything on the USB drive will be deleted, press the blue **OK** button

> [!WARNING]  
> **Make sure there is nothing important on the USB drive**

![[attachments/Gtdimage.png|attachments/Gtdimage.png]]

Now wait until Rufus is finished, it took me 2 minutes and 30 seconds so it shouldn't take long

When it is done, it will say **READY** and now you have Clonezilla on your USB drive

![[attachments/zG4image.png|attachments/zG4image.png]]

---

# **2. BOOTING CLONEZILLA**

**Finding your Boot Menu**

You have to find your boot menu or change the boot priority to do this.

This part varies greatly since there are many different BIOS and yours will most likely look different than others

You can ask me for help in Discord, click [here](https://discord.com/users/451884726618423351) for my profile

One way you can find the Boot Menu is by looking at the startup screen of your PC

You may see some text that says **Press F11 for Boot Menu**

![[attachments/z3mimage.png|attachments/z3mimage.png]]  
Another way of finding the Boot Menu is in the BIOS

There is usually a key to access the BIOS, most of the time it is **F2** or **Del**

To access the BIOS, turn off your computer. Turn it on and repeatedly press the **F2** or **Del** key (or both if you want to) until a menu shows up.

Once you find it, your Boot Menu should look similar to this

![[attachments/3zfimage.png|attachments/3zfimage.png]]

Look for your USB drive and press **Enter** to boot to it

# **3. USING CLONEZILLA**

When you boot to Clonezilla, you will see this

Press **Enter** or wait 30 seconds for it to automatically boot

![[attachments/Bnlimage.png|attachments/Bnlimage.png]]

Choose your language

![[attachments/yOTimage.png|attachments/yOTimage.png]]

Press **Keep**

![[attachments/kxQimage.png|attachments/kxQimage.png]]

Press **Start Clonezilla**

![[attachments/Bc2image.png|attachments/Bc2image.png]]

Choose **device-device**

![[attachments/4DLimage.png|attachments/4DLimage.png]]

Press **Beginner**

![[attachments/8Eximage.png|attachments/8Eximage.png]]

Press **disk\_to\_local\_disk**

![[attachments/GSsimage.png|attachments/GSsimage.png]]

> [!WARNING]  
> **This is very important, make sure you follow these steps closely as you can clone the wrong drive and lose data**

In this example, I am cloning a 20GB drive to a 30GB drive

First, you will choose the drive you are trying to clone which is the 20GB drive for me

![[attachments/x7Wimage.png|attachments/x7Wimage.png]]

Next, you will choose the drive that you want to clone to which is the 30GB drive for me

![[attachments/N6uimage.png|attachments/N6uimage.png]]

Press the **first** option (**-sfsck**)

![[attachments/tVnimage.png|attachments/tVnimage.png]]

Press **-k0**

![[attachments/CILimage.png|attachments/CILimage.png]]

Now you can choose to either reboot or shutdown when finished.

I'm going to choose shutdown

![[attachments/UIwimage.png|attachments/UIwimage.png]]

It will give you a message, just press **Enter**

![[attachments/ga8image.png|attachments/ga8image.png]]

It will warn you that the disk listed will be deleted

> [!WARNING]  
> **Make sure it is the right disk (the disk you are cloning to)**

Type **Y** and press **Enter** to continue

![[attachments/j9iimage.png|attachments/j9iimage.png]]  
It will tell you are you sure, just type **Y** again and press **Enter**

Now it is actually cloning the drive and will look like this, wait until it's done.

![[attachments/RCOimage.png|attachments/RCOimage.png]]

It may say this when it is finished, just press **Enter**

![[attachments/07yimage.png|attachments/07yimage.png]]
