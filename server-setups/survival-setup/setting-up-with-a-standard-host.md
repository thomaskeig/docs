---
description: >-
  Just a friendly reminder that you cannot redistribute this setup or re-use
  configs in any other servers that you don't own and all payments are final.
---

# Setting up with a Standard Host

This page walks you through setting up the Servival Setup on most server hosts. If you are using Minehut, please follow the setup [here](setting-up-with-minehut.md).

### 1. Create your Zip File

Find the server files in your downloaded files. You should be in a directory similar to the image below.

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Select all the files and add them to a ZIP file. I recommend using 7Zip for this but any zipping program should work.

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

### 2. Upload to your Server

Once you have a ZIP file of your server files, shut down your server and connect to it via FTP or SFTP (contact your server hosting provider if you don't know how to do this).

You then need to delete/cut all the server files out of the main directory of your server. If you want to keep these files, you'll have to put them in another folder or download them to somewhere else.

Upload your newly created ZIP file to your server host. It should be the only file on there.

Unzip the file; it should create many files in the main directory. Once the file has been unzipped, the .zip can be deleted.

### 3. Download a Server Jar

You will now need to choose a server jar for your server to run. You can use any spigot fork you wish; however, I suggest paper for simplicity. If your server host has a built-in jar downloader, you can use that, ignore this step and proceed using that.

Download the latest **1.19.4** Paper JAR file [here](https://papermc.io/downloads/all) (Click 1.19.4 on the sidebar). and place it in your main server directory. Make sure to set the name of the server jar in the server host settings.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

### 4. TAB & Citizens Plugin

Download the Citizens plugin [here](https://ci.citizensnpcs.co/job/Citizens2/) and place it into your /plugins folder.

Download the TAB plugin [here](https://github.com/NEZNAMY/TAB/releases) and place it into your /plugins folder.

### 5. EULA

You will need to accept my Mojang EULA by going into `eula.txt` and changing `false` to `true` to start the server.

### 6. Starting the Server

After you have uploaded the server jar, you can start the server and enjoy your premade setup. (NOTE: The startup may take longer for the first time, as it needs to generate the necessary files).

### Extra Information

You will probably find that when you first log in, there are a lot of plugin updates. We recommend updating these if you can to avoid any issues further down the line.

Make sure to read the [Extra Information](../boxpvp-setup/extra-information.md) to continue with the setup and personalise it.

If you have trouble setting up the server, please join the discord server for support. The link can be found on [this](../../) page.



