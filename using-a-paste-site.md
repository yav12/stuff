# How to upload a Minecraft log

## Steps
* [Uh oh](#uh-oh)
* [Some notes about this guide](#some-notes-about-this-guide)
* [Crash report or log?](#crash-report-or-log)
* [Finding the log](#finding-the-log)
   * [PolyMC/MultiMC](#polymc-multimc)
   * [Everyone else](#everyone-else)
* [Uploading the log](#installing-forge)
   * [Paste.ee](#paste.ee)
   * [Paste.gg](#paste.gg)
   * [Hastebin](#hastebin)
* [Sharing the log](#sharing-the-log)

## Uh oh
![image](https://user-images.githubusercontent.com/80121423/188249502-a9f2e862-ade8-4ccf-ae03-6cfa4471464a.png)![image](https://user-images.githubusercontent.com/80121423/188249534-5a88d663-8b51-4c0c-b712-b0339bdebbe8.png)

If you are reading this, something is probably gone wrong. Minecraft for some reason has crashed on you and you dont know what to do. To be able to properly diagnose the problem, you need to have a look at a crash report or a log file. This guide is to help you get help by uploading that log so that you can share it with (hopefullly) more knowledgable people. 

## Some notes about this guide
I tried to include as many pictures as i could and for different operating systems. Some things may look little different, but you should hopefully be able to recognize what they are (mainly file explorer looking a little different). [Paste.ee](https://paste.ee/) is often flagged as a malicous website by antivirus browser extensions (most notably malwarebytes). This is not the case, but if it makes you uncomfortable, you can one of the other options. 

## Crash report or log?
Knowing the difference is the first step to getting help. Minecraft generates a crash report when it, well, crashes. In addition, like every well written program should, it has a continuous log file that records everything that happens in your client while it is open. It also gives a debug.log that provides advanced information for people who really know what they are doing. If the game has crashed, and you have been returned to the launcher, you will want a crash report to give to someone. On the other hand, if Minecraft got "stuck" and isnt responding for an extended period of time, a log will provide more assistance as minecraft did not crash (and most likely you will not be able to find a crash report). 

If you are unsure of which to take, take the log as it gives all the same information as the crash report and more. Only give the debug.log if someone instructs you to. 

## Finding the log
To upload a log, you need to be able to find it first. To do that, you have to get from your Minecraft launcher to the log file itself. 

### MultiMC/PolyMC
If you are using MultiMC or its fork, PolyMC, There is no need for you to locate the log file and upload it, the launcher does all this for you!
First open up MultiMC select the modpack you want to get a log for (single click not double click). Then click edit instance and then navigate to "Other Logs."

![image](https://user-images.githubusercontent.com/80121423/188250857-abd0c87e-53f2-41a2-aa65-08153ef88f1a.png)

From this menu, you can access all the logs that minecraft has produced for this instance. by clicking the dropdown (where my cursor is in the screenshot) you can select a log. Pick the one you want, and then press upload. A confirmation message will appear, and it will copy the link to your log to your clipboard. Skip down to [Sharing the log](#sharing-the-log) :>

### Everyone else

The first step is to open the main page of the minecraft modpacks page in the launcher you are using. You should see a list of installed modpacks where you can choose to play or modifiy a pack. (need an image for curseforge)

Right-click the image of the modpack you wish to get a log from, and select open folder (it might say open instance folder). 

![image](https://user-images.githubusercontent.com/80121423/188254388-7d9b07b6-4bdf-4dcd-8578-08faaefe48a3.png)
*GDLauncher*
<!picture of curseforge coming soon>
Clicking this will open file explorer, once it loads, navigate to the appropriate folder (the folder is crash-reports or logs, [depending on your needs](#crash-report-or-log)). Then open the log/report you want. Logs other than the latest.log will be saved as .gz archives and can be extracted using software like [7zip](https://www.7-zip.org/), [tar](https://man7.org/linux/man-pages/man1/tar.1.html), or [The Unarchiver](https://theunarchiver.com/), all of which I highly recommend. 


## Uploading the Log
To be able to share your log file, you need to put it somewhere on the internet where people can access it. Thats where paste sites come in. They offer a free place to place text for others to access for a limited time (or forever if you want). 
