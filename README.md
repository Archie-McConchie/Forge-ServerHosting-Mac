# Server-Hosting
Learn how to safely host your own forge Minecraft server with mods on mac for your mates or for, anyone really. Learn how to keep yourself safe, and your IP and location hidden whilst your at it.

Why do it yourself and not just pay for a server hoster?
Well, for one this is free, but two, you have no restrictions, this way is highly customisable meaning you can invite as many players as you like or put whatever mods you want on your server. All of this ran on your own spare computer, or if you don't have a spare computer, on your main computer.

Forge, on macOS:
1. Figure out which version you will be using. In order to run mods on a server with your mates. Your computer, your friends computer, the server, the modloader (ie forge) and all the mods donwloaded need to have the same version. For example, if I have a 1.20.1 mod, ! will need to download the 1.20.1 version of forge.

2. Download the file, the 1.21 and 1.12.2 files are linked above, however if you want a direct download link or want a different version: visit the following link. 'https://files.minecraftforge.net/net/minecraftforge/forge/'. Select which version you want on the selection bar on the left and use the download button in the middle. You can either use the recommended or latest version. It doesn't matter.

3. Now that you have forge, before you run it, you will need to install java. Visit the following link: 'https://www.oracle.com/java/technologies/javase/jdk22-archive-downloads.html' and scroll down until you find the macOS Arm and macOS x64 DMG download links. Download the Arm version with the link across the right of the page if your laptop has a M1,M2,M3 or later chipset in. Otherwise use x64 for intel macs. Make sure you download the DMG files otherwise you will not be able to install the file once you have it. If you are unsure if your macbook has a apple silicon chip (M1 etc) or an intel chip, you can click the apple icon at the top left of your screen and click 'about this mac'. It will say which chipset you have.

4. Once downloaded, install Java and follow the instructions on the setup.

5. You are now ready to install forge on your system with the first file you downloaded. Run the file, a box asking if you want to install forge for your client or server should pop up. Just ignore the other options as you won't need them for this. In order for a modded server with forge to work, the server and all the players must have forge and the mods installed on their own computers. If you didnt know, the client is your computer and the server is the computer your running the server off of. In order to install forge for the client, you will need to have minecraft installed. Note you won't need to have curseforge installed. Select the client and install forge if you havn't already, you don't need to worry about the directory at the bottom of the window, it should be set correctly automatically. If it isn't, navigate to (/Users/'your username'/Library/Application Support/minecraft) and install it there. Make sure your minecraft and launcher are closed whilst you do this otherwise it might not work. You can also improve your performance by installing optifine, however we'll cover that at the end.

1.17 and above, scroll down for older versions.

6. You'll now have to install forge on your server. The first thing you need to do is create a folder, you can create the folder anywhere, in your documents folder or in your downloads folder. It doesn't matter. You can name the folder whatever you like. Now follow the same steps as you did to install forge for the client except select 'Install Server' instead. You'll notice an error at the bottom of the window, to fix this change the directory to the directory of the folder and click install. If you get an error, run it again or make another folder. If these dont work, copy the error code and google it. When it is successful you should get a message pop up.

7. Once installed, open the folder you created to begin with, if you installed forge for 1.16.5 or earlier, you will have three files in your folder. A forge jar file, a minecraft jar file and a libaries file. However if you downloaded forge for 1.17 or later then you will have a run.bat file, run.sh file, user_jvm_args.txt and a libaries folder.

8. Open terminal, and go to the directory of the run.bat file. For example, if my folder is located in my documents folder, then I type 'cd documents/minecraftserverfolder'. If your folder has a space in it's name you will need to use single quotation marks to inclose it. After this, write 'chmod a+x ./run.sh'. Finally enter, './run.sh to run the file'.

Example:
1. cd documents/minecraftserverfolder
2. chmod a+x ./run.sh
3. ./run.sh

Your server should start running with the mods installed. Type 'stop' in the terminal to stop the server.

To add mods:
1. Find and download a mod you like (remember it has to have the version) and make sure it is a jar file. Put the jar file into the mods folder created when you ran forge. Don't forget to install the mod locally on your computer too. You can do this my going to /Library/Application Support/minecraft/mods. If there isnt already a 'mods' folder, make one. Don't use a capital 'm' for mods. Put the jar file for the mod in this folder too. Everytime you want to run your server, you'll need to either run the 'run.sh' file or type ./run.sh in the terminal. Be aware for this to work, you'll need to be in the directory. 

