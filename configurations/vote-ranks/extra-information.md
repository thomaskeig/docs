---
description: A few commonly asked questions about the Vote Ranks config
---

# Extra Information

## List of the files which need to be changed:

* Change Vote Rewards - `vote.yml (Line 27 & 28)`
  * **NOTE:** You will need to configure VotingPlugin yourself to actually give out the continuous vote rewards.
* Change Vote Links - `vote.yml (Line 64)`

## How do I reset Playtime Levels?

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

## Common Issues:

### Issue: All the ranks are already claimed when I open the menu.

**FIX:** Players with OP will see all ranks as claimed. To revoke this, give those players the FALSE node on the permission: `meta.voterank.*`.\
\
This can be done on luckperms using the following commands:

* **User:** `/lp user <username> permission set meta.voterank.* false`
* **Group:** `/lp group <groupname> permission set meta.voterank.* false`

### Issue: When using /vote, a different GUI comes up.

**FIX:** Make sure that you've followed step no 5.
