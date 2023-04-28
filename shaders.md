# Installing Shaders with Optifine

## Steps

* [Get the shaders](#get-the-shaders)
* [Get Optifine](#get-optifine)
* [Setup](#setup)
* [Profit](#profit)

## Get the shaders

The first thing you will need to do is to find yourself a shader pack. A good place to find them is [Curseforge](https://www.curseforge.com/minecraft/search?page=1&pageSize=20&sortType=1&class=customization&search=Shaders) or [Modrinth](https://modrinth.com/shaders).
After you find the shaders you want to use, download it and save it somewhere (you will need it later).

## Get Optifine

To be able to utilize these shaders, you will need optifine. Please note optifine is known to cause several unexplainable problems in modded minecraft. You can get optifine from their [website](https://optifine.net/downloads) (you may need to press "show all versions"). A tool like [FastForward](https://github.com/FastForwardTeam/FastForward) can help skip through the ads instantly and not waste your time. Be sure you select the latest version of optifine for the version of minecraft you want to play.

NOTE: dont mess with that optiforge stuff its a fraud

## Setup

Open the launcher that you are using, and navigate to the instance, right click, and press open folder or instance folder (if you use multimc or any of its forks, you may need to navigate to the .minecraft folder).

![image](https://user-images.githubusercontent.com/80121423/235218805-92304deb-622b-45c0-9d0d-f2b0c632ea07.png)

Next, you will need to create a folder called `shaderpacks`. Place your shader zip that you downloaded in the first [step](#get-the-shaders) into this shaderpacks folder.

![image](https://user-images.githubusercontent.com/80121423/235218875-03aaf1af-8111-4dfb-8d29-fccd11364e74.png)

Next, place the optifine jar into the mods folder in your instance, ensuring that it is the right version for your instance of minecraft (for example, 1.19 optifine will not work with 1.12 minecraft)

![image](https://user-images.githubusercontent.com/80121423/235218992-788cfc30-c1d3-4051-baf8-30ce97dcf985.png)

Last, open up (or create) the `optionsshaders.txt` in your preferred text editor (it is located in the root folder of the instance). Scroll to the line labled `shaderPacks` and edit it so it becomes `shaderPacks:<pack>` where `<pack>` is the name of the zip that you placed into your `shaderpacks` folder earlier. It should end up looking like

    #Fri Apr 28 13:29:04 EDT 2023
    shaderPack:BSL_v8.2.03.zip
    antialiasingLevel=0
    normalMapEnabled=true
    specularMapEnabled=true
    renderResMul=1.0
    shadowResMul=1.0
    handDepthMul=0.125
    cloudShadow=false
    oldHandLight=default
    oldLighting=default
    tweakBlockDamage=false
    shadowClipFrustrum=true
    TexMinFilB=0
    TexMinFilN=0
    TexMinFilS=0
    TexMagFilB=0
    TexMagFilN=0
    TexMagFilS=0

## Profit

Launch the game and rejoice as you have fancier graphics :crab:

![image](https://user-images.githubusercontent.com/80121423/235218656-f35999a2-6dc2-4bb7-879b-6dac6b8791fd.png)

![image](https://user-images.githubusercontent.com/80121423/235219921-9893dd53-dbba-4772-83a0-5cf1988ea883.png)

 \- Mystic
