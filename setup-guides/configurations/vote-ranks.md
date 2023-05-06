---
description: >-
  This page walks you through setting up the Vote Ranks config on your server
  host.
---

# 3⃣ Vote Ranks

## 1. Extract & Find the Folder

Extract the downloaded .zip file and locate the "Configuration Files" folder. Open that folder and choose the configuration for your shop plugin.

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

## **2. Installing Dependencies**

Download [DeluxeMenus](https://www.spigotmc.org/resources/deluxemenus.11734/), [RocketPlaceholders](https://www.spigotmc.org/resources/rocketplaceholders-custom-placeholders.82678/), [jShader](https://www.spigotmc.org/resources/jshader.93342/) and [VotingPlugin](https://www.spigotmc.org/resources/votingplugin.15358/). Copy the jar files into your plugin folder. It is assumed that you already have your shop plugin on your server.

## 3. Installing the config

If you have installed DeluxeMenus for the first time, drag the contents of the `/plugins` folder into the `/plugins` folder of your server. This should hold the config files for DeluxeMenus and RocketPlaceholders. You can then restart your server and move on to the next step.

If you already have DeluxeMenus running other GUIs on your server, you will need to copy the menu separately.

* Open `/plugins/DeluxeMenus/gui_menus` in the Playtime Levels resource folder and copy the `vote.yml` file. Upload this to the `/plugins/DeluxeMenus/gui_menus` folder in your server host.
* Navigate to /plugins/DeluxeMenus/config.yml in your server host. Open the file and add the following to the bottom of the file:

```
  vote:
    file: vote.yml
```

* You can now reload DeluxeMenus with `/dm reload` and continue.

## 4. Shop Modifiers

Follow the different steps depending on the shop plugin you are using:

### ShopGUI+

1. Open the `pricemodifiers.yml` file in the ShopGUI+ directory.
2. Replace the text in that file with [this](https://pastebin.com/raw/0USKvSxP) text.
3. Save the file and reload the plugin.

### EconomyShopGUI

1. Open the config.yml file in the EconomyShopGUI directory.
2. Set `enable-sell-multipliers` to true in the config.
3. Locate the `sell-multipliers:` key in the file and replace everything underneath that key (not the rest of the file) with [this](https://pastebin.com/raw/ZeBDr5UF) text.
4. Save the file and reload the plugin.

## 5. Final Setup

Add the following to the bottom of your commands.yml file in the root folder of your host. This will ensure that the correct menu opens.

```
  vote:
  - deluxemenus:vote $1-
```

The config is built to work with PlayerPoints (for coins). If your server uses a different plugin, you'll have to change the commands in the file (but this can be done quickly with find and replace tools).

## 6. Placeholders

* `%rp_voteranks_rank%` - Shows the player's rank as a nice rank (Useful for chat, tab and above name)
* `%rp_voteranks_number%` - Shows the player's rank as a number.

## 7. Extra Information

Please read the contents of the dropdown below to learn more about the configuration:

<details>

<summary>Extra Information - Vote Ranks</summary>

### List of the files which need to be changed:

* Change Vote Rewards - `vote.yml (Line 27 & 28)`
  * **NOTE:** You will need to configure VotingPlugin yourself to actually give out the continuous vote rewards.
* Change Vote Links - `vote.yml (Line 64)`

### How do I reset Playtime Levels?

You may want to reset the levels for various reasons; the most common one is for a new season/reset. Here's how to do it.

1. Run the following command in the console. This will bulk delete all player permission nodes that tell the config which rewards have been claimed.\
   \
   `/lp bulkupdate users delete "permission ~~ meta.voterank.%`\
   \
   After running this command, you must run another command to confirm the action. It will let you know in the console what this command is.\
   \
   These commands make use of LuckPerms' Bulk Update command. You can view their documentation [here](https://luckperms.net/wiki/Bulk-Editing) to learn more about the command.
2. You now need to remove the shop multipliers from each player, this is different based on which shop plugin you use. The process works the same as the previous step, just with a different command.\
   \
   **ShopGUIPlus:** `/lp bulkupdate users delete "permission ~~shopguiplus.pricemodifiers.%`\
   \
   **EconomyShopGUI:** `/lp bulkupdate users delete "permission ~~ economyshopgui.sell-multipliers.%`

### Common Issues:

#### Issue: All the ranks are already claimed when I open the menu.

**FIX:** Players with OP will see all ranks as claimed. To revoke this, give those players the FALSE node on the permission: `meta.voterank.*`.\
\
This can be done on luckperms using the following commands:

* **User:** `/lp user <username> permission set meta.voterank.* false`
* **Group:** `/lp group <groupname> permission set meta.voterank.* false`

#### Issue: When using /vote, a different GUI comes up.

**FIX:** Make sure that you've followed step no 5.

</details>



