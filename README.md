# Server-Hosting
Learn how to safely host your own Minecraft server with or without paper, quilt, neoforge, forge, bukkit and spigot mods on any operating system for your mates or for, anyone really. Learn how to keep yourself safe, and your IP and location hidden whilst your at it.

Why do it yourself and not just pay for a server hoster?
Well, for one this is free, but two, you have no restrictions, this way is highly customisable meaning you can invite as many players as you like or put whatever mods you want on your server. All of this ran on your own spare computer, or if you don't have a spare computer, on your main computer.

Forge, on macOS:
1. Figure out which version you will be using. In order to run mods on a server with your mates. Your computer, your friends computer, the server, the modloader (ie forge) and all the mods donwloaded need to have the same version. For example, if I have a 1.20.1 mod, ! will need to download the 1.20.1 version of forge.

2. Download the file, the 1.21 and 1.12.2 files are linked above, however if you want a direct download link or want a different version: visit the following link. 'https://files.minecraftforge.net/net/minecraftforge/forge/'. Select which version you want on the selection bar on the left and use the download button in the middle. You can either use the recommended or latest version. It doesn't matter.

3. Now that you have forge, before you run it, you will need to install java. Visit the following link: 'https://www.oracle.com/java/technologies/javase/jdk22-archive-downloads.html' and scroll down until you find the macOS Arm and macOS x64 DMG download links. Download the Arm version with the link across the right of the page if your laptop has a M1,M2,M3 or later chipset in. Otherwise use x64 for intel macs. Make sure you download the DMG files otherwise you will not be able to install the file once you have it. If you are unsure if your macbook has a apple silicon chip (M1 etc) or an intel chip, you can click the apple icon at the top left of your screen and click 'about this mac'. It will say which chipset you have.

4. Once downloaded, install Java and follow the instructions on the setup.

5. You are now ready to install forge on your system with the first file you downloaded. Run the file, a box asking if you want to install forge for your client or server should pop up. Just ignore the other options as you won't need them for this. In order for a modded server with forge to work, the server and all the players must have forge and the mods installed on their own computers. If you didnt know, the client is your computer and the server is the computer your running the server off of. In order to install forge for the client, you will need to have minecraft installed. Note you won't need to have curseforge installed. Select the client and install forge if you havn't already, you don't need to worry about the directory at the bottom of the window, it should be set correctly automatically. If it isn't, navigate to (/Users/'your username'/Library/Application Support/minecraft) and install it there. Make sure your minecraft and launcher are closed whilst you do this otherwise it might not work. You can also improve your performance by installing optifine, however we'll cover that at the end.

6. You'll now have to install forge on your server. The first thing you need to do is create a folder, you can create the folder anywhere, in your documents folder or in your downloads folder. It doesn't matter. You can name the folder whatever you like. Now follow the same steps as you did to install forge for the client except select 'Install Server' instead. You'll notice an error at the bottom of the window, to fix this change the directory to the directory of the folder and click install. If you get an error, run it again or make another folder. If these dont work, copy the error code and google it. When it is successful you should get a message pop up.

7. Once installed, open the folder you created to begin with, if you installed forge for 1.16.5 or earlier, you will have three files in your folder. A forge jar file, a minecraft jar file and a libaries file. However if you downloaded forge for 1.17 or later then you will have a run.bat file, run.sh file, user_jvm_args.txt and a libaries folder.

For 1.17 and above:
1. Open terminal, and go to the directory of the run.bat file. For example, if my folder is located in my documents folder, then I type 'cd documents/minecraftserverfolder'. If your folder has a space in it's name you will need to use single quotation marks to inclose it. After this, write 'chmod a+x ./run.sh'. Finally enter,./run.sh to run the file.

Example:
1. cd documents/minecraftserverfolder
2. chmod a+x ./run.sh
3. ./run.sh

To add mods:
1. Find and download a mod you like (remember it has to have the version) and make sure it is a jar file. Put the jar file into the mods folder created when you ran forge. Don't forget to install the mod locally on your computer too. You can do this my going to /Library/Application Support/minecraft/mods. If there isnt already a 'mods' folder, make one. Don't use a capital 'm' for mods. Put the jar file for the mod in this folder too. Everytime you want to run your server, you'll need to either run the 'run.sh' file or type ./run.sh in the terminal. Be aware for this to work, you'll need to be in the directory. 

This should start the server.

For 1.16.5 and below:
1. Run the server.jar file.
2. Change the eula to true by opening the text file and removing false. Make sure you make the 't' lowercase and that there isn't a space between the equal sign and true.
3. Run the server.jar file again, your server should start up.

In order to use forge, run the forge jar file in the same folder. You'll notice this won't work. You will need to create a sh file.

1. Press command + space to use spotlight and type in 'textedit'.
2. Write the following,
("/Library/Java/JavaVirtualMachines/jdk-1.8.jdk/Contents/Home/bin/java" -server -Xmx6000M -Xms6000M -jar minecraft_server.1.12.2.jar nogui).
3. Press command + s to save the file. Then navigate to the menu bar - (the bar at the top of your screen) and click format, and then make plain text.
4. Drag this file into your server folder and make sure it is an SH file. If you don't know how to do this, google or use the .sh file linked above.
5. In terminal, navigate to the folder (as shown in the 1.17 and up steps) and enter 'chmod a+x ./run.sh' and the './run.sh'.
6. This should run your server.

Please note that, the chmod command is only needed the first time as it allows the neccessary permissions, you might need to allow terminal full disk access, and older versions of minecraft such as 1.12.2 require older versions of java. So if the method isnt working, try installing Java 8 and 17 as well as the newest version.

To add mods:
1. Find the 'mods' folder in the folder you created and drop your mods in. Be sure you have the mods installed locally too. This can be done by creating a mods folder in the minecraft folder inside application support. You can find that inside of the library folder.

Joining:
Ngrok and perhaps noip
other wise portforwding link
sh file link

Using Optifine:


