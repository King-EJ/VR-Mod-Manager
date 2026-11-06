# VR-Mod-Manager
VR MOD MANAGER  -  install / update / turn off / uninstall BepInEx mods (all the VR mods)


HOW TO USE
  * Double-click "VR Mod Manager.bat".
    - If it is in a game folder (next to the game's .exe) it uses that game.
    - Otherwise it offers the last game you used, or asks you to pick the game folder.
  * Or DRAG a mod zip (or several) onto "VR Mod Manager.bat" - it installs them right away.

MENU
  1) Install / update a mod (or BepInEx itself) from a zip
       Lists the zips next to the .bat, or browse for one. Works with any zip that has a "BepInEx" folder
       inside (also when it's inside another folder in the zip). Your settings (BepInEx\config) are never
       overwritten. The mod's README is put in the mod's folder and you can open it.
  2) Uninstall a mod      - removes all its files (it remembers what it installed); asks if you also want to
                            delete its settings file (keep it if you may install the mod again).
  3) Turn a mod on / off  - an "off" mod is moved to BepInEx\plugins_disabled (not loaded), nothing deleted.
  4) Open the mod log     - BepInEx\LogOutput.log in Notepad (the file to send when something goes wrong).
  5) Open the game folder
  6) Choose another game
  7) Remove BepInEx and all mods from this game - the game is back to normal. Your settings are backed up
     to Documents\VR mod settings backup\<game> first.

The top of the screen shows the game, if it is Mono (BepInEx 5) or IL2CPP (BepInEx 6), which BepInEx is
installed (and warns if winhttp.dll is missing) and all mods with on / off.

NOTES
  * Close the game before installing / uninstalling (it tells you if it is still running).
  * Windows may ask "Do you want to run this file?" the first time - that's normal for a downloaded .bat.
  * It's a plain text file (PowerShell inside) - open it in Notepad to see exactly what it does.
