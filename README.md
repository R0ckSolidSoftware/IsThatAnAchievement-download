# Is That An Achievement?

**Hypixel SkyBlock never gave you enough achievements. So here are 100+ more.**

IsThatAnAchievement (ITAA) is a client-side Fabric mod that adds custom, multi-tier SkyBlock achievements with silly titles, advancement-style toasts and a proper in-game achievements screen. Mine some Mithril, get "Gourmand in Training". Spot enough Golden Goblins, become a "Goblin Slayer". Visit the Rift, get "Rifted". It's SkyBlock, but somebody is finally keeping score.

No API key. No account linking. No setup.

## What you get

- **100+ achievements** across Mining, Combat, Farming, Fishing, Pets, Dungeons, Slayer, Exploration and Misc, most with several tiers.
- **Rarities** from Common up to Legendary, with a coloured chip and tint so you can spot the nasty grinds.
- **Toasts and chat messages** the moment a tier unlocks.
- **A clean achievements screen** with categories, search, progress bars and a tooltip for every tier. Press `K` or type `/ach`.
- **Hidden achievements** that stay `???` until you find them.
- **Stats per SkyBlock profile**, so your Ironman and your co-op don't get mixed up.
- **Updates in-game.** The mod tells you when a new version is out and installs it when you close the game, but only after you click.

## Install

You need Minecraft **26.2**, [Fabric Loader](https://fabricmc.net/use/) **0.19.5 or newer**, Fabric API, and Java 25.

1. Grab the latest `.jar` from [**Releases**](../../releases/latest).
2. Drop it into your `mods` folder next to Fabric API.
3. Join Hypixel SkyBlock, press **`K`**, and start collecting.

## How it works (the short version)

The mod only reads what your client already sees: chat messages, menus you open, the tab list and sidebar, nearby mobs and block updates. It never touches the Hypixel API and sends nothing about you anywhere; the only network request is the update check, which asks this repository for the latest release.

For the big lifetime numbers it reads the in-game menus. Open these once to sync your progress, and the mod keeps counting from there:

`/bestiary` · `/collection` · `/pets` · `/skills` · `/hotm`

Type `/ach sync` any time for a reminder. Nothing is tracked until you've joined SkyBlock, because the mod needs to know which profile you're on.

## Commands

| Command | What it does |
|---|---|
| `K` or `/ach` | Open the achievements screen (`/itaa` works too) |
| `/ach list [category]` | Every achievement and your progress |
| `/ach stats [filter]` | The raw numbers the mod has recorded |
| `/ach sync` | Which menus to open to refresh your progress |
| `/ach update` | Download an update the mod found |
| `/ach reset all` | Wipe stats and unlocks for the current profile |

## Settings

Everything lives in `config/isthatanachievement/config.json`: toasts on or off, chat announcements, a small HUD showing your next unlock, screen scale, and whether to check for updates.

## Something not counting?

Some chat messages and menus haven't been confirmed in the real game yet, and those achievements show a `! UNTESTED` tag. If something doesn't count, [open an issue](../../issues) and say what you did.

---

*Made by rasmushk. Not affiliated with Hypixel or Mojang. This repository only hosts release builds.*