This should start the server, skip to the joining section of this article to see how you and your friends can join.

For 1.16.5 or older versions:

6. Google '1.16.5 minecraft server' and click on the first link. Scroll down and click on the 'minecraft server.jar' file and download it.
7. Make a new folder and call it whatever you want, but put it somewhere you can find it.
8. Drag the jar you just downloaded into the folder, rename it to server, and make a new text file called start. In the file, write the following:
 ("/Library/Java/JavaVirtualMachines/jdk-1.8.jdk/Contents/Home/bin/java" -Xmx8192M -Xms8192M -jar server.jar nogui)
9. The numbers represent how much ram you use, never use more than half your computers ram. 🐑 🐏 Xms is the minimum and Xmx is the maximum. M is for megabytes.
10. Note that the directory could be different so check.
11. Save the text file, and on the top menu bar, click format and then make plain text. Close the file.
12. Rename the file from a .txt to a .sh.
13. Run the sh file the same way you would for 1.17 (follow the instructions above).
14. Open the newly created EULA file and change false to true (assuming you agree with the eula).
15. Run the sh file again. The server should start. This is a vanilla server. Stop the server by typing stop in the console of the world or by closing terminal.
16. In order to make the server forge, reopen the forge installer jar file you previously donwloaded and run it.
17. Select 'Install Server' and change the directory to the folder you created. Then press install.
18. Once successful, open your folder and delete the first jar file you renamed. Then edit your sh file and change server.jar to the name of the new jar file. It should be something similar to minecraft_server1.12.2.jar.
19. Run the sh file in terminal by going to the directory of the folder, and typing chmod a+x ./start.sh and then ./start.sh. You will only have to write the chmod command the first time. Now, everytime you want to run your server, type that command: ./start.sh. (Scroll up for instructions on how to enter the directory in terminal).

To add mods, drop the jar files into the newly created mods folder in the server folder you created. Don't forget to install them locally.

Joining:
In order to join your minecraft server, you will need to be on the same wifi as the server and have the IP. This is highly impractical, and if you could join from somewhere else, people would have your ip address and then your location. So to prevent this you can use two services called Ngrok and NoIP. NoIP changes the ip address from some random numbers which no one can remember to a free memorable subdomain for example: 'myserver.ddns.net' The ddns.net part is compulsory unless you pay for a proper domain. Ngrok allows for your mates to connect when they aren't on the same wifi and it passes through servers in sydney meaning the IP address you give to people can't be tracked back to your location allowing you to safely host your server for anyone.

Setting up Ngrok.
1. Google Ngrok and sign up.
2. You will need to add your debit/credit card as identifcation for your account. It will not be charged. To do this go to settings and then account on the side bar.
3. If you know your IP adress, then great. However if you dont, go to settings, then wifi, then details (to the left of the wifi your connected to) and click on TCP/IP. You will see your ip address there.
4. Go back to the Ngrok dash board and follow the instructions on how to install the service and add your authtoken.
5. Next, go to terminal and the your folders diretory and type the following: ./ngrok tcp 'yourIP':25565. This should run NGROK.
6. At the bottom of the page you should see: Forwarding. Forwarding: tcp://0.tcp.au.ngrok.io:14132 -> 'yourIP':25565.
7. The '0.tcp.au.ngrok.io' and ':14132' parts are the important bits.
8. Use a domain to IP address converter to find the IP address of the domain.
https://domaintoipconverter.com
9. Put the port after the IP. For example: the IP could be 3.24.145.55. You would put 3.24.145.55:14132 and that would be your server IP. Anyone will be able to join your server with this. The port at the end will also change.
10. Keep in mind that the IP address: 3.24.145.55 changes and that you have to run Ngrok everytime you boot the server and leave it open. Just create a new window for terminal and run the server that way.

Using the NoIP service. 

Now that you have a working server and an IP, you might get tired of typing in long numbers. You can use NoIP to change the IP of the domain for example 3.24.145.55 to a subdomain for example 'myserver.ddns.net'. Which is much easier typed. Keep in mind you can only do this for the domain and will have to add the port after this IP address. For example 'myserver.ddns.net:14132'.

Using Optifine:
To install optifine, google and download the jar file. To run optifine without mods or forge, run the jar file and click install. If you want optifine with forge, drop the jar file into the mods file in the minecraft folder inside of application suppport. Keep in mind optifine is a client mod and you won't need it on the server. The optifine jar file for 1.20.1 is linked above.

