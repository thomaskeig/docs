---
description: A few commonly asked questions about the Playtime Levels config
---

# Extra Information

## How do I reset Playtime Levels?

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

## Common Issues:

### Issue: All the rewards are already claimed when I open the menu.

**FIX:** Players with OP will see all rewards as claimed. To revoke this, give those players the FALSE node on the permission: `meta.playtimelevels.*`.\
\
This can be done on luckperms using the following commands:

* **User:** `/lp user <username> permission set meta.playtimelevels.* false`
* **Group:** `/lp group <groupname> permission set meta.playtimelevels.* false`

### Issue: When using /playtime, the EssentialsX command gets used instead of the DeluxeMenus one.

**FIX:** Go into your Essentials config & add “playtime” under “disabled-commands:” then restart your server.
