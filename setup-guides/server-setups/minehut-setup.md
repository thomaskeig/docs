---
description: Learn how to set up any of my setups on a Minehut with ease!
---

# 💾 Minehut Setup

{% hint style="info" %}
This page walks you through setting up my server setup on Minehut. If you are using a different server host, please follow the guide [here](standard-host-setup.md).
{% endhint %}

## 1. Create your Zip File

Find the server files in your downloaded files from BuiltByBit or Polymart. You should be able to find the directory that looks similar to the following:

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Select all the files and add them to a ZIP file. I recommend using 7Zip for this but any zipping program should work.

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

## 2. Upload to your Minehut Server

* Shut down your server from the main settings tab and make your way to the file manager tab.

<figure><img src="../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

* You then need to delete/cut all the server files out of the main directory of your server. If you want to keep these files, you'll have to put them in another folder or download them somewhere else.
* To delete all your files, tick all the boxes to the left of the server folders, then press the trash can icon at the bottom of your screen.

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

* Upload your newly created ZIP file to this file directory by using the upload file button. It should then be the only file on there.
* Unzip the file by right-clicking it and pressing "Unzip"; it should create many files in the main directory. Once the file has been unzipped, the .zip can be deleted.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

## 3. Select Server Version

Make your way back to the settings tab and under the panel named "Server Version". Select "Paper" as your Server Type and choose the correct server version. You can find out what server version is supported for the setup you have bought on [this](../../miscellaneous/resource-versions.md) page. Then press "Update" to save the changes.

{% hint style="danger" %}
It is extremely important that all server setups are run using the specific versions as shown on [this](../../miscellaneous/resource-versions.md) page. Failure to comply with this requirement may lead to the failure of the world to load if an earlier version is used, or the inability of certain plugins to function if a later version is used. To enable connectivity for clients utilizing different versions, the use of [ViaVersion](https://hangar.papermc.io/ViaVersion/ViaVersion) and/or [ViaBackwards](https://hangar.papermc.io/ViaVersion/ViaBackwards) is recommended.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

## 4. Plugin Dependencies

Because of licensing restrictions with certain plugins used in the setups, you will need to download some independently and add them to your `/plugins` folder. You can find links to these here:

* [TAB Plugin](https://github.com/NEZNAMY/TAB/releases)
* [Citizens Plugin](https://ci.citizensnpcs.co/job/Citizens2/)

{% hint style="info" %}
If you are setting up the Lifesteal Setup and wish to utilize the LifestealCore integration, please see the setup guide [here](../../miscellaneous/lifestealcore-integration.md).
{% endhint %}

## 5. Agree to the EULA

You will need to accept the [Minecraft EULA](https://www.minecraft.net/en-us/eula) by going into the `eula.txt` and changing `false` to `true` to start the server.

## 6. Starting the Server

You can start the server and enjoy your premade setup. Please be aware that the startup may take longer for the first time, as it needs to generate the necessary files.

Due to how pre-made server setups are created and delivered, you will probably find that when you first log in, there are a lot of plugin updates. I recommend updating these if you can to avoid any issues further down the line.

## 7. Styling your server

To obtain further information regarding server styling, rank permissions, and essential tips, kindly refer to the instructions outlined on [this](extra-information.md) page.

