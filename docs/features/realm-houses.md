# Traitors and the houses of a realm

In the base game a kingdom is as strong as the number of its houses, and a house only ever disappears. Kingdoms Alive lets a crown punish the houses that rose against it, raise new houses when it has more land than lords, and let lords go when it has more lords than land.

## After a civil war the crown wins

### The leader of the rising

The head of the house that led the plot is **put to death**. An AI ruler nearly always does it; a merciful one may spare the life. If you are the ruler, a window asks you: *"Put him to death"* or *"Spare his life"*. The sentence is carried out once the leader is in the crown's hands or free in the realm, never in the middle of a battle. If he flees abroad with his house, the sentence lapses.

If **you** led the rising and lost, the same awaits you: you are brought before the ruler and, unless the ruler spares you, executed. Your heir takes over your house as after any death in the game; with no heir, the campaign ends.

His house is not banished: it comes back to the realm with its towns and castles, under its new head, and is marked as traitor like the others.

### Houses marked as traitors

Every rebel house that comes back is marked as traitor for **60 days**. While the mark lasts, the ruler may judge it **by decree**: no vote of the council, no influence spent, and the rest of the realm does not hold it against the ruler.

- **Pardon**: the house keeps everything and its head is grateful.
- **Take a town or castle**, or **all of them**: they go before the council to be granted anew (or to a new house, below). The house stays in the realm and holds a grievance against the crown.
- **Banish**: like an expulsion by the council, but with no vote and no influence to spend: its towns and castles go before the council to be granted anew and the house leaves the realm with nothing. Its head, and its kin and friends among the realm's houses, think less of the ruler, though less than the lords who vote an expulsion. If no other kingdom takes it in, it fades away within a month, as any house without land or kingdom does in the base game.

The house may **refuse** the judgment and break with the realm, holding its fiefs by the sword, by the same odds as when a fief is taken from it (its character and how it gets on with the ruler; banishment is refused more readily, the loss of one fief less). If it bows and the sentence is carried out, its kin and friends among the realm's houses think a little less of the ruler.

As ruler, a window asks you about each house when the war ends; choose *"Not yet"* to decide later, then speak to the head of the house: *"Your house rose against the crown. Hear my judgment."* You can also banish a marked house from the **Clans** tab of the kingdom screen: while the mark lasts, its **Expel** button reads *Banish*, costs no influence and needs no vote.

An AI ruler judges each house the day after the war, by its character: a merciful one pardons more often, a cruel one takes everything; it banishes only now and then, and only when its realm has houses to spare. If your house rose and the AI ruler judges it, a herald brings the sentence: bow to it, or defy the crown.

## New houses

When an AI kingdom has a town or castle to share out (taken in a war, taken from a traitor, or left by a house expelled or gone; never a fief voted away from a house, nor one you took) and holds many more fiefs than houses to hold them, its ruler **raises a new house** and grants it that fief instead of putting it to the vote: *"{Ruler} has raised {Lord} to the nobility of {Kingdom}. The new house of the {Clan} holds {Fief}."*

- It happens when the kingdom holds more than **2.2** towns and castles per house, counting the one to share out (at the start of a campaign a kingdom holds about 1.6, so a balanced map rarely sees one). A kingdom with fewer than **5** houses always raises one with its next fief.
- Every new house makes the next one harder: each house needs its own share of land, and over 11 houses the mark also rises by **0.3** for each house. A kingdom of 9 houses needs 20 fiefs for one more; one of 11 houses, 25; one of 13 houses, 37; one of 15 houses, 52.
- At most one new house every **30** days per kingdom, and never during a civil war.
- The house is born from nothing, as in the game's own rebellions: three lords of the kingdom's culture, one of them its head, at **clan tier 3** (two parties), with some silver to raise its men.

Your own kingdom is left to you: as in the base game, you make a new house by granting a fief to a companion.

## A kingdom takes in a house only with land for it

An AI kingdom does not take in a noble house (sellswords are not affected) if, with it, it would hold fewer than **1.2** towns and castles per house. A banished house, or one cut loose when its kingdom falls, finds a new kingdom only where there is land to spare; otherwise it fades away.

## Knights of a house

A rich AI house with at least one town or castle, and fewer grown lords than the parties its tier allows, takes a **knight** into its service: a new lord of its culture who leads one of its parties. At most one every 30 days and three per house.

A knight is never the heir of the house and never weds. When the last of the blood dies, the house dies out as in the base game, and its knights with it.

## Too many lords for the land

An AI kingdom with **12 houses or more** and fewer towns and castles than houses lets one landless house go at a time, at most one every 30 days: *"There is no land in {Kingdom} for every lord who serves it. The {Clan} have taken their leave of {Ruler} to seek their fortune elsewhere."* The house that leaves is a landless one: first one of another culture than the kingdom's, then the one of the lowest clan tier, and between equals the one that likes the ruler least; never the ruler's, yours, a sellsword, or one in a plot, a faction or a feud. It leaves in peace and seeks another kingdom. Houses that leave of their own will (going over to another kingdom, rising) are another matter and can take a kingdom below that.

## A house expelled by the council

When the council votes a house out of a kingdom (the game's **Expel**), its towns and castles go before the council to be granted anew, as in the base game and as a banished traitor's do. The house may refuse, as a banished traitor may: it breaks with the realm and holds its towns and castles by the sword, by the same odds as a banishment. A house with no town or castle cannot refuse, nor one in a plot, nor the ruling house, nor mercenaries, nor a house whose refusal would leave the realm with no other fief, nor one riding in your army (it is simply expelled); neither does yours. Only you ever put an Expel to the council: the AI never proposes one.

## Turn it off

In the [settings file](../settings.md), set to `false`:

- `CrownWinsExecutesLeaderEnabled`: the leader of a failed rising is not put to death; his house comes back like the others;
- `TraitorsEnabled`: no houses marked as traitors;
- `RealmJoinNeedsLandEnabled`: AI kingdoms take in houses as in the base game;
- `RealmNewHousesEnabled`: no new houses;
- `HouseKnightsEnabled`: no knights;
- `RealmShedHousesEnabled`: no kingdom lets a house go;
- `ExpelRefuseEnabled`: a house expelled by the council always goes.
