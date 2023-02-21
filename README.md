# Steam Deck Setup Guide


<!--Not final name-->

<p align="center">
  <img src="https://user-images.githubusercontent.com/34931118/213886812-fc65cc59-9b64-48a3-96de-eccd1374bf6e.png">
</p>


This is a guide containing a compilation of a multiple of steam deck tools that are all around useful, especially for a new setup.

<!--Section to explain what a Steam Deck is? Go over SD card/dock recommendations? -->

## Table of Contents
- Tips
- Easier File Transfers
- Emulation
- Remote Play
- Non-Steam Games
- Other Launchers
- Tools
- Accessories

# Tips
## Turn off adaptive brightness

<!--Kills the battery. Use QAM for brightness changes.-->

# Don't be afraid to use the built in limiter

In the QAM you get an option between locking it at 15 fps, 30 fps or 60 fps. You can also lock it to 40 fps but only after you change the refresh rate to 40 as well.

<!--40hz with 40 fps is better than FPS jumping between 40-60. It also looks surprisingly smooth and keeps the battery lasting longer. Use CPU/GPU limiter and you can save these settings per game. -->


# Easier File Transfers
## [AnyDesk](https://www.anydesk.com)![anydesk-logo-white-red-ec4e3a](https://user-images.githubusercontent.com/34931118/213895260-7b7d34e3-b0d5-48bf-ab91-46f71b318404.png)

AnyDesk is a remote desktop application  one of the best and easiest ways to navigate the Steam Deck while in Desktop mode. It's free and it'll share the mouse/keyboard and clipboard with your actual PC. The best part is it's multiplatform. It's available on Windows, macOS, Linux, Android, iOS, FreeBSD, Raspberry Pi and Chrome OS.  

## Enable SSH

Enabling SSH is useful for file transfering purposes via FTP applications such as WinSCP, etc <!--Look up other examples-->

## KDE Connect
As of software version 3.4.4 KDE was updated to support KDE Connect which allows you to -- <!--Look for examples--> The functionality is built into the OS. Just download KDE connect on the device you'd like to transfer files from. <!--Find supported OS's-->

# Emulation
## [EmuDeck](https://www.emudeck.com)![logo](https://user-images.githubusercontent.com/34931118/213895041-d8c051e5-850f-4c43-93b7-0f630c37cdd7.png)

An all-in-one emulation installer. It'll set-up the file structure needed for every emulator so you can just start and go.

### Install Guide
1. If using an SD card format it if you haven't done so yet. 

``` NOTE: This WILL delete any existing data on your SD Card. ``` 
>To format an SD Card go to Settings > System > Format SD Card. It will format it correctly for you. 
2. Go into Desktop mode by pressing the STEAM button > Power > Switch to Desktop.
3. Open up your browser of choice and go to https://www.emudeck.com/#download and download the EmuDeck installer.
4.  

Note: 

<!--Remember to add the emulators that you need to manually install via the Discover store.-->


## [RetroDECK](https://retrodeck.net)![logo_unstacked](https://user-images.githubusercontent.com/34931118/213895119-bd5b9501-2a11-4af7-8f92-6f735eceb80f.png)

Another all-in-one emulator except this one uses the front-end of EmulationStation. 
<!--Look up differences between this and Emudeck.-->

Note: 



# Remote Play
<!--Think about adding performance of each? Or keep this install centered only? -->

## [Chiaki4deck](https://github.com/streetpea/chiaki4deck)![chiaki_wide](https://user-images.githubusercontent.com/34931118/213895158-7a678b9f-a117-44ed-8496-d915b54e5550.png)

<!-- describe the process for installing and how to set it up. -->

A PS4/PS5 remote play app. 
<!-- Include screenshots of deck. Find out how to "put screenshot in photo of deck"-->

## [Moonlight](https://moonlight-stream.org)
<!-- describe how to install and set up. -->
Moonlight utilizes Gamesteam  to trick your PC into thinking the streaming device is a Nvidia Shield so you can stream any of your games. You can also use this as a Remote Desktop application by adding mstsc.exe to the Shield tab in Geforce Experience. 

<!--Should I do a nested list here highlighting the process for installing on host/steam deck, configuration, recommended settings, recommended controller config, --> 

Gamestream allows you to stream any of your games from your PC using a Nvidia GTX or RTX graphics card. Using high speed, low latency video encoders built into GTX/RTX GPUs It's intended use is for you to stream your games to a Nvidia Shield TV or Shield Tablet. 


Note: Nvidia has announced they are dropping GameStream from the Shield in early 2023 which will essentially kill Moonlight's current functionality without using Sunshine.

## MoonDeck
<!--downloaded from Deckyloader store. Show how to do that or maybe show the store in the seperate deckyloader section. Link to that from here.-->

MoonDeck is a plugin downloaded via the Deckyloader storefront. It is a quicker way to stream your games via Moonlight. The positive to using MoonDeck is that you're able to use seperate controller layouts based on the game you're playing. 

