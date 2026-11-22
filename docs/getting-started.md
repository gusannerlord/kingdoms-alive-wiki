# Getting started

## Requirements
- Mount & Blade II: Bannerlord **1.5.7**, or **1.4.8** (the default Steam branch), with or without the War Sails expansion. Each has its own main file on the mod's Nexus page: download the one for your game.
- [Harmony](https://www.nexusmods.com/mountandblade2bannerlord/mods/2006), loaded first in the launcher, above the game's own modules (Native, SandBox Core, SandBox...).
- [UIExtenderEx](https://www.nexusmods.com/mountandblade2bannerlord/mods/2102), loaded right below Harmony, also above the game's own modules. Kingdoms Alive adds its tabs, pages and lines to the game's own screens through it instead of replacing those screens, so other mods that add to the same screens (the encyclopedia, the clan and kingdom screens) work beside it.

!!! note "Playing on 1.4.8?"
    Kingdoms Alive is made for **1.4.8** again, and needs Harmony and UIExtenderEx there too. A few things differ there (see [Compatibility](#compatibility)): the game's 1.4.8 has no blood feuds, and lords riding to relieve a siege keep the game's own waiting. If you come from Kingdoms Alive 2.2.0, the last version for 1.4.8 until now, read [Updating](#updating) first.

## Installing
1. Install Harmony and UIExtenderEx.
2. If an older version of the mod is in your **Modules** folder, **delete its CampaignImprovements folder first** (see [Updating](#updating)).
3. Download the main file for your game (1.5.7, or 1.4.8) and extract its **CampaignImprovements** folder into your game's **Modules** folder, for example:
   `C:\Program Files (x86)\Steam\steamapps\common\Mount & Blade II Bannerlord\Modules`
4. If Windows blocks the file: right-click `Modules\CampaignImprovements\bin\Win64_Shipping_Client\CampaignImprovements.dll`, choose **Properties** and tick **Unblock**.
5. Open the launcher, go to the **Mods** tab and enable **Kingdoms Alive - Campaign and Diplomacy Overhaul**. The order: Harmony first, UIExtenderEx right below it, both above the game's own modules (Native, SandBox Core, SandBox...); Kingdoms Alive below the game's modules.

!!! note "Why is the folder called CampaignImprovements?"
    That was the mod's first name. The folder and the settings file keep it so that updates and saves keep working.

## Translations { #translations }
Kingdoms Alive can be played in **Español (LA)**, **Português (BR)**, **Русский**, **Türkçe** and **简体中文**. Each language is a small optional download of its own, in the files of the mod's Nexus page.

1. Download the file for your language, with **the same version as your Kingdoms Alive**. The same file serves on 1.5.7 and on 1.4.8.
2. Extract its folder (for example **KingdomsAliveSP**) into the same **Modules** folder, next to **CampaignImprovements**.
3. In the launcher, enable it (for example **Kingdoms Alive - Español (LA)**) **below** Kingdoms Alive.
4. Play with the game set to that language.

!!! note
    The translations were made by AI and reviewed by AI, and have not yet been read through by native speakers. The settings of the mod in Mod Configuration Menu are translated too, from the first start; some numbers and a few phrases built by the code stay in English. A language file from an older version of the mod makes the launcher warn you, and the newer texts show in English: update it with the mod.

## Updating { #updating }
**Delete the old CampaignImprovements folder** in **Modules**, then extract the new one (and the same with your language folder, if you use one). Extracting over the old folder leaves files of the old version behind, and the game would show some of the mod's screens twice; if the mod finds such files, a red message on the game's main menu tells you so. Your campaign carries on, and your settings file is kept: it lives in your Documents folder, not in the mod's. New switches are added to your settings file with their default values (almost all on), and switches of features that are gone are dropped from it.

If you use **Arms of the Faithful**, the optional add-on that gives the warriors of the faiths their arms and colours, update it with Kingdoms Alive, taking the file for your game (on 1.4.8 the Order of Paravenos has no tabards).

!!! note "Loading a 2.2.0 campaign"
    This is for a campaign from 2.2.0, the last version for 1.4.8 until now, loaded in this one. If you play on 1.4.8, install [UIExtenderEx](#requirements) first: Kingdoms Alive needs it since then. Keep a copy of your save first. Then:

    - Every realm keeps the law of succession it has, and that law is its custom: nobody resents it. (In a new campaign Vlandia starts under Salic Primogeniture; in yours it keeps Primogeniture.)
    - Every realm gets a law of each group of the [laws of the crown](features/crown-laws.md): **Autonomous Vassals** where High Crown Authority is not law, and **No Tax Obligation** where nothing is owed. The realms of the Empire hold High Crown Authority as their custom.
    - The goodwill a house had from being named to the court, and the ill will from being put out of it, stay as they were; from now on an office warms a house only while it holds it.

## New or existing campaign?

!!! warning "Start a new campaign with the mod, and keep it to the end"
    The mod is best played from the first day of a campaign, and it is **not meant to be removed halfway**. Taking it out of a campaign in progress can break that save.

- It can be added to a campaign in progress, and everything starts working from the day you load it, but a new campaign is the way it is meant to be played.
- Some features build up over time (tension between kingdoms, the grievances of the lords, plots, the courts of AI rulers, vassal realms), so give them a few weeks of game time.
- Two of the biggest changes are on from the start, and you will feel them from your first days: [Smarter warlords](features/command-your-armies.md#smarter-warlords-on-by-default), AI lords and armies who see as you do and wage war more wisely, and [recruitment by the land](features/recruitment.md), where men come from the villages, towns and castles of their lord and are missed there, and veterans are made, not bought. Both can be turned off in the game's options or in the [settings](settings.md).

## Removing the mod
Do not remove it from a campaign you want to keep playing. If you do, keep a copy of your save first: the campaign may no longer load, or may misbehave. Things the mod had under way (an envoy or companion away on an errand and its quest log entry, a feast or hunt, a civil war, a court, a vassal realm) stay as they were at that moment or are lost. Some of these are kept in your save as quests of the mod's own (your rival, your mercenary service and its tasks, anyone you sent away), and the Unsworn troops are the mod's own too: without the mod, a save that holds them may not load.

## Compatibility
- **Not compatible with the "Diplomacy" mod** or other mods that replace how AI kingdoms decide on war and peace. Despite the name, this is not an add-on for it.
- If a game update changes the game's war formula, the mod's war scoring switches itself off instead of breaking.
- The launcher may show a version warning on game versions other than 1.5.7 and 1.4.8. The mod has not been tested there.
- **On 1.4.8** the game has no blood feuds: your [rival](features/rival.md)'s house cannot be paid off at a ransom broker, and a [hunting accident](features/hunts.md) that is found out costs relation and Honor instead. Lords riding to relieve a siege do not [wait out of the besiegers' reach](features/command-your-armies.md): they keep the game's own waiting.

## Story mode, sandbox, normal or fast mode
Everything works in all of them. Most testing was done in sandbox campaigns in fast mode. While a story quest is under way, you cannot raise a rebellion or ride with one: the option is greyed out and tells you why. Leaving your kingdom would break the quest.
