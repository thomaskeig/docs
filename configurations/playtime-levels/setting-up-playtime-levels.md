---
description: >-
  Just a friendly reminder that you cannot redistribute this setup or re-use
  configs in any other servers that you don't own and all payments are final.
---

# Setting up Playtime Levels

This page walks you through setting up my Playtime Levels config on your server host.

### 1. Extract & Find the Folder

Extract the downloaded .zip file and locate the folder named "plugins"

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

### **2. Installing Dependencies**

Download [DeluxeMenus](https://www.spigotmc.org/resources/deluxemenus.11734/), [RocketPlaceholders](https://www.spigotmc.org/resources/rocketplaceholders-custom-placeholders.82678/) and [jShader](https://www.spigotmc.org/resources/jshader.93342/). Copy the jar files into your plugin folder.

### 3. Installing the config

If you have installed DeluxeMenus for the first time, simply drag the contents of the `Playtime Levels vX.X.X/plugins` folder into the `/plugins` folder of your server. This should hold the config files for DeluxeMenus and RocketPlaceholders. You can then restart your server and move on to the next step.

If you already have DeluxeMenus running other GUIs on your server, you will need to copy the menus separately.

Open `/plugins/DeluxeMenus/gui_menus` in the Playtime Levels resource folder and copy the YML files. Upload these to the `/plugins/DeluxeMenus/gui_menus` folder in your server host.

Navigate to /plugins.DeluxeMenus/config.yml in your server host. Open the file and add the following to the bottom of the file:

```
  playtime:
    file: playtime.yml
  playtime2:
    file: playtime2.yml
  playtime3:
    file: playtime3.yml
  playtime4:
    file: playtime4.yml
  playtime5:
    file: playtime5.yml
  playtime6:
    file: playtime6.yml
  playtime7:
    file: playtime7.yml
```

You can now reload DeluxeMenus with `/dm reload` and continue.

### 4. Final Setup

Playtime Rewards should now be working on your server. However, all players will need the `playtimelevels.open` permission to be able to use the menu. Make sure you grant this to the rank that you want to be able to use them.

The config is built to work with EssentialsEconomy, LifestealCore (Premium) & PlayerPoints (for coins). If your server uses a different plugin, you'll have to change the commands in the file (but this can be done quickly with FIND and REPLACE).

### 5. Placeholders

The placeholder for a player's Playtime Level can be fetched using `%rp_playtimelevels_level%`.

### Extra Information

Please read the [Extra Information](extra-information.md) page before asking any questions in the support server.

Please join the discord server for support if you have trouble setting up the config. The link can be found on [this](../../) page.



