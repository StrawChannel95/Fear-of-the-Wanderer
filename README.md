<p align=center>StrawChannel95 is proud to present:</p>

# <p align=center>**Fear of the Wanderer**</p>

<table stlyle="border: none;">
<tr>
<td><img src="https://github.com/StrawChannel95/Apocalyptic-Wonderland/blob/main/.github/WJIcon.png?raw=true" width="64px" /></td>
<td><a href="https://github.com/wabbajack-tools/wabbajack/releas
es">Download on Wabbajack</a></td>
</tr>
</table>

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

# Preamble
- [Fear of the Wanderer](#fear-of-the-wanderer)
- [Preamble](#preamble)
-   [Requirements](#requirements)                                                                                                                                  
    - [Specifications](#specifications)                                                                                                                           
    - [Steam/GOG Requirements](#steamgog-requirements)
    - [Site Requirements](#site-requirements)                                                                                                            
    - [Extra Requirements](#extra-requirements)                                                                                                                   
-   [Installation](#installation)                                                                                                                                  
    - [File Path Setup](#file-path-setup)
    - [Generating INI Files](#generating-ini-files)                                                                                                                
    - [Clean Installation (Steam)](#clean-installation-steam)                                                                                                     
    - [INI Folders (Steam)](#ini-folders-steam)                                                                                                                   
-   [Steam Config](#steam-config)                                                                                                                                  
    - [Reinstallation](#reinstallation)                                                                                                                           
      - [Steam Library](#steam-library)                                                                                                                            
      - [Setting the Game language to English](#setting-the-game-language-to-english)                                                                              
      - [Disabling Steam Overlay](#disabling-steam-overlay)                                                                                                        
-   [GOG Installation and Config](#gog-installation-and-config)                                                                                                    
    - [Clean Installation (GOG)](#clean-installation-gog)                                                                                                         
    - [INI Folders (GOG)](#ini-folders-gog)                                                                                                                       
-   [Using Wabbajack](#using-wabbajack)                                                                                                                            
    - [Preparations](#preparations)                                                                                                                               
      - [Disabling Base Address Randomization](#disabling-base-address-randomization)
      - [Creating Exclusions](#creating-exclusions)
    - [Downloading and Installing](#downloading-and-installing)
      - [Problems with Wabbajack](#problems-with-wabbajack)
-   [Installing TTW](#installing-ttw)
-   [Post-Installation](#post-installation)
    - [Capping FPS](#capping-fps)
      - [RivaTuner Statistics Server (RTTS)](#rivatuner-statistics-server-rtss)                                                                                    
      - [Special K](#special-k)
-   [Important Info](#important-info)
    - [Where to Ask for Support](#where-to-ask-for-support)                                                                                                        
    - [How to Keep Extra Mods After Updating](#how-to-keep-extra-mods-after-updating)

# What is Wabbajack?

Wabbajack is an automated mod list installer that works by scanning the [META files](https://wiki.wabbajack.org/modlist_author_documentation/Meta%20Files.html) of MO2 Downloads so that it can download the mods on the user's device without redistributing any assets of said mods. This is needed because in the world of Bethesda modding, no clear permissions have been set for mods, each mod can have radically different permissions. That's why things like modpacks, or modlists, as we call them, didn't come until later down the line.

# Requirements

### Specifications

> [!Important]
>
>**If you can BARELY run base New Vegas, you can run this list on 60 FPS.**

### Steam/GOG Requirements

A legal copy of Fallout 3 with all DLCs from either [Steam](https://store.steampowered.com/app/22370/Fallout_3_Game_of_the_Year_Edition/) or [GOG](https://www.gog.com/en/game/fallout_3_game_of_the_year_edition).

A legal copy of Fallout: New Vegas with all DLCs from either [Steam](https://store.steampowered.com/sub/13435/) or [GOG](https://www.gog.com/en/game/fallout_new_vegas_ultimate_edition).

**(I cannot provide support for any other version, the Cut German version and the Epic Games version can be used provided you install [DepotDownloader](https://github.com/SteamRE/DepotDownloader) to get the international executable for the German version, and the [Epic Games Patcher](https://www.nexusmods.com/newvegas/mods/81281) for the Epic Games version, the PCR, Microsoft Store and Gamepass versions are completely unsupported)**

### Site Requirements

A [Nexus Mods](https://nexusmods.com) account (Premium is not necessary but recommended for automated downloads).

A [ModPub](https://mod.pub/) account.

### Extra Requirements

[Every Visual C++ Redistributable Package](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one).

[DirectX Runtime Libraries](https://www.microsoft.com/en-us/download/details.aspx?id=8109).

[.NET Framework](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-8.0.302-windows-x64-installer).

The latest driver versions for your GPU ([NVIDIA](https://www.nvidia.com/download/index.aspx), [Intel](https://www.intel.com/content/www/us/en/search.html#sort=relevancy&f:downloadtype=[Drivers]&f:@tabfilter=[Downloads]&f:@stm_10385_en=[Graphics]), [AMD](https://www.amd.com/en/support/download/drivers.html)).

# Installation

### File Path Setup

- Navigate to the `Root Directory` (`C:\`, `D:\`, etc).
- Create a folder named `Modding`, then open it.
- Create a folder named `Wabbajack`.
- Create another folder named `Fear of the Wanderer`.

### Generating INI Files

- Launch Fallout: New Vegas from Steam/GOG.
- Click `OK` when prompted with `Detecting Video Hardware`.
- Close the launcher.
- Launch Fallout 3 from Steam/GOG.
- Click `OK` when prompted with `Detecting Video Hardware`.
- Close the launcher.

### Clean Installation (Steam)

**If you use GOG, then please skip to the [GOG Installation and Config](#gog-installation-and-config) section of the README.**

In order to ensure that your Fallout: New Vegas and Fallout 3 installations are pristine and vanilla, we are going to completely re-install the game. This is especially important if you have modded the game previously, as left-over files might interfere with your installation. If you never modded Fallout: New Vegas and Fallout 3 and/or never installed other Wabbajack lists, you may skip this step. However, I still recommend you verify the game files through Steam in that case.

-   Uninstall Fallout: New Vegas and Fallout 3 through Steam.
-   Navigate to your Steam directory.
-   If there is still a Fallout: New Vegas and Fallout 3 folder there, delete it.

### INI Folders (Steam)

More Fallout-related files are located inside the so-called `INI folder`, which needs to be cleaned out as well. It contains your save games as well as the game’s INI files and, if you modded Fallout: New Vegas before, NVSE plugin logs.

-   Navigate to the INI folder; this is found under Documents/My Games.
-   If you have an ongoing vanilla playthrough, back up the Saves folder.
-   Delete everything inside the Fallout: New Vegas and Fallout 3 folders.

# Steam Config

### Reinstallation

The reinstallation also serves the purpose of relocating the game files to a better directory. Using `UAC-protected folders` for the game or any modding tools has a risk of causing issues down the line. It is best to avoid those folders to begin with. Most Wabbajack list authors, myself included, will not provide support for people who disregard this warning and use UAC-protected folders anyway. Note that this does not include the `Steam client`. Additionally, Fallout: New Vegas and Mod Organizer 2 should be installed on the same hard drive. Ideally, that hard drive would be an SSD to reduce loading times and eliminate stuttering. 

### Steam Library

In order to prevent some confusion, I will refer to the Library in Steam as the `Game Library`. It is the second of four items in the top menu in the Steam client and contains a list of all your games. A `Steam Library`, on the other hand, is a folder on your hard drive into which Steam games are installed. Since we do not want to have files inside a `UAC-protected folder`, we should not install Fallout: New Vegas in the default directory. A new `Steam Library` is required.

### Setting the Game language to English

You must do this for Wabbajack to work. If your game was previously set to non-English, make sure to verify your files on Steam after fixing it. There is no support for non-English TTW.

Open the `Steam Properties` window, navigate to the `Language` tab, and select `English` from the dropdown menu.

### Disabling Steam Overlay

- Navigate to your Steam root folder (the same folder where your steam.exe is).
- Right click `GameOverlayRenderer.dll` and open properties.
- Open the `security tab` and click `edit`.
- Click the `Deny` option under `Read & Execute` for every user.
- Click `Apply`, then `Yes`.
- In the same folder, right click `SteamOverlayVulkanLayer.dll` and open `properties`.
- Open the `security tab` and click `edit`.
- Click the `Deny` option under `Read & Execute` for every user.
- Click `Apply`, then `Yes`.

# GOG Installation and Config

### Clean Installation (GOG)

Inside the game folders of both Fallout 3 and New Vegas, there will be a file known as `unins000`. Run it, and it will activate the uninstaller; it will completely uninstall the game, and then you have to reinstall it from GOG.

### INI Folders (GOG)

More Fallout-related files are located inside the so-called `INI folder`, which needs to be cleaned out as well. It contains your save games as well as the game’s INI files and, if you modded Fallout: New Vegas before, NVSE plugin logs.

-   Navigate to the INI folder; this is found under Documents/My Games.
-   If you have an ongoing vanilla playthrough, back up the Saves folder.
-   Delete everything inside the Fallout: New Vegas and Fallout 3 folders.

# Using Wabbajack

### Preparations

Grab the latest release of Wabbajack from [here](https://github.com/wabbajack-tools/wabbajack/releases) and place the `Wabbajack.exe` file in the Wabbajack file path that you set earlier.

#### Disabling Base Address Randomization

- Open `Windows Security` from the `Start Menu`.
- Open `App & Browser Control` in the left sidebar.
- Open `Exploit Protection Settings` under `Exploit Protection`.
- Set `Force Randomization for Images (Mandatory ASLR`) to `Use Default (Off)`.

#### Creating Exclusions

- Open `Windows Security`.
- Open `Virus & Threat Protection`.
- Click `Manage Settings` under `Virus & Threat Protection Settings`.
- Scroll down and select `Add or Remove Exclusions` under `Exclusions`.
- Select the `Fear of the Wanderer folder`.
- Add another exclusion for the `Wabbajack Installation` location.
- This process will also need to be done for any third-party antivirus.

### Downloading and Installing

The download and installation process will take a very short time, this is the smallest New Vegas list after all. Wabbajack will calculate the number of threads it will use at the start of the installation. To have the highest number of threads and, thus, the fastest speed, it is advised to have the working folder on an SSD. You can have the `Fear of the Wanderer install folder` and Downloads folders on separate drives without issue, aside from being limited by the slowest drive during Wabbajack installation. Click the `Play` arrow. If you have a Nexus Premium account, all of your downloads will be automated. Without Premium, you will need to manually click the Download button for each mod. Installation will be automated, regardless of your account status.

-  Open Wabbajack.
-  Load the Modlist from Disk.
-  Set Fear of the Wanderer to install to the `Fear of the Wanderer install folder` and download to the `Fear of the Wanderer download folder`.
-  Click the Go/Begin button.
-  Wait for Wabbajack to finish.

### Problems with Wabbajack

There are a lot of different scenarios where Wabbajack will produce an error. If you do not see an installation failure warning, do not worry about it. If you feel like Wabbajack is stuck or a download is hanging, just restart Wabbajack; it will pick up from exactly where you left off. Please rerun Wabbajack at least twice and try to manually download the file from Nexus first before posting about a failed download. Wabbajack will not work with a pirated version of the game. If you own the game on Steam, go back to the [Steam Config](#steam-config) section; if you own it on GOG, go back to the [GOG Installation and Config](#gog-installation-and-config) section.

# Installing TTW

>[!note]
>This section is only required if you use the TTW profile of this list, otherwise, ignore this step.

-   You then want to head over to ModPub and download the [TTW 3.3.2 Installer](https://mod.pub/ttw/133-tale-of-two-wastelands).
-   Extract the downloaded archive to a folder of your choosing.
-   You then want to run the installer as Administrator and set the path to both Fallout 3 and New Vegas, you then want to set the installation folder as the empty mod called `[No Delete] Tale of Two Wastelands`. You can find it by heading to where you installed MO2, going to the `mods` file, and finally going to the file named `[No Delete] Tale of Two Wastelands`, you then want to double-click while hovering the file and you want to copy the file path at the top.
-   Then you wait for the installer; this will take more time if you have other processes running in the background. It is also CPU-bound, so if you have a good CPU, it will be faster. (This will approximately take between 45 minutes and 3 hours).

# Post-Installation

### Capping FPS

> [!Important]
> RTSS is the recommended option for AMD graphics card users. Special K lacks compatibility with the combination of AMD graphics cards and DXVK. NVIDIA graphics card users will have memory related crashes if following this section instead of the [Special K section](#special-k).
>
> Special K is the recommended option for NVIDIA graphics card users. RTSS is not able to configure flip and interop appropriately, which causes a large amount of memory related crashes. AMD graphics card users will not be able to launch the game if following this section instead of the following [RTSS section](#rivatuner-statistics-server-rtss).

#### RivaTuner Statistics Server (RTSS)

- Install and launch [RTTS](https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download).
- Open the `System Tray` (the triangle pointing upwards on the taskbar) and click the `RTSS icon` (an image of a computer screen) to open it.
- Press the green `Add` button and select `FalloutNV.exe` from the `Root` folder.
- Set `Application Detection Level` to `Low`.
- Set `Framerate Limit` to `59.95`.
- Enter settings using the `Setup` button.
- Scroll down and enable `Passive Waiting`.
- Set `Framerate Limiter` to `Front Edge Sync`.
- Optionally enable `On-Screen Display Support` and use the `X,Y Coordinate Buttons` at the bottom to adjust On-Screen FPS display location.
- Minimize RTSS back to the System Tray.

#### Special K

- Navigate to the NVIDIA app settings and `turn off NVIDIA overlay`, as the overlay will cause a black screen if used alongside Special K.
- Download the [Special K](https://sk-data.special-k.info/SpecialK.7z) program.
- Extract the downloaded archive into your downloads folder.
- Open the SpecialK folder.
- Rename `SpecialK32.dll` to `dinput8.dll`.
- Move the newly renamed `dinput8.dll` into the `Root` folder.
- Download the [Viva New Vegas Preconfigured Settings Archive](https://performance.moddinglinked.com/files/sk.zip).
- Extract the newly downloaded `SK.zip` into the `Root` folder.
- Launch Fear of the Wanderer.
- Select `Yes` when prompted to enable DXVK support/vulkan bridge, then relaunch the game.
- Press `Ctrl + Shift + Backspace` to enter the `Special K Control Panel`.
- Under the `Framerate Limiter`, click the `Enable Framerate Limit` checkbox.
- Right click the bar next to Framerate Limit (the one that specifies FPS and says `(Limit Engaged)`, not the graph).
- Select your monitors refresh rate.
- Click `Advanced` and select `Latent Sync (VSYNC -off-) mode`.
- Double Left Click on the bar and type in 59.995, and press `enter`.
- For instructions on configuring Latent Sync, enabling V-Sync or Variable Refresh Rate, please reference the [Special K section of Wall's Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters).

# Important Info

## Where to Ask for Support

Don't ask on the Wabbajack server, they cannot help you; they will tell you to head over and ask the modlist author (me).

Don't DM me or anyone else regarding the list, Ask in the support channels; more people see it, and it makes my life easier.

Please ask in my Discord server, here is the [link](https://discord.gg/ez3dsBub8Q).

## How to Keep Extra Mods After Updating

When updating, any additional mods you have installed on top of Fear of the Wanderer will be deleted. Your downloads folder will not be touched!

If you wish for Wabbajack to ignore any additional mods you've installed, rename them to say `[NoDelete]` at the beginning of the name.

# Credits

- All the mod authors whose mods made this modlist possible.
- JanuarySnow, TDarkShadow and all the other Wabbajack staff for helping us on this eternal one-way ticket.
- reyqune for having a sense of humor.
- Kamchatka for answering my many questions.
- Halgari for being the saint who made Wabbajack.
- Also, fuck you January, you made a list that's an actual safety hazard. Jokes aside, why?

I wish you all a happy nuclear winter.
