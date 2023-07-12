---
description: >-
  This page walks you through setting up the Simple Prestiges config on your
  server host.
---

# Simple Prestiges

## 1. Extract & Find the Folder

Extract the downloaded .zip file and locate the folder named "Configuration Files"

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

## **2. Installing Dependencies**

Download [DeluxeMenus](https://www.spigotmc.org/resources/deluxemenus.11734/), [LifestealCore](https://www.spigotmc.org/resources/101284/) & [PlaceholderAPI](https://www.spigotmc.org/resources/6245/). Copy the jar files into your plugin folder.

## 3. Installing the config

If you have installed DeluxeMenus for the first time, drag the contents of the `DeluxeMenus` folder into the `/plugins` folder of your server. You can then restart your server and move on to the next step.

If you already have DeluxeMenus running other GUIs on your server, you will need to copy the menu separately.

Open `/plugins/DeluxeMenus/gui_menus` in the Simple Prestiges resource folder and copy the YML file. Upload this to the `/plugins/DeluxeMenus/gui_menus` folder in your server host.

Navigate to /plugins/DeluxeMenus/config.yml in your server host. Open the file and add the following to the bottom of the file:

```
  prestige:
    file: prestige.yml
```

You can now reload DeluxeMenus with `/dm reload` and continue.

## 4. Final Setup

Make sure you have downloaded the Player and Math expansion with the commands:\
`/papi ecloud download Player`\
`/papi ecloud download Math`

Once you have ran these two commands, reload PlaceholderAPI with `/papi reload`.

The config is built to work with LifestealCore. If your server uses a different plugin (assuming you can set a user's maximum hearts), you'll have to change the commands in the file (but this can be done quickly with FIND and REPLACE).

## 5. Extra Information

Please read the contents of the dropdown below to learn more about the configuration:

<details>

<summary>Extra Information - Simple Prestiges</summary>

### Resetting Prestiges?

Prestige data is kept in LifestealCore, so when you reset that data, user prestiges will reset too.

### Common Issues:

None yet.

</details>



