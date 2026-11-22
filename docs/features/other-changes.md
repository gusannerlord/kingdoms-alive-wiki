# Other changes

Smaller changes to the campaign: a wide demesne breeds corruption, sieges give relief armies time to arrive, AI armies are forged in war rather than in idle peace, and good weapons and armour cost something a player can actually save up for.

## Corruption in a wide demesne
The base game knows corruption only from low security or loyalty. With the mod, a house that holds **two or more towns and castles** also loses part of their taxes, and of their villages', to the people who run them: a little with two, more with each one beyond, up to a heavy share for the greatest houses. It shows as **"Corruption, too many holdings to watch"** in each fief's tax breakdown.

A **governor** cuts it in his own fief by his Steward: a good steward cuts it, a master of the craft stops it altogether. It is the same for every house, AI or yours (AI houses put their idle lords in as governors as in the base game).

### In the Fiefs tab { #in-the-fiefs-tab }
The **Fiefs** tab of the clan screen shows each town and castle's current corruption as a **Corruption** row, wherever there is some. Hover over it for the reason in words, and whether its governor's stewardship is cutting it.

## Longer siege preparations
**Siege Preparations** (the first thing a siege camp builds, before any siege engine and before it can assault) take **longer**, for you and for the AI, in any campaign. As in the base game, a bigger camp finishes them sooner.

What this means in play:

- Defenders have more time to build their own engines and for help to arrive.
- Besiegers spend more food and wages before they can assault, so more sieges are lifted.
- When you besiege, you wait longer too. If you send your troops in without fighting yourself and that assault ends with no winner, the base game resets your preparations, and rebuilding them also takes longer.
- The tooltip still shows the game's own "Build Cost", but the progress bar fills more slowly.
- Only the preparations change. Siege engines built afterwards, and everything the defenders build, are as in the base game.

### AI assault patience
In the base game, the AI starts to accept worse odds for an assault after some days of siege, counted from the start. With longer preparations, small and medium armies would finish them with that patience already spent and storm the walls too soon. The mod does not count the extra preparation time, so after its preparations the AI is about as patient as in the base game: AI armies storm the walls with their siege engines built, not in a rush.

## Less free training for AI troops in peace
In the base game, troops in AI lords' parties gain experience every day without fighting, more in a clan leader's party, so that a recruit becomes a veteran on his own in a few months of idling.

With the mod, once a kingdom has gone some days without a war against another kingdom, its lords' troops get only a small part of that free experience until the next war. Armies are built in war, not in long breaks between them.

- Applies to the AI lords of every kingdom, including the vassals and mercenaries of your own kingdom.
- Your own clan's parties, and parties in an army you lead, get no free experience in the base game either, so nothing changes for them.
- Clans without a kingdom are untouched. Wars against rebels or clans without a kingdom do not count as war.
- Experience from battles and from perks is untouched.
- A recruit who spends a peace in a lord's party no longer rises in rank by himself.

Under the [recruitment by the land](recruitment.md#wages-and-rising-in-rank), every soldier also needs more experience, and more gold, to rise in rank, much more for the highest ranks.

## Weapon and armour prices
In the base game, the best weapons and armour cost a fortune no player could ever save. With the mod they cost far less when **you** buy or sell them.

- Only your trades change. AI lords, caravans and workshops trade at base-game prices, so the economy of the world does not change.
- Loot, tournament prizes, shop stock and smithing are untouched. The "value" shown outside trading is the base game's.
- Cheap pieces keep their price. Above that, the dearer the item, the bigger the cut.
- **Selling** expensive gear also pays less, since prices are lower both ways.
- Quality still matters as in the base game (legendary pieces dearer, rusty ones cheaper), and so do the town's market and buying in an enemy town.
- Applies to armour (horse armour included) and weapons (shields, bows and ammunition included). Banners and horses are untouched.

### Armour
Armour is priced by its protection, rising steadily across the whole range. In the base game, prices stop following protection for the heaviest armours, which are ranked mostly by looks; the mod counts protection all the way up and gives looks less weight in expensive armour. Light padding costs about what it did; a good mail shirt a fraction of its old price; the finest lamellar and plate, once out of reach, become a prize a successful captain can buy. A full set of the best Vlandian gear, horse barding included, costs a fraction of what it did.

### Weapons
Weapons are cut a little less than armour, and the dearer the weapon, the more it is cut.

## Turn it off
In the settings file, set the switch to `false`. See [Settings](../settings.md).

- `CorruptionEnabled`: no corruption from holding many towns and castles.
- `SiegePreparationEnabled`: siege preparations take as long as in the base game.
- `SiegePatienceIgnoresAddedPreparationTime`: the AI's assault patience counts the extra preparation time (only matters while longer preparations are on).
- `AiPeaceTrainingEnabled`: AI troops gain their full free experience in peace.
- `GearPricesEnabled`: base-game prices for weapons and armour.
- `ApplyToWeapons`: when `false`, only armour gets cheaper.
