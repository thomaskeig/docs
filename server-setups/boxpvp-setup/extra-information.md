---
description: >-
  This page contains extra good-to-know information about the setup before you
  use it!
---

# Extra Information

### List of the files which need to be changed:

* `plugins/DecentHolograms/holograms/hologram_spawn.yml` (Change Store Link)
* `plugins/DeluxeMenus/gui_menus/discord.yml` (Change Discord link)
* `plugins/DeluxeMenus/gui_menus/vote.yml` (Change Voting links)
* `plugins/TAB/config.yml` (Change IP on TAB & Scoreboard)
* `plugins/Infiniteannouncements/announcements.yml` (Change Store Link)
* `plugins/DeluxeMenus/gui_menus/coinshop.yml` (Change Store Link)
* `plugins/MiniMOTD/main.conf` (Change MOTD)
* OPTIONAL: `server-icon.png` (Change the Server Icon - File Found in the main directory)

### List of the files which need your configuration to setup:

* `plugins/Votifier/config.yml` (Configure Votifier Key)
* `plugins/DiscordSRV/config.yml` (Configure Discord Linking)
* Install Tebex Plugin: [https://tebex.io](https://tebex.io) (Setup your Server Store)

### Managing Coins

Coins can be given and removed to players using the `/points` command. The essential commands can be found below, or you can go [here](https://github.com/Rosewood-Development/PlayerPoints/wiki/Commands-&-Permissions) for the full plugin command list.

* `/points give <name> <amount>` - Give coins to a player.
* `/points take <name> <amount>` - Remove coins from a player.

### Temporary Blocks

All blocks placed in the arena will be removed after a certain time. Temporary blocks can be bypassed and reloaded with the commands below.

* `/temporaryblocksreload` - Reload the config (Perm: `temporaryblocks.reload`)
* `/temporaryblocksbypass` - Toggle your bypass (Perm: `temporaryblocks.bypass`)

### AFK Room

The rewards for the AFK room can be edited in the Skript file - `/plugins/Skript/scripts/afkReward.sk`

### Shopkeeper Trades

The shopkeeper trades can be configured by being opped and shift right-clicking a shopkeeper.

### Default Donator Rank Perks (For Tebex):&#x20;

_These can be changed, but this is what is set by default._

#### VIP:

* VIP prefix in chat & Tablist
* Access to VIP Mine
* 2x Level XP Multiplier
* \+1 AFK Shard every 15 minutes
* 5 Coins as a Daily Reward (Default: 3)
* VIP Kit Access
* 2x Enderchest Rows
* /ptime Command
* /craft Command

#### Pro:

* All perks from VIP Tier
* PRO prefix in chat & Tablist
* Access to Pro Mine
* 2x Concurrent Active Quests
* 8 Coins as a Daily Reward (Default: 3)
* Pro Kit Access
* 3x Enderchest Rows
* /spectate Command
* /hat Command

#### MVP:

* All perks from Pro Tier
* MVP prefix in chat & Tablist
* Access to MVP Mine
* 10 Coins as a Daily Reward (Default: 3)
* MVP Kit Access
* 4x Enderchest Rows
* /enderchest Command
* /disposal Command

#### Elite:

* All perks from MVP Tier
* ELITE prefix in chat & Tablist
* Access to Elite Mine
* 3x Concurrent Active Quests
* 12 Coins as a Daily Reward (Default: 3)
* Elite Kit Access
* 5x Enderchest Rows
* /invsee Command

#### Immortal:

* All perks from Elite Tier
* IMMORTAL prefix in chat & Tablist
* Access to Immortal Mine
* 15 Coins as a Daily Reward (Default: 3)
* Immortal Kit Access
* 6x Enderchest Rows
* /heal Command (10 Minute Cooldown)
