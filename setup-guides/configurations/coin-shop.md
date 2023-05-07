---
description: >-
  This page walks you through setting up the Coin Shop config on your server
  host.
---

# 2⃣ Coin Shop

## 1. Extract & Find the Folder

Extract the downloaded .zip file and locate the folder named "plugins"

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

## **2. Installing Dependencies**

Download [DeluxeMenus](https://www.spigotmc.org/resources/deluxemenus.11734/), [Vault](https://www.spigotmc.org/resources/vault.34315/), [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/), [Luckperms](https://luckperms.net/download), [PlayerPoints](https://www.spigotmc.org/resources/playerpoints.80745/), [DeluxeTags](https://www.spigotmc.org/resources/deluxetags.4390/), [eGlow](https://www.spigotmc.org/resources/eglow-glow-cosmetic-respects-eula-mysql.63295/), [EZColors](https://www.spigotmc.org/resources/1-8-8-1-19-3-ezcolors.69871/), and [UltraCosmetics](https://www.spigotmc.org/resources/1-8-8-1-19-4-ultra-cosmetics-opensource-free.10905/). Copy the jar files into your plugin folder if you already have them on the server.

## 3. Installing the config

Copy the folders from the /plugins folder in the config files into your server /plugins folder. If some folders already exist, you may need to combine them (If you already have configs for any setups other than DeluxeMenus, DeluxeTags or UltraCosmetics, I would recommend sticking with the current ones on your server as they are not essential.

## 4. Final Setup

The config is built to work with PlayerPoints (for coins). If your server uses a different plugin, you'll have to change the commands in the file (but this can be done quickly with find and replace tools).

## 5. Extra Information

Please read the contents of the dropdown below to learn more about the configuration:

<details>

<summary>Extra Information - Coin Shop</summary>

### How do I give players coins?

Coins are handled through the PlayerPoints plugin. You can use the base command `/points` to give and take coins from people

### Rank Backwards Buying:

Add the `meta.group.<name>` permission to each of your ranks to prevent players from being able to purchase ranks they already own. If you have changed the rank names in the config, you will also need to change this metadata.

### Common Issues:

None yet; check back here soon!

</details>



