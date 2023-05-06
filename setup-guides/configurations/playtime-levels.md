---
description: >-
  This page walks you through setting up the Playtime Levels config on your
  server host.
---

# 1⃣ Playtime Levels

## 1. Extract & Find the Folder

Extract the downloaded .zip file and locate the folder named "plugins"

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

## **2. Installing Dependencies**

Download [DeluxeMenus](https://www.spigotmc.org/resources/deluxemenus.11734/), [RocketPlaceholders](https://www.spigotmc.org/resources/rocketplaceholders-custom-placeholders.82678/) and [jShader](https://www.spigotmc.org/resources/jshader.93342/). Copy the jar files into your plugin folder.

## 3. Installing the config

If you have installed DeluxeMenus for the first time, drag the contents of the `Playtime Levels vX.X.X/plugins` folder into the `/plugins` folder of your server. This should hold the config files for DeluxeMenus and RocketPlaceholders. You can then restart your server and move on to the next step.

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

## 4. Final Setup

Playtime Rewards should now be working on your server. However, all players will need the `playtimelevels.open` permission to be able to use the menu. Make sure you grant this to the rank that you want to be able to use them.

The config is built to work with EssentialsEconomy, LifestealCore (Premium) & PlayerPoints (for coins). If your server uses a different plugin, you'll have to change the commands in the file (but this can be done quickly with FIND and REPLACE).

## 5. Placeholders

* `%rp_playtimelevels_level%` - Shows the player's current level.

## 6. Extra Information

Please read the contents of the dropdown below to learn more about the configuration:

<details>

<summary>Extra Information - Playtime Levels</summary>

### Resetting Playtime Levels?

You may want to reset the levels for various reasons; the most common one is for a new season/reset. Here's how to do it.

1. The Playtime Data is stored in the world statistics folder. Turn off your server, go to `/world/stats` and delete the folder.
   * Your "world" folder may be named differently depending on if you changed your default world in `server.properties`
   * This will also delete player statistics from the in-gaming "Statistics" menu.
2. Turn your server back on and run the following command in the console. This will bulk delete all player permission nodes that tell the config which rewards have been claimed.\
   \
   `/lp bulkupdate users delete "permission ~~ meta.playtimelevels.%`\
   \
   After running this command, you must run another command to confirm the action. It will let you know in the console what this command is.\
   \
   These commands make use of LuckPerms' Bulk Update command. You can view their documentation [here](https://luckperms.net/wiki/Bulk-Editing) to learn more about the command.

### Common Issues:

#### Issue: All the rewards are already claimed when I open the menu.

**FIX:** Players with OP will see all rewards as claimed. To revoke this, give those players the FALSE node on the permission: `meta.playtimelevels.*`.\
\
This can be done on luckperms using the following commands:

* **User:** `/lp user <username> permission set meta.playtimelevels.* false`
* **Group:** `/lp group <groupname> permission set meta.playtimelevels.* false`

#### Issue: When using /playtime, the EssentialsX command gets used instead of the DeluxeMenus one.

**FIX:** Go into your Essentials config & add “playtime” under “disabled-commands:” then restart your server.

</details>



