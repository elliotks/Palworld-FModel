# Instructions
1. Download FModel [https://github.com/4sval/FModel/releases]
2. Configure Settings in FModel
GAME  
Archive Directory: <PATH>\SteamLibrary\steamapps\common\Palworld  
UE Versions: GAME_UE5_1  
Texture Platform: Desktop / Mobile  
Compressed Audio: Play the decompressed data  
ADVANCED  
Local Mappings File: Enabled  
Mapping File Path (downloaded from this repo): <PATH>\Pal-Windows_1.2_Steam_Mappings.usmap  
![image](https://github.com/elliotks/Palworld-FModel/assets/10646544/cb09bdc2-a166-4344-b59b-dccb24ff1a2a)
3. ???
4. Profit!

## Documentation I followed
-   Procedure to check the contents of a pak file in FModel

This is the content we have organized after receiving the information. Thank you for the information. I am writing this because I received information from an English\-speaking person and succeeded in unpacking, so I thought I should share the information here as well. I can only speak Japanese, so I am writing this using automatic translation. Please let me know if the same information has already been shared. I will delete the post.

1.  install Unreal Engine 4/5 Scripting System

[https://github.com/UE4SS-RE/RE-UE4SS](https://github.com/UE4SS-RE/RE-UE4SS "https://github.com/UE4SS-RE/RE-UE4SS")

2.  modify the configuration file as follows

```
[Debug]
ConsoleEnabled = 0
GuiConsoleEnabled = 1
GuiConsoleVisible = 1
```

`ConsoleEnabled` can be 0 or 1.

3.  launch the game

4.  output mapping file (image 1)

Output `.usmap` from the `Dumper` tab of the `UE4SS Debugging Tool`. How the file is output. `Palworld(Game Folder Root)\Pal\Binaries\Win64\Mappings.usmap`. At this point, the work on the game side is finished and you may exit the game. 5.

5.  install FModel

[https://github.com/4sval/FModel](https://github.com/4sval/FModel "https://github.com/4sval/FModel")

6.  add reference settings for pal world in FModel (image 2)

7.  add reference settings for mapping file in FModel (image 3)

Specify the file output in step 4. The mapping file may need to be updated when the game version is updated. 8.

8.  check any file

Double\-click `.uasset` to see the contents of the file.

-   How to find it in the file tree

Select any `pak` file from `Archives`, select any folder in the `Folders` tab, and search for any file in the `Packages` tab.

-   How to search from the whole

Select `Search` from the top menu `Packages` and enter any string to search.

(See Source post for images)

Source: [Palworld Discord](https://discord.com/channels/505994577942151180/1196354583040118824/1198468327308271698)

# AES Decryption - Not required, but good information
Backup Repo: [https://github.com/elliotks/UE4-AES-Key-Extracting-Guide] 
Original Repo: [https://github.com/Cracko298/UE4-AES-Key-Extracting-Guide]
