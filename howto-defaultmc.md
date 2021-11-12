# Running Modpacks with the Vanilla Minecraft Launcher

## Steps
* [Installing the modpack](#installing-the-modpack)
* [Preparing the Vanilla Launcher](#preparing-the-vanilla-launcher)
* [Setting up an Instance](#setting-up-an-instance)

## Installing the modpack

To do this you will need a launcher to download the modpack for you. This is because the modpack .zip files from curseforge do not actually contain the mods, only links to the mods so that a launcher can download them. The vanilla launcher is not currently capable of this. Launchers you should use are [GDLauncher](http://gdevs.io), [MultiMC](https://multimc.org/), and [Curseforge](https://download.curseforge.com/) (although curseforge is known to incorrectly download modpacks on occasion). 

After getting your launcher, you will need to install the pack as per the launcher's instructions. 

## Preparing the Vanilla Launcher

Download and install the [Vanilla Launcher](https://www.minecraft.net/en-us/download) if you do not already have it installed. Install [Java 8](https://www.java.com/en/download/) as well if you do not already have it. To ensure you have installed java, open a terminal window (or command prompt for Windows) and run: 

    java -version

This should produce a response similar to what is shown below: 

![unknown](https://user-images.githubusercontent.com/80121423/141528372-a1743b53-b051-45e3-af05-6caad8684f60.png)

If you have other versions of java installed, this command may not show Java 8. 

## Setting up an Instance

To launch a Forge modpack with the vanilla launcher, you need to install the correct version of forge. You can locate this in the launcher you used to install the modpack. 

In GDLauncher, you can find it by rightclicking the modpack (once installed) and pressing "Manage". ![gdlauncher forge](https://user-images.githubusercontent.com/80121423/141530354-d8f40fb1-95e5-41c7-a1d8-db20e98c1dd2.png)

In MultiMC, you can find it by selecting the downloaded modpack and pressing "Edit instance". ![multimc forge](https://user-images.githubusercontent.com/80121423/141531655-431dcda1-9d1f-402e-bc79-04c9be25be11.png)

After determining the forge version you need, head over to the [forge website](https://files.minecraftforge.net/net/minecraftforge/forge/) select the correct version of Minecraft from the sidebar. Then scroll down and select "Show all Versions" and find the version you need. Pick the Universal installer and run it after downloading it. Install the client without changing any settings, and close it when it is finished. 
