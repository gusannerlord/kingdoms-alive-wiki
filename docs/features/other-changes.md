# Other changes

Smaller changes to the campaign: a wide demesne breeds corruption, sieges give relief armies time to arrive, AI armies are forged in war rather than in idle peace, and good weapons and armour cost something a player can actually save up for.

## Corruption in a wide demesne
The base game knows corruption only from low security or loyalty. With the mod, a house that holds **two or more towns and castles** also loses part of their taxes, and of their villages', to the people who run them: **5%** with two, **2.5% more** for each one beyond, **30%** at most (from twelve). It shows as **"Corruption, too many holdings to watch"** in each fief's tax breakdown.

| Towns and castles | Lost from each |
|---|---|
| 1 | nothing |
| 2 | 5% |
| 4 | 10% |
| 6 | 15% |
| 10 | 25% |
| 12 or more | 30% |

A **governor** cuts it in his own fief by his Steward: half at 75, none at all at **150**. It is the same for every house, AI or yours (AI houses put their idle lords in as governors as in the base game).

## Longer siege preparations
**Siege Preparations** (the first thing a siege camp builds, before any siege engine and before it can assault) take **half as long again** (1.5 times as long), for you and for the AI, in any campaign.

In the base game, preparations take roughly 48 days divided by the square root of the healthy besiegers, before Engineering bonuses:

| Besiegers | Base game | With the mod |
|---|---|---|
| 100 | about 4.8 days | about 7.2 days |
| 400 | about 2.4 days | about 3.6 days |
| 1,000 | about 1.5 days | about 2.3 days |

What this means in play:

- Defenders have more time to build their own engines and for help to arrive.
- Besiegers spend more food and wages before they can assault, so more sieges are lifted.
- When you besiege, you wait longer too. If you send your troops in without fighting yourself and that assault ends with no winner, the base game resets your preparations, and rebuilding them also takes longer.
- The tooltip still shows the same "Build Cost" (48), but the progress bar fills at two thirds of the speed.
- Only the preparations change. Siege engines built afterwards, and everything the defenders build, are as in the base game.

### AI assault patience
In the base game, the AI starts to accept worse odds for an assault after 96 hours of siege, counted from the start. With longer preparations, small and medium armies would finish them with that patience already spent and storm the walls too soon. The mod does not count the extra preparation time, so after its preparations the AI is about as patient as in the base game.

In a 249-day test campaign (with the earlier doubled preparations), AI armies first assaulted at a median of 81 hours into the siege, always with 2 to 4 siege engines built: no rushed assaults.

## Less free training for AI troops in peace
In the base game, troops in AI lords' parties gain experience every day without fighting: 15 + 3 x tier per troop in a clan leader's party, 10 + 2 x tier in other lords' parties. A recruit reaches tier 5 on its own in about 135 days with a clan leader and about 205 days with other lords.

With the mod, once a kingdom has had **no war with another kingdom for more than 10 days**, its lords' troops get only **a quarter** of that free experience until the next war. Armies are built in war, not in long breaks between them.

- Applies to the AI lords of every kingdom, including the vassals and mercenaries of your own kingdom.
- Your own clan's parties, and parties in an army you lead, get no free experience in the base game either, so nothing changes for them.
- Clans without a kingdom are untouched. Wars against rebels or clans without a kingdom do not count as war.
- Experience from battles and from perks is untouched.
- With the usual length of peace breaks, kingdoms lose roughly 6 to 20% of their free experience overall. A recruit who spends a 40-day peace in a lord's party no longer reaches tier 2 by itself.

## Weapon and armour prices
In the base game, the best weapons and armour cost hundreds of thousands of denars. With the mod they cost far less when **you** buy or sell them.

- Only your trades change. AI lords, caravans and workshops trade at base-game prices, so the economy of the world does not change.
- Loot, tournament prizes, shop stock and smithing are untouched. The "value" shown outside trading is the base game's.
- Anything up to 1,000 denars keeps its price. Above that, the dearer the item, the bigger the cut.
- **Selling** expensive gear also pays less, since prices are lower both ways.
- Quality still matters as in the base game (legendary x1.8 ... rusty x0.3), and so do the town's market and buying in an enemy town.
- Applies to armour (horse armour included) and weapons (shields, bows and ammunition included). Banners and horses are untouched.

### Armour
Armour is priced by its protection: each 10 points of armour multiply the price by about 1.9, steadily across the whole range. In the base game, prices stop rising with protection above 79 points and the best armours are ranked mostly by looks; the mod counts protection all the way up and gives looks less weight in expensive armour.

Body armour, normal quality, in a normal town (approximate buying prices):

| Armour | Total armour | Base game | With the mod |
|---|---|---|---|
| Light Padded Armor | 29 | 1,600 | 1,300 |
| Stitched Cured Leather Coat | 36 | 3,200 | 2,100 |
| Robe over Mail Shirt | 49 | 12,000 | 4,900 |
| Nordic Long Heavy Mail | 57 | 44,000 | 10,700 |
| Norse Chainmail | 63 | 90,000 | 16,100 |
| Coat Of Plates | 70 | 121,000 | 20,200 |
| Rough Brigandine | 76 | 208,000 | 28,500 |
| Reinforced Mail Shirt | 80 | 281,000 | 36,700 |
| Cataphract Lamellar Armor | 86 | 351,000 | 57,800 |
| Heavy Lamellar over Hauberk | 90 | 351,000 | 74,700 |
| Decorated Hauberk | 94 | 402,000 | 100,500 |
| Khan's Coat of Plates | 95 | 603,000 | 121,000 |

Other pieces: the **Plated Helmet with Sideguards** goes from about 221,000 to about 27,000. A full set of the best Vlandian gear, horse barding included, costs about 105,000 instead of about 580,000.

### Weapons
Weapons are cut a little less than armour:

| Base game price | 2,000 | 5,000 | 10,000 | 20,000 | 50,000 | 100,000 | 250,000 |
|---|---|---|---|---|---|---|---|
| With the mod | 1,700 | 3,300 | 5,500 | 9,200 | 18,000 | 30,000 | 60,000 |

## Turn it off
In the settings file, set the switch to `false`. See [Settings](../settings.md).

- `CorruptionEnabled`: no corruption from holding many towns and castles. Numbers you can change: `CorruptionFromFiefs` (2), `CorruptionBase` (0.05), `CorruptionPerFief` (0.025), `CorruptionMax` (0.3), `CorruptionStewardForNone` (150).
- `SiegePreparationEnabled`: siege preparations take as long as in the base game.
- `SiegePatienceIgnoresAddedPreparationTime`: the AI's assault patience counts the extra preparation time (only matters while longer preparations are on).
- `AiPeaceTrainingEnabled`: AI troops gain their full free experience in peace.
- `GearPricesEnabled`: base-game prices for weapons and armour.
- `ApplyToWeapons`: when `false`, only armour gets cheaper.
