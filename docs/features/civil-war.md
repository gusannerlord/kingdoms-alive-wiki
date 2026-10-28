# Civil war

A kingdom that grows too large starts to rot from within. Its lords lose patience with the ruler, a powerful clan starts a plot, and if the plot grows strong enough it raises its banner and the realm splits in a civil war. You can join a plot, lead one, work against it, or, if you wear the crown, fight to keep it.

## When a kingdom is "too large"

The mod compares each kingdom with its fair share of the map: all the towns and castles held by kingdoms, divided by the number of kingdoms. Kingdoms already destroyed still count in that number. Kingdoms born from a rising never do, so one civil war does not make every other realm look larger.

A kingdom is **too large** once it holds **1.25 times** its fair share or more. Example: with 80 towns and castles and 8 kingdoms, the fair share is 10, so a kingdom with 13 or more is too large.

## Discontent

Every 7 days (the mod's own count, not the game's week, which is only 3 days in fast mode), in a kingdom that is too large, every clan leader loses relation with the ruler:

| Size of the kingdom | Relation lost per 7 days |
|---|---|
| 1.25 times its fair share | 0.5 (one point every two weeks) |
| between the two | rises steadily |
| 2 times or more | 1.5 |

- It reaches every vassal clan leader, **you included**. It does not reach the ruler's own clan, the ruler's close kin (parents, children, brothers and sisters, husband or wife) or mercenaries.
- **It stops at a limit that depends on the kingdom's size.** In all, it never takes more from a clan leader than:

    | Size of the kingdom | Most it takes in all |
    |---|---|
    | 1.25 times its fair share | 3 |
    | 1.3 times | 5 |
    | 1.4 times | 9 |
    | 1.5 times | 12 |
    | 1.75 times | 18 |
    | 2 times or more | 25 |

    A kingdom that keeps growing wears its lords down further, up to the new limit. One that shrinks gives back what is over its new limit, a point every 7 days. Size alone rarely turns lords against a ruler badly enough for a civil war; [quarrels between clans](clan-events.md) and other grudges do the rest.
