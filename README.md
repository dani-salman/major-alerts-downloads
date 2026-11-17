# Major Alerts for WoW Forever

Nine addons for World of Warcraft: Forever, and a small program that installs them and keeps them up to date. One minimap button opens a menu of all of them (`/major`).

| Addon | What it does | In game |
|---|---|---|
| Major Bag Alert | Clears your bags: quest items you don't need, your cheapest junk | `/mba` |
| Major Quest Alert | Your quest item at its objective, and a button that targets quest mobs | `/mqa` |
| Major Buff Alert | Warns before Well Fed, elixirs or your sleeping bag buff run out, and flashes when your gathering tracking is off | `/mbf` |
| Major Professional Alert | Recipe costs and profit, the cheapest way to level, buying it all at the auction house | `/mpa` |
| Major Upgrade Alert | How much of an upgrade every item is for your class and talents | `/mua` |
| Major Investment Alert | What's worth buying at the auction house now to sell later, and why | `/mia` |
| Major Blacklist Alert | A blacklist shared by everyone with the addon, so you're warned before you group | `/mbl` |
| Major Attune Alert | Which dungeons and raids you're not attuned to, with an arrow to follow | `/maa` |
| Major Mob Alert | In dungeons: who to kill first and why, and one key that marks the pull | `/mma` |

## Install (Windows)

1. Download **[MajorAlertsUpdater.exe](https://github.com/dani-salman/major-alerts-downloads/releases/latest/download/MajorAlertsUpdater.exe)**.
2. Open it. Windows will probably show "Windows protected your PC", because the program is new and isn't signed by a company. Click **More info**, then **Run anyway**.
3. Click **Install**. It finds your WoW Forever folder by itself. If it can't, click **Change...** and pick your World of Warcraft folder.
4. Start WoW Forever. On the character screen, click **AddOns** and check the Major addons are ticked. If they're greyed out, tick "Load out of date AddOns".

Leave **Keep my addons up to date automatically** ticked and that's the last time you do anything. About once an hour it checks for a new version and installs it, with one small notification when an update has gone in. If WoW is open at the time, type `/reload` in game to load it.

## What it touches on your PC

- The `Major...` folders in `World of Warcraft\_forever_\Interface\AddOns`. Nothing else in there, and never your saved settings.
- Its own folder, `%LOCALAPPDATA%\MajorAlertsUpdater` (a copy of the program, a small settings file and a log).
- One Windows scheduled task called "Major Alerts Updater", and a Start menu shortcut with the same name.

It doesn't need administrator rights, and it only ever downloads from this page.

## Turning it off

Open **Major Alerts Updater** from the Start menu and untick **Keep my addons up to date automatically**. That removes the scheduled task. To remove every trace, also delete the folder above and the Start menu shortcut.

The addons themselves stay until you delete their folders, or untick them in the game's AddOns list.

## Without the program (or on a Mac)

Download **[MajorAlerts.zip](https://github.com/dani-salman/major-alerts-downloads/releases/latest/download/MajorAlerts.zip)** and unzip its nine folders into `World of Warcraft/_forever_/Interface/AddOns`. The zip also has a README with everything each addon does. You'll need to do this again for each update.

## If something goes wrong

- **"WoW Forever wasn't found":** click **Change...** and pick the World of Warcraft folder Battle.net installed the game into (it has a `_forever_` folder inside).
- **"Couldn't check for updates":** check your internet connection and click **Try again**.
- **The addons don't show in game:** close WoW completely and start it again.
- Anything else: send the file `%LOCALAPPDATA%\MajorAlertsUpdater\updater.log` to whoever gave you this link.
