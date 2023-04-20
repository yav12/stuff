# Running Modpacks with the Vanilla Minecraft Launcher

## Steps

* [Installing a modpack](#installing-a-modpack)
* [Preparing the Vanilla Launcher](#preparing-the-vanilla-launcher)
* [Installing Forge](#installing-forge)
* [Making an Instance](#making-an-instance)
* [Launch :crab:](#launch-crab)

## Installing a modpack

To do this you will need a launcher to download the modpack for you. This is because the modpack .zip files from curseforge do not actually contain the mods, only links to the mods so that a launcher can download them. The vanilla launcher is not currently capable of this. Launchers you can use are [GDLauncher](http://gdevs.io), [MultiMC](https://multimc.org/) (although MultiMC is not currently capable of installing modpacks [due to API changes](https://github.com/MultiMC/Launcher/commit/0a827ba70e6ef20187f8507a536d54a8441020dc)), and [Curseforge](https://download.curseforge.com/).

After getting your launcher, you will need to install the pack as per the launcher's instructions. If you are using curseforge and dont know how to install modpacks, see below. If you already know how, skip down to [the next section](#preparing-the-vanilla-launcher). 

To install a modpack with curseforge, head over to their [website](https://download.curseforge.com/) website and download/install Curseforge for your platform. After it has been installed, open it up and select the top bar. You can search for modpacks here, or if you dont know what you want to play, you can browse for them. Once you find the one you are looking for, hit install and wait for it to complete the download. 
![curseforge layout](https://user-images.githubusercontent.com/80121423/169679046-4a401464-a098-46ce-9390-f6bb0f23ce7b.png)

## Preparing the Vanilla Launcher

Download and install the [Vanilla Launcher](https://www.minecraft.net/en-us/download) if you do not already have it installed. Install [Java 8](https://www.java.com/en/download/) as well if you do not already have it. To ensure you have installed java, open a terminal window (or command prompt for Windows) and run: 

    java -version

This should produce a response similar to what is shown below: 

![java version cmd](https://user-images.githubusercontent.com/80121423/141528372-a1743b53-b051-45e3-af05-6caad8684f60.png)

If you have other versions of java installed, this command may not show Java 8. 

## Installing forge

To launch a Forge modpack with the vanilla launcher, you need to install the correct version of forge. You can locate this in the launcher you used to install the modpack. **Make sure the vanilla launcher is not open at this step**

In Curseforge, you can find it by selecting the modpack you downloaded (click the modpack's picture). ![curse...forge???](https://user-images.githubusercontent.com/80121423/169678668-f05cc777-e00d-4aaa-9fac-3525d3f014b1.png)

In GDLauncher, you can find it by rightclicking the modpack (once installed) and pressing "Manage". ![gdlauncher forge](https://user-images.githubusercontent.com/80121423/141530354-d8f40fb1-95e5-41c7-a1d8-db20e98c1dd2.png)

In MultiMC, you can find it by selecting the downloaded modpack and pressing "Edit instance". ![multimc forge](https://user-images.githubusercontent.com/80121423/141531655-431dcda1-9d1f-402e-bc79-04c9be25be11.png)

After determining the forge version you need, head over to the [forge website](https://files.minecraftforge.net/net/minecraftforge/forge/) select the correct version of Minecraft from the sidebar. Then scroll down and select "Show all Versions" and find the version you need. Pick the Universal installer and run it after downloading it. Install the client without changing any settings, and close it when it is finished. 

## Making an Instance

To launch the modpack, you now need to create an instance for it in the Vanilla Launcher. Open the Vanilla launcher and go to "Installations", then select "New installation". ![defaultinstance](https://user-images.githubusercontent.com/80121423/169678653-db5b2ba1-24d3-4fa8-af64-4f6a96ee0e6c.png)

Give it a name, and an icon (or upload your own). Under `Version`, pick the correct forge version that you installed earlier. To find the game directory, open the launcher you used to install the pack and rightclick the modpack. Then select "Open Folder". In the window that appears, copy the file path and paste that into the Game directory box (you can also manually browse to the pack's folder if you know where it is, usually in your documents folder for curseforge users). 

Next, you need to configure the java settings. Select `More Options` and scroll down. In the java executable box, you need to enter the java path for the java you installed. For Windows, this is usually something along the lines of `C:\Program Files\Java\jre1.8.0_XXX\bin\javaw.exe`, where XXX is the java version. For macos, the path is something like `/Library/Java/JavaVirtualMachines/jdk1.8.0_XXX.jdk/Contents/Home/java`. For many linux distros, the java paths is something like `/usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java`, however this can vary greatly. Doing this will make Minecraft use a modern java version instead of the ancient one bundled with it (which may cause problems). If you are usinng windows, ensure you have the `javaw.exe` listed and not `java.exe`, as that will cause the game to crash on startup, or start without a window (really bad). Also note that the required version of java is different if you are playing 1.17+ versions of minecraft, and the path may differ slightly. 

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