## [Sunshine](https://github.com/LizardByte/Sunshine)
Sunshine is a Gamestream host for Moonlight. This removes the need to have a Nvidia graphics card so if you're using an AMD card this is what you'll need to use Moonlight. Since Nvidia has announced they will be removing Gamestream from the Geforce Experience application, there have been huge imrpovements with Sunshine development. It's essentially the replacement to Nvidia's Gamestream. It performs as good or better than Gamestream did but also offers other useful features. 

ie. Being able to choose which controller type is being emulated when using Moonlight.

## Installation

1. Go to the github page and click on releases on the right hand side. <!--Insert image-->
2. Download the file that corresponds to your operating system. ie. If you're on Windows, you'd download either the exe file or the windows.zip file. 
3. If you downloaded the exe then just run it. 
4. You will see an option to create a username and password for your web interface. Try not to forget it but if you do you can enter the following command in terminal to reset it. <!--Enter commands given to me in Discord-->
5. In the Terminal you should see the localhost link where is where you'd be doing all of your customization.
6. You will need to go into Moonlight where you should see a new device ready to be paired and connect to it. 
7. When it gives you the code, you enter this in the webui under *code* <!--Check proper language--> 
8. You should now be able to connect via Moonlight as you were before with Gamestream.  


## [Greenlight](https://github.com/unknownskl/xbox-xcloud-client)
Greenlight is an Xbox Remote Play app. Not to be confused with xCloud. This is used to connect directly to your Xbox.

1. Go into Desktop mode by pressing the Steam button -> Power -> Desktop Mode
2. Download [AppImageLauncher](https://github.com/TheAssassin/AppImageLauncher/releases/download/v2.2.0/appimagelauncher-lite-2.2.0-travis995-0f91801-x86_64.AppImage) and rename it to appimagelauncher.AppImage (Case sensisitve)
3. Inside the folder AppImageLauncher was downloade, right click an empty area and select Open Terminal. 
4. Run these two commands. 

    ``chmod +x appimagelauncher.AppImage``


    ``./appimagelauncher.AppImage install``
5. Download the Greenlight AppImage [here](https://github.com/unknownskl/xbox-xcloud-client/releases/download/v1.2.0/Xbox-xCloud-1.2.0.AppImage) and save it in the Home/Applications directory. 
6. Select Start -> Utilities and right click Xbox-xCloud. 
7. Select Properies -> Launch Options
8. Enter the following
    
    ``--no-sandbox --fullscreen`` 
9.  (Optional) While in Properties, rename the shortcut to Xbox Remote Play. 
10. Click play and login to your account. 
11. Connect to your console. 

>If you don't see your console listed then make sure your Xbox is setup for remote play by going to Settings -> Devices & Connections -> Remote features and seelct Enable remote features.

12. Switch into Gaming mode. 
13. Run Xbox Remote Play & play your games!
>Note: Go into Controller settings via the Steam button and map a button to the N key. This will be your Xbox button. 



# Non-Steam Games
<!-- Consider combining this with Other Launchers -->

# Other Launchers

## Lutris
<!--Explain how to install and what it does. List services it connects to.-->

## Heroic
<!--Explain how to install and what it does. List services it connects to. Also compare to Lutris-->


# Tools

## [Decky Loader](https://github.com/SteamDeckHomebrew/decky-loader)
Decky Loader is a plugin-manager used to install various useful tools into the Quick Action Menu [...]
<!-- Describe deckyloader. Maybe create a nested list for each current plugin. -->

## ProtonQT
<!--Explain how to use this and why you should use it. Maybe look up an example of a game that needs it to run. 

## Cryobyte33 Steam Deck Utilities
<!--Explain how to use this tool and why it's useful-->

## Steamdeck utils
<!-- Dev changed name. Need to look it up -->

# Accessories 

<!--Steam Dock + 3rd Party Docks, Compact M+KB, SD Card, -->
## Docks
NOTE: There are no docks that will make the Steam Deck run better while connected to a TV. 


[Steam Deck Docking Station](https://store.steampowered.com/steamdeckdock) 

This is the official dock released by Valve for the Steam Deck. 

## Tech Specs 
<sup>*Taken directly from Valves store page.</sup>


| Expansion |  <!-- -->
|----------|----------|
| Peripherals | 3x USB-A 3.1 Gen1 Ports |
|Networking | Gigabit Ethernet |
|External displays | DisplayPort 1.4 <br />HDMI 2.0 <br /> Supports up to 4K 60hz, or 1440p 120hz <br />

| Power | <!-- -->
|-------|---------|
|Input | USB-C Power Delivery passthrough input (power supply included) |
|Deck Connection | 6" USB-C captive cable with low profile 90 degree connector |
|Charger | Included PSU with 1.5m long cable (same as what comes with Steam Deck) |

| Size and Weight | <!-- -->
|-----------------|-----------|
| Size | 117mm x 29mm x 50.5mm
| Weight | Approximately 120 grams
