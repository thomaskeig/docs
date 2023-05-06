---
description: >-
  This page contains extra good-to-know information about the setup before you
  use it!
---

# Extra Information

### List of the files which need to be changed:

* `plugins/DecentHolograms/holograms/spawn.yml` (Change Store Link)
* `plugins/DeluxeMenus/gui_menus/discord.yml` (Change Discord link)
* `plugins/DeluxeMenus/gui_menus/vote.yml` (Change Voting links)
* `plugins/TAB/config.yml` (Change IP on TAB & Scoreboard)
* `plugins/Infiniteannouncements/announcements.yml` (Change Store Link)
* `plugins/DeluxeMenus/gui_menus/coinshop.yml` (Change Store Link)
* `plugins/MiniMOTD/main.conf` (Change MOTD)
* **OPTIONAL:** `server-icon.png` (Change the Server Icon - File Found in the main directory)

Note: If you need to put your IP in the small caps font, you can use [this page](https://www.madeintext.com/small-caps-text-generator/) or use the bot in my [Discord Server](https://dsc.gg/thomaskeig) (`/smallcaps`)

### List of the files which need your configuration to setup:

* `plugins/Votifier/config.yml` (Configure Votifier Key)
* `plugins/DiscordSRV/config.yml` (Configure Discord Linking)
* Install Tebex Plugin: [https://tebex.io](https://tebex.io) (Setup your Server Store)

### Managing Coins

Coins can be given and removed to players using the `/points` command. The essential commands can be found below, or you can go [here](https://github.com/Rosewood-Development/PlayerPoints/wiki/Commands-&-Permissions) for the full plugin command list.

* `/points give <name> <amount>` - Give coins to a player.
* `/points take <name> <amount>` - Remove coins from a player.

### Shop Prices

The shop prices can be edited in: `/plugins/EconomyShopGUI/shops.yml`

### Default Donator Rank Perks (For Tebex):&#x20;

_These can be changed, but this is what is set by default._

#### VIP:

* VIP prefix in chat & Tablist
* 2x Level XP Multiplier
* 5 Coins as a Daily Reward (Default: 3)
* Access to /ptime
* Access to /spectate

#### Pro:

* All perks from VIP Tier
* PRO prefix in chat & Tablist
* 2x Concurrent Active Quests
* 8 Coins as a Daily Reward (Default: 3)
* Access to /pweather

#### MVP:

* All perks from Pro Tier
* MVP prefix in chat & Tablist
* 10 Coins as a Daily Reward (Default: 3)
* Access to /nick

#### Elite:

* All perks from MVP Tier
* ELITE prefix in chat & Tablist
* 3x Concurrent Active Quests
* 12 Coins as a Daily Reward (Default: 3)
* Access to /invsee

#### Immortal:

* All perks from Elite Tier
* IMMORTAL prefix in chat & Tablist
* 15 Coins as a Daily Reward (Default: 3)
* Access to /heal \[10m Cooldown]
