# Mercenary contracts and the Unsworn

The ruler who pays you now puts you to work: a messenger stops you on the road with a task, and a good record opens the way to vassalage. The **Unsworn**, a new company of sellswords who answer to no crown, can also be hired in the taverns.

## How tasks arrive

- Only while your house serves a kingdom **as mercenaries**.
- A messenger of the ruler finds you on the map. The first comes about **5 days** after you sign. After that, one every **15 to 25 days**, counted from the last messenger, and never sooner than **5 days** after your last task ended.
- **One task at a time.** No messenger comes while a task is under way.
- The messenger waits until you are out on the map and free: not while you are a prisoner, at sea, in a town, castle or village, in a battle, a siege or a menu. If they cannot reach you for **5 days**, they give up, with no penalty. The days you spend riding in someone's army do not count towards those 5.
- If there is nothing to ask of you nearby, the ruler looks again **3 days** later.
- If the ruler is a prisoner, their house speaks for them: see [The ruler's rescue](#the-rulers-rescue).

## The messenger's offer

The messenger describes the task, its deadline and reward. Answer **"Tell her/him my company is on its way. It will be done."** (it goes into your quest journal, with the places marked on your map) or **"Tell her/him my men are in no state for this. I cannot take it on."** (a refusal). Close the talk without answering and they come back 12 hours later.

## "In the service of the crown"

The first messenger of each service also tells you the deal and opens a quest in your journal: **"In the service of the crown of {KINGDOM}"**. It has two bars:

- **Contracts fulfilled**: **0 of 5**.
- **House standing**: your clan must be **tier 2** or higher.

Each task given, fulfilled, failed or refused gets a line in it. With **5 tasks fulfilled** and your clan at tier 2, the quest is complete and the ruler makes you **the game's own offer of vassalage** (or tells you to go and ask): go and speak with them in person to swear. If you swear to that ruler some other way first, the quest still ends well.

Vassalage comes without land: a sworn sellsword starts as a lord of the realm with no fief of their own, and earns one the way any vassal does.

## The tasks

| Task | Deadline | Reward |
|---|---|---|
| Raid an enemy territory | 60 days | 5,000 denars, 5 renown, 20 influence, honor, +10 with the ruler |
| Escort a caravan | 30 days | 2,000 denars, 3 renown, +5 with the ruler |
| Guard a border village | 30 days | 3,000 denars, 3 renown, +5 with the ruler |
| Rescue a lord | 50 days | 8,000 denars (12,000 for one of the ruler's house), 5 renown, +3 with the ruler, +5 with the lord |

### Raid an enemy territory
The game's own **"Raid an Enemy Territory"** quest, given by messenger: burn **one village** of the enemy kingdom whose villages lie nearest to you (the game's own quest asks three; here one is enough, for a third of its gold). The reward is paid the moment it burns. A village burnt in a fight as time runs out still counts. Only offered while the ruler has no other quest of their own open.

### Escort a caravan
One of the realm's caravans on the road near you, bound for a **named town** no more than about three towns' ride away. The town is marked on your map and named in your journal, and the caravan carries an arrow on your map. Ride with it and **be close by when it enters a town**, within 30 days. You are warned when you are losing sight of it.

- If it reaches its town without you, the caravan master trades there for a few hours and sets out for another town; the journal tells you which.
- If the road ahead closes (war, a siege), it turns aside or shelters in the nearest safe town and goes on later.
- If every town it could make for is closed to it, the escort lapses with no penalty.
- If an enemy destroys it, the task fails.

### Guard a border village
A village of the realm near you and close to an enemy town or castle. Keep it **in sight for 3 days in all** within 30 days, like the game's quest to scout enemy garrisons: every hour it is within your party's sight counts. A message marks each day (for example *"Another day of watch over {VILLAGE} is done (1/3)."*). If the village is looted first, it fails, unless it was looted before you could have got there: then it lapses with no penalty. Beating an enemy lord's party at or near the village fulfils it at once.

!!! note "The Unsworn tasks moved to the King's Writ"
    Clearing an Unsworn hideout and sweeping three Unsworn bands are no longer mercenary tasks: they are now contracts of [the King's Writ](kings-writ.md#the-kings-contracts), for a free man-hunter. A task of either kind already under way runs to its end as described below. With the writ's contracts turned off (`WritContractsEnabled` or `WritEnabled` set to `false`), they are mercenary tasks again.

### Clear an Unsworn hideout
Reward: 4,000 denars, 3 renown, +5 with the ruler, within 30 days. A hideout near the realm's villages, taken over by the Unsworn and marked on your map as **"Unsworn Hideout"**. Inside are **35 to 40** Unsworn on foot, more as your campaign advances, and no common bandits. Attack it as any hideout, or use "Send troops". The last fight is against the **Unsworn Captain**, the hideout's own chief, with the game's usual duel offer.

### Sweep of the Unsworn bands
Reward: 2,000 denars, 3 renown, +5 with the ruler. **Three bands** of Unsworn, each of **20 to 40** men (more as your campaign advances) and led by a veteran, roam around villages of the realm away from you. Each has an arrow on the edge of the map pointing to it. Beat all three within 50 days. They ride a little faster than a lord's party, will not talk or surrender, and come after you if you are near and they are clearly stronger (more than 1.2 times your strength). The lords of the map leave them alone, so it is up to you.

### Rescue a lord
A lord of the realm held in the **dungeon of an enemy town** within a few days' ride (never a castle, which a sellsword cannot slip into, and never one carried by a party). One of the ruler's own house is picked first, then the nearest. Where they are held is marked on the map. Free them:

- with the game's own **prison break** in that town: the full reward;
- by **taking the town** in an assault you lead: the full reward;
- by being **among the besiegers** when the realm's host takes it, led by someone else (in the camp, in the army or in the assault): **40% of the reward**;
- if the enemy moves them meanwhile, by **beating the party that carries them** (the full reward if you lead the fight, 40% if someone else does). You are told where they were taken, and the new place or party is marked.

While the task is under way, the lord almost never escapes on their own (about 1 in 8 over the 50 days, instead of nearly always in the base game). If they go free some other way (ransom, peace, someone else) or die, the task lapses with no penalty.

### The ruler's rescue
If the ruler themselves lies in the dungeon of an enemy town within a long ride of you, someone of their house sends the messenger in their place: their spouse, or failing that their eldest child, or the eldest lord of the house. Bringing the ruler home is then the only task offered. It works as a rescue of a lord of the ruler's house (12,000 denars), and the ruler pays and thanks you once free. If the ruler is held somewhere you cannot reach, or carried by a party, the house waits and looks again every few days.

## How the task is chosen

Each task has its weight in the draw, and **the kind you were given last is much less likely to come again** next time.

- **In war**, a lord to rescue comes first: when there is one, the rescue weighs 4 times as much as a raid (8 times for one of the ruler's house). The caravan escort and the border village weigh a little more than a raid each.
- **In peace**, there are no raids, border villages or rescues: you get the caravan escort.

## Failing and refusing

A refusal or a failed task (time ran out, the caravan lost, the village looted):

- your **mercenary pay is cut by half for 20 days**;
- **-2 relation** with the ruler, but never more than **-5** in all with the same ruler;
- **three in a row** and the ruler ends your contract: *"A rider brings a sealed letter: the crown of {KINGDOM} no longer wants your swords. Your contract is ended, and you are free to sell them elsewhere."* You are warned after the second. Any fulfilled task resets the count.

A task **lapses**, with no penalty, through no fault of yours: you were a prisoner when time ran out, the ruler is no longer on the throne, the caravan has nowhere left to go, or the village changes hands.

## The Unsworn troop tree

Sellswords of no culture. Their names in the party screen:

| Tier | Troop | Upgrades to |
|---|---|---|
| 1 | Unsworn Recruit | Footman, or Outrider (needs a horse) |
| 2 | Unsworn Footman | Wilder or Trained Bowman |
| 2 | Unsworn Outrider | Raider or Horse Archer |
| 3 | Unsworn Wilder | Warmonger or Hellion |
| 3 | Unsworn Trained Bowman | Longbowman |
| 3 | Unsworn Raider | Battle Rider (needs a war horse) |
| 3 | Unsworn Horse Archer | Mounted Master Archer (needs a war horse) |
| 5 | Unsworn Warmonger, Hellion, Longbowman, Battle Rider, Mounted Master Archer | — |

Where to get them:

- **Taverns.** When a town's tavern changes the mercenaries it offers (every two days, as in the base game), about **1 time in 5** they are Unsworn instead, mostly of the lower tiers. You hire them from the tavern's mercenary like any other.
- AI lords and caravans hire them from the same taverns, so you will also meet Unsworn in other parties.
- **Prisoners.** Like any regular troop of **tier 2 or higher**: every Unsworn except the Recruit.

!!! tip
    Need hundreds of men at once, for a few weeks? Hire a whole company instead: see [Companies for hire](free-companies.md).

## Turn it off
In the settings file, set the switch to `false`. See [Settings](../settings.md).

- `MercContractsEnabled`: no more tasks by messenger, and no "In the service of the crown" quest. A task under way still ends as usual.
- `MercContractRaid`: no raid tasks.
- `MercContractProtect`: no caravan escorts or border villages to guard.
- `MercContractUnswornHideout`, `MercContractUnswornSweep`: only matter with the King's Writ contracts turned off (see above).
- `MercContractRescue`: no rescues of lords.
- `MercContractRescueRuler`: no rescue of a captured ruler; no task comes while the ruler is a prisoner.
- `MercContractVassalPath`: no "In the service of the crown" quest, no vassalage offer; the tasks go on.
- `UnswornTroopsEnabled`: taverns no longer offer the Unsworn, and the two Unsworn tasks are not given.
- `FixMercHideoutMenEnabled`: the hideouts of the Unsworn and of [your rival](rival.md) hold only as many men as the game's own hideouts.
