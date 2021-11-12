# Running Modpacks with the Vanilla Minecraft Launcher

## Steps
* [Installing the modpack](#installing-the-modpack)
* [Preparing the Vanilla Launcher](#preparing-the-vanilla-launcher)
* [Installing Forge](#installing-forge)
* [Making an Instance](#making-an-instance)
* [Launch :crab:](#launch-crab)

## Installing the modpack

To do this you will need a launcher to download the modpack for you. This is because the modpack .zip files from curseforge do not actually contain the mods, only links to the mods so that a launcher can download them. The vanilla launcher is not currently capable of this. Launchers you should use are [GDLauncher](http://gdevs.io), [MultiMC](https://multimc.org/), and [Curseforge](https://download.curseforge.com/) (although curseforge is known to incorrectly download modpacks on occasion). 

After getting your launcher, you will need to install the pack as per the launcher's instructions. 

## Preparing the Vanilla Launcher

Download and install the [Vanilla Launcher](https://www.minecraft.net/en-us/download) if you do not already have it installed. Install [Java 8](https://www.java.com/en/download/) as well if you do not already have it. To ensure you have installed java, open a terminal window (or command prompt for Windows) and run: 

    java -version

This should produce a response similar to what is shown below: 

![unknown](https://user-images.githubusercontent.com/80121423/141528372-a1743b53-b051-45e3-af05-6caad8684f60.png)

If you have other versions of java installed, this command may not show Java 8. 

## Installing forge

To launch a Forge modpack with the vanilla launcher, you need to install the correct version of forge. You can locate this in the launcher you used to install the modpack. **Make sure the vanilla launcher is not open at this step**

In GDLauncher, you can find it by rightclicking the modpack (once installed) and pressing "Manage". ![gdlauncher forge](https://user-images.githubusercontent.com/80121423/141530354-d8f40fb1-95e5-41c7-a1d8-db20e98c1dd2.png)

In MultiMC, you can find it by selecting the downloaded modpack and pressing "Edit instance". ![multimc forge](https://user-images.githubusercontent.com/80121423/141531655-431dcda1-9d1f-402e-bc79-04c9be25be11.png)

After determining the forge version you need, head over to the [forge website](https://files.minecraftforge.net/net/minecraftforge/forge/) select the correct version of Minecraft from the sidebar. Then scroll down and select "Show all Versions" and find the version you need. Pick the Universal installer and run it after downloading it. Install the client without changing any settings, and close it when it is finished. 

## Making an Instance

To launch the modpack, you now need to create an instance for it in the Vanilla Launcher. Open the Vanilla launcher and go to "Installations", then select "New installation". Give it a name, and an icon (or upload your own). Under `Version`, pick the correct forge version that you installed earlier. To find the game directory, open the launcher you used to install the pack and rightclick the modpack. Then select "Open Folder". In the window that appears, copy the file path and paste that into the Game directory box (you can also manually browse to the pack's folder if you know where it is). 

Next, you need to configure the java settings. Select `More Options` and scroll down. In the java executable box, you need to enter the java path for the java you installed. For Windows, this is usually something along the lines of `C:\Program Files\Java\jre1.8.0_XXX\bin\javaw.exe`, where XXX is the java version. Doing this will make Minecraft use a modern java version instead of the ancient one bundled with it (which may cause problems). 

Finally, you need to enter java arguments. Delete everything there and insert 

    -XmxNG -XmsNG

where `N` is the ammount of memory you wish to allocate, in GB. You can also use 

    -XmxDm -XmsDm
    
where `D` is the ammount of memory you wish to allocate, in MB. After this, paste the recommended java arguments for the pack you are playing. For example, MC Eternal's recommended arguments are: 

    -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:MaxNewSize=2200m -XX:SurvivorRatio=2 -XX:InitialSurvivorRatio=1 -XX:NewRatio=3
    
So the JVM arguments box would contain this: 

    -XmxDm -XmsDm -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:MaxNewSize=2200m -XX:SurvivorRatio=2 -XX:InitialSurvivorRatio=1 -XX:NewRatio=3

Once you have finished here, hit "Create". 

## Launch :crab:

Go to the main menu (Play) and select the instance you just made (where it may say "Latest Release").

Then press play and rejoice :crab:


 \- Mystic
