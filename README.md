# ![Droplets](https://github.com/user-attachments/assets/b78ae8fe-da35-414b-a720-cf7c7241ddd0) GSpots

Simple way of getting GWorld, GNames, and GObjects of an Unreal Engine Game.

![GSpots](https://github.com/user-attachments/assets/b089c37f-1c2d-4845-9296-65cadc30c672)

<details>
 
   <summary>Demo Videos</summary>
 
   https://github.com/user-attachments/assets/09385216-2965-4023-9e87-830c1a8e0818

   https://github.com/user-attachments/assets/dba9ca71-98ce-4fb8-af61-86e96e7cb997

 </details>  

## Need Help? Join our <a href="https://discord.gg/TRDsYfNEV8">Discord</a>! - Be sure to react with "Game Modding" in reaction roles.  
Looking for a new memory editor? - https://github.com/Do0ks/MemRE

# How to use

- Download the precompiled release, or build in x64-release with Multi-Byte Character Set.  
- Drag and drop the games executable onto GSpots.exe ( The executable located in <b>..\Binaries\Win64</b>. It typically includes "Win64-Shipping.exe" in the name )

- You don't have to have the game running in the background, but if you do it will improve scanning results greatly. GSpots will automatically attach to the games process, if it fails to find offsets with the file scan method, it will try to find the missing ones in the games memory.

### This will not work on EVERY Unreal Engine game...

If the games exe is encrypted, this could bypass it via the memory scan, but if they have taken the time to encrypt the exe, chances are they also took the time obfuscating other things too.. But, it should get you close!

<b>As time goes on I will add more signatures!</b>  
If you have a game that is unsupported, feel free to post in the [Game Compatibility Request](https://github.com/Do0ks/GSpots/issues/1) thread. 

# Planned Fetures:
<details>
  
  ## Soon:  
  
  - Add automatic fetching of the Unreal Engine Version the game is built with. :white_check_mark:
  
  - Add XOR encryption calculations with padding if applicable.

  - Added memory scan if the games running in the background to try finding the offsets file scanning failed at. :white_check_mark:

  ## Later:  

  - Try to pre calculate point of interest pointer chains such as the player class while the games running. This should function like before (you'll just need the game running before dropping the games exe onto GSpots.exe)
  
</details>

# Updates:
<details>

- Added the ability to attach to the game IF its running. This is in preperation for future updates.

- Added functions from my other github repository to detect the Unreal Version number.

- Added memory scan if the games running in the background to try finding the offsets file scanning failed at.
Memory scanning is in beta.. It worked for every game i tried, and the one that it didn't work for has obfuscation. This update should help compatibility greatly!

- Added The ability to detect and handle encrypted exes.

</details>

# Disclosure:
<details>

- If you choose to use this tool with a online game and you get banned, thats on you. I put no effort into making this tool evade anti cheat detection. While I don't expect anyone to be banned (I havent yet) for using GSpots, It's always a risk.

</details>

# Some Other Awesome Tools!

<details>

 - Injectable Memory Scanner - https://github.com/Do0ks/B2D-Scanner

 - DLL Injector - https://github.com/Do0ks/Injector

</details>