- A [Chancellor](royal-court.md#the-offices) cuts it by up to 15%.
- It never takes anyone below **−25** with the ruler. Lords who already dislike the ruler more than that lose nothing further from it.
- Every so often you see a yellow message. As a vassal: *"{Kingdom} has grown too large to be ruled well. {ruler} has no time for lords like you any more, and your regard for your liege keeps wearing away."* As the ruler: *"The lords of {Kingdom} grumble that the realm has grown too large to be ruled well: {N} houses think less of you."*
- **Recovery:** once the kingdom is no longer too large, or while it rests after a civil war, each clan leader gets back 1 point every 7 days, up to what the discontent took and never more. That claim is lost if the ruler changes, the clan gets a new leader, or the clan leaves the kingdom.
- During a civil war nothing is lost and nothing comes back.

## How a plot starts

Every 7 days, in each kingdom that is too large, or whose ruler has a [weak claim](succession.md#what-a-claim-does), and has no plot yet, the AI clan leaders may start one. A clan leader can start a plot if:

- their clan has a **Clan Strength of 1,000 or more** (the figure shown on the clan's page in the Encyclopedia);
- their relation with the ruler is **−5 or worse** (**+5 or worse** if the ruler's claim is weak and theirs is better);
- they are not the ruler's clan or close kin, nor a mercenary, nor sworn to the crown at the moment (see below).

Each such leader has a **10% chance** a week, plus 5% for each level of Calculating and of Valor, minus 10% for each level of Honor. A plot starts only if at least one other clan would join it straight away.

A kingdom can hold **up to three plots at once**, each behind its own pretender. A house is in one plot at most, the one it leans to most, and goes over to another only if it leans to it clearly more (a house that gave its word stays where it swore). The **first plot to rise ends all the others**.

No new plot starts for **60 days** after a plot ends, nor for **100 days** after a civil war.

A [vassal realm](vassal-realms.md) never has a plot or a civil war: a plot under way dies quietly when its realm bends the knee. And no realm becomes a vassal while either side is in a civil war.

## Who joins, and why

Every 7 days, each clan leader of the kingdom weighs every plot. The ruler's own clan and close kin never join. The rest add up a score:

| What counts | Effect |
|---|---|
| Relation with the plot's leader | half of it, for or against |
| Relation with the ruler | 0.7 of it, the other way: liking the ruler holds them back, hating the ruler pushes them in |
| Honor | −8 per level |
| Valor | +3 per level |
| Calculating | only a calculating lord sides with the winner: drawn in once the plot holds more than 30% of the realm's strength, put off below that |
| How big the plot is | up to +20, as it grows toward the whole realm |
| Clan without towns or castles | +10, only while the realm is too large |
| Close kin or in-law of the plot's leader | +20 |
| Swore the [oath of fealty](royal-court.md#the-oath-to-a-new-ruler) to the current ruler | −10, for 120 days |
| Refused that oath, or let the time pass | +20, for 180 days |
| Dismissed from the [court](royal-court.md#the-offices) | up to +8, fading over about 120 days |
| The [claims](succession.md) of the plot's leader and the ruler | up to +10 when the leader's claim is the better one; up to −10 when the ruler's claim is beyond question |

A lord **joins at 25** and **leaves below 5**. Example: a lord with −20 toward the ruler (+14) and +10 toward the plotter (+5), with the plot holding 30% of the realm (+6), reaches 25 and joins.

"The realm's strength" here means the Clan Strength of all its vassal clans together, the ruler's clan included and mercenaries left out. The plot's **share** is the part of that held by its clans.

**The plot's leader recruits.** Each week an AI plot leader tries to win over one undecided lord (score between 5 and 25), the closest to joining. The odds are 15%, plus 2% for every 10 points of the leader's Charm, plus 2% for each point the lord is above 5, between 5% and 60%. At the same feast or the same [hunt](hunts.md) the odds are 1.5 times higher. A lord won over this way stays in the plot for at least 30 days. Once the plot holds 60% of the realm, the leader stops recruiting (lords may still join by themselves).

**At a hunt.** An AI plot leader who hosts a hunt likes to invite wavering lords (score between 5 and 25). On the last day of the hunt they try once to win over each wavering guest who came, with the odds above, 1.5 times higher. A member of the plot who hosts a hunt tries with each wavering guest half the time. An AI ruler who knows of the plot and hosts a hunt tries to win back each guest who is in it.

**The ruler wins lords back.** Once the plot holds 25% of the realm, an AI ruler tries each week to win back the member who is least committed. The deeper the lord is in it, the harder. A lord won back leaves the plot, gains **+5** relation with the ruler and stays loyal for at least **60 days**. If you are the ruler, this is your job (see below).

## Rumours

When a plot reaches **20%** of the realm's strength, and you are a vassal of that kingdom outside the plot, you hear: *"There is talk of a plot among the lords of {Kingdom} against {ruler}. Who is behind it, nobody will say."* If you are the ruler, it says "against you". From then on you know a plot exists, but not who leads it or who is in it.

## How a plot dies

- **It never grew:** a plot that has not reached **25%** within **60 days** comes to nothing.
- **It stalls (AI plots only):** after **120 days** without holding enough to rise (counted from its start, or from the last week it had enough), it gives up.
- **The realm shrank (AI plots only):** once the kingdom has been back below "too large" for **60 days in a row**, it ends.
- **The leader is gone:** the leader dies, is replaced at the head of the clan, leaves the kingdom, becomes a mercenary, comes to the throne, or (an AI leader) becomes close kin of the ruler, for example by marriage.
- **The leader is talked out of it** (by you, see below).

If you knew of it you see *"The plot among the lords of {Kingdom} has come to nothing."*

## The rising

An AI plot raises its banner when **all** of this is true:

- it holds **50%** of the realm's strength;
- it began at least **21 days** ago and has at least one clan besides its leader's;
- the kingdom is too large, or was within the last 14 days;
- the kingdom is **at peace with every other kingdom** (nobody rises while the realm fights a foreign war);
- at least one house of the plot holds a town or castle, and the crown keeps at least one of its own.

When it rises:

- The plot's leader founds a **new kingdom**, named *"{Clan} Pretenders"*, with their clan's culture and emblem, on a banner of its own colours, distinct from the realm it rose against (if you lead the rising, your clan keeps its own colours). It claims the throne and is at war with the crown at once.
- Every clan of the plot goes over with its towns, castles and villages, keeps its influence, and must stay at least **60 days**.
- You are told in the middle of the screen, wherever it happens: *"Civil war: {Leader} of the {Clan} has raised the banner against {ruler}, ruler of the {people}."* (or *"Civil war in your realm: ..."* in your own kingdom). If you led the rising, were in the plot or were asked whether you ride with it, you already know and get no extra notice.
- The log keeps a red line with the news and the houses that went over to the rebels.

## Winning the civil war

Each day the mod compares the two sides: the total Clan Strength of each side's vassal clans.

- **By strength:** from day **30** of the war, a side that holds **twice** the other's strength for **10 days in a row** wins.
- **By land:** a side left without a single town or castle loses at once, even before day 30.

Nothing is settled while you are in a battle or siege on either side; it waits for the fight to end.

## The outcomes

**The rebels win.** The rebel leader's clan becomes the ruling clan of the old kingdom. Every rebel house comes back into it (and must stay 60 days), and the rebel kingdom disappears. The old ruler loses **20** relation with the new one. If that ruler was you: *"You have lost the throne of {Kingdom}. {New ruler} of the {Clan} now rules; your house remains as a vassal."*

If you led the rising and win, you are told the crown of the kingdom is yours. A new ruler means a new [oath of fealty](royal-court.md#the-oath-to-a-new-ruler): the houses that stayed loyal to the old crown are much less willing to swear to the winner.

**The crown wins.** The plot's leader loses every town and castle (they go to the ruler) and is banished: an AI clan goes to another kingdom, preferably of its own culture and whose ruler it likes best, never yours. If none will do, it is left without a kingdom. The other rebel houses come back pardoned, each with **−20** relation with the ruler, and must stay 60 days.

**A negotiated peace.** From day **120** either side may offer peace. It is never automatic: the side that receives the offer must want it (if that side is a kingdom you rule, you decide). Before day 120 a peace is refused with *"Blood is still too hot for talk of peace in this civil war. Unless one side wins outright, it will be some {N} days before either will hear of it."* A peace leaves **two kingdoms**: the rebels keep what they hold, and an AI rebel kingdom drops "Pretenders" and becomes *"Realm of the {Clan}"*. A side that has already lost every town and castle cannot make peace: it has lost.

**Afterwards:** every kingdom that comes out of a civil war gets **100 days of calm**: no discontent and no new plots, while the discontent of the past slowly mends.

## Other kingdoms stay out

While a civil war lasts, other AI kingdoms are reluctant to attack either side:

- they need a much stronger reason than usual to declare war;
- they weigh each side as if half of the other side's strength stood with it;
- they never see the civil war as a chance to retake lost lands.

It is not impossible: a kingdom with a strong grievance may still attack. In the council you may hear *"they are at war among themselves, and we will not meddle in it"* or *"their rivals in the civil war would be the ones to gain"*. None of this holds back a kingdom you rule, nor an ally of one side attacking the other.

## Your part in it

Everything below needs you to lead your clan as a vassal (not a mercenary) of the kingdom, and neither you nor the lord you talk to can be a prisoner. You talk to clan leaders of your own kingdom: choose *"There is something I'd like to discuss."* and the plot options appear among the others.

### What you can say to a clan leader

| You say | When it appears | What it does |
|---|---|---|
| *"{Ruler} is leading this realm to ruin. Would you stand with me if it came to it?"* | You are neither the ruler nor the ruler's close kin, you know of no plot in the realm, and the lord is not of the ruler's clan or close kin. | Starts **your own plot** and tries to win this lord over. Greyed out if your Clan Strength is below 1,000, if the realm is in its calm after a plot or civil war (*"The lords of the realm are wary just now. It is too soon."*), or if you spoke to this lord about it too lately. If a secret plot already exists, the lord answers *"Hush. You are not the first to say so..."* and you learn that there is one. |
| *"There are those of us who mean to set this realm right. Join our cause."* | You are in a plot, your own or an AI lord's. | Persuade the lord to join. |
| *"There is a plot against {ruler}. Stay loyal to the crown."* | You know of a plot and are not in it. | Persuade the lord to stay out of it, or to leave it. If you convince the plot's leader, the whole plot falls apart and that leader stays loyal for 60 days. |
| *"There is talk of a plot. Where does your house stand?"* | You know of a plot, are not in it, and do not know this lord's stance. | The lord tells the truth if your relation is 10 or better, or else with a chance of 30% plus 2% for every 10 points of your Charm. Ask the same lord again within 7 days and you get nothing but *"Plots? I know nothing of plots..."* A member names the leader; a leader admits it; an outsider may know the leader's name. You remember the answer for 60 days. |
| *"I know what you are planning. Count me in."* | You are talking to the plot's leader and know they lead it. | You join if they would take you like any other lord: your relation with them and with the ruler and your traits count, and a score of 5 is enough. Otherwise: *"I do not trust you enough for that. Not yet."* Not possible while you are sworn to the crown. |
| *"I will have no more part in this plot of yours."* | You are a member of an AI lord's plot and talk to its leader. | You leave the plot. *"Then go, and keep your mouth shut."* |

**How persuasion works.** It uses the game's usual persuasion screen. Some lords agree at once (*"You need not persuade me..."*). Some refuse to discuss it at all, for example lords already sworn to the other side. When you ask a lord to stay loyal without knowing where they stand, they only open up if they would tell you the truth when asked (same roll as above); otherwise they answer *"Plots, loyalty... I will not speak of such things with you."* The rest want convincing, and how many arguments you need to win depends on how far they are from changing their mind and on your relation with them. A good relation (15 or more) makes it easier, a bad one harder, and being at the same feast or out at the same hunt makes it easier.

The four arguments for joining:

- *"Fortune favours the bold..."* (Leadership; suits a lord with Valor)
- *"Count the houses already with us..."* (Tactics; suits a Calculating lord, easier once the plot holds 30%)
- *"{Ruler} broke faith with the lords of this realm..."* (Charm; suits an honorable lord, easier if they dislike the ruler)
- *"There will be lands to give when this is over..."* (Roguery; suits a generous lord, easier with a clan that has no fiefs)

The four arguments for staying loyal:

- *"You swore an oath to {ruler}..."* (Charm; suits an honorable lord, easier if they like the ruler)
- *"This plot will fail..."* (Tactics; suits a Calculating lord)
- *"A war among ourselves burns our own villages..."* (Charm; suits a merciful lord)
- *"Do this for me, as a friend..."* (Charm; suits a generous lord, easier if they like you)

**Results:**

- A lord you win over to a plot is sworn to it for **30 days**.
- A lord you keep loyal is sworn to the crown for **30 days**, or **60 days** if you are the ruler.
- If you fail, you must wait **45 days** before trying that lord again. A bad failure means **60 days** and **−4** relation.

### The Factions tab

Open the kingdom screen (**K**) and pick the **Factions** tab, from anywhere. It is laid out like the game's Diplomacy tab: on the left, the mood of every house of the realm, the feuds and factions, and the plots against the crown, one entry each; on the right, the two sides face to face with the game's comparison bars (strength, fiefs, houses) and the list of their houses. If you know of nothing, it says *"No whispers reach you."* Once you know of a plot, its entry lists every house of the realm by strength with what you know of its stance: *leads the plot* (only once you have found out who leads it), *in the plot*, *in the plot, sworn*, *loyal*, *loyal, sworn*, *wavering* (could still go either way), *the ruler*, *the crown's own* (the ruler's close kin), or *unknown*.

If you are in the plot, the top line and a bar give its exact share of the realm's strength and when it can rise. If you are not, you only learn who leads it, and only once you have found out.

As ruler, the tab lists under **The crown's will** the lords who will vote with you to [take a fief from a house](royal-court.md#winning-the-votes-first), with the days they have left. Under **Fiefs and rights**, **Your house's rights** shows your [rights to fiefs](fief-rights.md), the forged grants still looking for witnesses, who claims your fiefs, and the lords who will back your house when the next [fief is shared out](council.md#who-gets-a-fief).

### Leading your own plot

- You cannot start a plot while you are in another. Your clan needs a Clan Strength of 1,000. Unlike the AI, you can plot in **any** kingdom, large or not, as long as you are neither its ruler nor the ruler's close kin.
- Lords also join and leave your plot by themselves each week, using the same scores as above. An AI ruler tries to win your members back.
- Your plot only fails if it has not reached 25% within 60 days. It does not give up after 120 days, and it does not die when the realm shrinks. Other plots may grow beside yours, and lords weigh yours against theirs; whichever rises first ends the rest.

### Raise the banner

When you lead the plot, its entry in the **Factions** tab has a **"Raise the banner"** button. It works only:

- while you are **inside a town or castle** of your kingdom held by a house of your plot (yours included);
- with the plot holding **40%** of the realm's strength (the AI needs 50%);
- with the kingdom at peace with every other kingdom;
- with the crown still holding a town or castle of its own;
- when no story quest is under way and you are not in the middle of a fight.

If something is missing, the button is greyed out and its tooltip says what. A confirmation explains that there is no going back, that peace is impossible for 120 days, and that if the crown wins your lands are forfeit and you are banished. Then you **name your kingdom** (it cannot take the name of the realm you rise against). Your plot's houses follow you with their lands, and the civil war begins.

### When an AI plot you are in rises

You get a window, **"The banner is raised"**:

- **"Ride with them":** your clan goes over to the rebel kingdom with its fiefs.
- **"Stay loyal to the crown":** you leave the plot and are sworn to the crown for 30 days. If the rising goes ahead without you, its leader loses **20** relation with you.

During a story quest you can only stay, with no penalty.

### If you are the ruler

- Discontent wears on your lords' relation with you, but never on your own clan or close kin, and those never plot against you.
- Nobody wins lords back for you: talk to them yourself (*"There is a plot against {your name}. Stay loyal to the crown."*), or send an envoy. A lord you keep loyal stays so for 60 days. Talking the plot's leader out of it ends the plot.
- When the rumour reaches you, ask around, and watch the **Factions** tab, to find who is behind it.
- **You can lose the crown.** If the rebels win, their leader rules your kingdom and your house stays on as a vassal.

### Envoys

With [Envoys](envoys.md) you can send a family member or companion to do this talking for you: **"Win a lord over to our plot"** (when you are in one) or **"Keep a lord loyal to the crown"** (when you know of one). An envoy sent to sound a lord out also reports where their house stands on the plot.

## Tips

- Discontent only starts once a realm is a quarter above its fair share. Conquering past that point slowly turns your own lords against the ruler.
- A plot's leader needs relation −5 or worse with the ruler. Gaining relation with your strongest clan leaders (feasts, gifts, favours) keeps them from starting one.
- Watch the **Calculating** lords: they hold back while a plot is small and rush in once it passes 30%.
- The AI only rises in peacetime. A ruler facing a strong plot is safe while at war with another kingdom, but a plot that already has enough waits for the peace.
- Feasts and hunts make winning lords over easier, for you and for the AI.
- Keep a town or castle of your plot in mind before you start: you can only raise the banner from inside one of them.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `RealmDiscontentEnabled` to `false`: large kingdoms cause no discontent (what it already took comes back slowly).
- `ConspiracyEnabled` to `false`: no new plots, and plots under way are called off. A civil war already going on continues until it ends.
- `CivilWarOutsideRestraintEnabled` to `false`: other kingdoms treat a war against either side of a civil war like any other war.
- `EnvoyPlotJoinEnabled` / `EnvoyPlotLoyalEnabled` to `false`: removes the two envoy errands for plots.
- `HuntPlotRecruitEnabled` to `false`: hunts no longer make talking lords into or out of a plot easier.
