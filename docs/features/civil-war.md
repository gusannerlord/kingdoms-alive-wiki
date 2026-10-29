# Civil war

Any kingdom can rot from within, and the larger it grows, the more ambitious and rancorous its lords become. Lords wronged by the crown lose patience with the ruler, a discontented clan starts a plot to put another house on the throne, and if the plot grows strong enough it raises its banner and the realm splits in a civil war. You can join a plot, lead one, urge a lord to press his claim to the crown, work against it, or, if you wear the crown, fight to keep it.

## How large a kingdom is

The mod compares each kingdom with its fair share of the map: all the towns and castles held by kingdoms, divided by the number of kingdoms. Kingdoms already destroyed still count in that number. Kingdoms born from a rising never do, so one civil war does not make every other realm look larger.

### Great realms, restless lords

The larger a kingdom grows beyond its fair share, the more ambitious and rancorous its lords become. At its fair share or below, nothing changes; above it, the effects grow steadily and are full at **twice** its fair share (halfway at 1.5 times). Example: with 80 towns and castles and 8 kingdoms, the fair share is 10; a kingdom with 15 is halfway, one with 20 or more is at the full.

| Effect | At twice the fair share or more |
|---|---|
| Every [grievance against the crown](factions.md#lords-remember) weighs more when it is born, and so does the goodwill toward the ruler it costs | twice as much |
| The relation with the ruler a house needs to [start a plot](#who-starts-one) | **+5 or worse** (instead of −5) |
| Every lord's wish to join a plot or a [faction](factions.md) of the realm | **+10** |
| The grudge a house needs to begin a [Reckoning](factions.md#the-reckoning-of-a-house) | **30% less** |

Grievances one house holds against another do not change with the size. A kingdom that shrinks back calms down at once for what comes next; what has already happened stays.

### "Too large"

A kingdom is **too large** once it holds **1.25 times** its fair share or more (13 or more in the example above). This only counts for the old discontent below (off by default), for a clan without towns or castles in a plot (see [Who joins, and why](#who-joins-and-why)) and, if you turn on `PlotsOnlyInLargeRealms`, for where the AI may plot.

## Discontent (off by default)

Since version 1.27.1 this is off unless you turn it on (`RealmDiscontentEnabled`): lords now turn on their ruler through what the crown has done to them (see [grudges against the crown](factions.md#lords-remember)), not for the size of the realm alone. With it on:

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

Every plot has two houses at its head, and they may be the same:

- the **leader**, the house that starts the plot, gathers the lords and, if it comes to it, raises the banner;
- the **pretender**, the house the plot would put on the throne.

### Claims to the throne

Only a house with a **claim to the throne** can be a pretender. The claim belongs to the house and is judged with whoever heads it today: if the head dies, the new head may keep the claim or lose it. A house has a claim when:

- **its head is close kin of the ruler** while leading a house of their own: the ruler's father or mother, son or daughter, brother or sister, husband or wife;
- **it married into the royal house**: its head's husband or wife is close kin of the ruler;
- **it once ruled the realm**: a house that wore this crown before, for example one deposed in an earlier civil war or one that lost the throne in a vote;
- **the law of the realm counts it among the worthy**. In the realms whose law chooses among the heads of houses (the Senate of the Northern Empire, the acclamation of the Western Empire, Battanian tanistry, the Aserai sheikhs' council and the Thing of the Nords), the **three** houses with the best [claim to rule](succession.md#what-makes-a-claim), besides the ruler's own, have a claim too;
- **it is of the old blood of the realm**. In the realms of hereditary law (Vlandia, Sturgia, the Southern Empire) and of the founder's blood (the Khuzaits), the **two** houses with the best claim to rule, besides the ruler's own, have a claim too.

The ruling house itself never plots. Every civil war the rebels win adds the deposed house to those that once ruled, so claims grow with the realm's history.

The houses with a claim are listed under **The Crown** in the Court tab of the kingdom screen, and on each clan's page in the Encyclopedia (see [The crown and its claim](succession.md#where-you-see-it)).

### Who starts one

Every 7 days, in every kingdom, the AI clan leaders may start a plot. Any vassal house can start one if:

- its leader's relation with the ruler is **−5 or worse**, rising to **+5 or worse** in a kingdom of twice its fair share (see [Great realms, restless lords](#great-realms-restless-lords)); and 10 more than that if the ruler's claim is [weak](succession.md#what-a-claim-does) and theirs is better;
- it is not the ruling house nor a mercenary, is not already in a plot or a [faction](factions.md), and is not sworn to the crown at the moment (see below).

A house needs no strength of its own to start a plot. The ruler's brother or son heading another house can start one too: he is the classic pretender.

Each such leader has a **10% chance** a week, plus 5% for each level of Calculating and of Valor, minus 10% for each level of Honor.

### Who it would crown

A pretender needs a claim to the throne, a **Clan Strength of 500 or more** (the figure shown on the clan's page in the Encyclopedia), and a relation with the ruler of **+10 or worse**: a lord who is merely cool toward the ruler will still take the crown if it is offered.

- If the house that starts the plot can be crowned itself, it is its own pretender (its −5 with the ruler is already enough). The plot then starts only if at least one other clan would join it straight away.
- If not, the plot is born together with the house with a claim that leans to it most, weighed like any lord deciding whether to join (see below), with the plot's leader as the man asking and **+10** for being the one who would wear the crown. It needs a score of 25. Between two equal, the one with the better claim to rule. That house joins at once as the plot's first member.
- If no house with a claim would have it, there is no plot. Nobody is ever forced, and an AI plot never names your house: whether you press a claim is your choice (see [Your part in it](#your-part-in-it)).

**The pretender is fixed** for the life of the plot: it is never replaced by another. If the pretender's house dies out, leaves the plot, leaves the kingdom or turns mercenary, comes to the throne, or **loses its claim**, the plot ends. A claim can be lost when the ruler dies and the new one is not kin, when the husband or wife who tied a house to the royal one dies, or when a house slips from among the worthy or the old blood: once a house is a pretender, it keeps such a claim as long as it stays among the **five** best claims of the realm (the **four** best under a hereditary law or the founder's blood).

### Several plots at once

A kingdom can hold **up to three plots at once**, each behind its own pretender. A house is in one plot at most, the one it leans to most, and goes over to another only if it leans to it clearly more (a house that gave its word stays where it swore). The **first plot to rise ends all the others**.

The house that led a plot cannot lead another for **60 days** after it ends; other houses of the realm can. No new plot starts for **100 days** after a civil war.

A [vassal realm](vassal-realms.md) never has a plot or a civil war: a plot under way dies quietly when its realm bends the knee. And no realm becomes a vassal while either side is in a civil war.

## Who joins, and why

Every 7 days, each clan leader of the kingdom weighs every plot. The ruler's own clan never joins. The rest add up a score:

| What counts | Effect |
|---|---|
| Relation with the plot's leader and its pretender | half of it, for or against; when the two are different houses, the average of the two relations (the one who asks and the one who would reign both matter) |
| Relation with the ruler | 0.7 of it, the other way: liking the ruler holds them back, hating the ruler pushes them in |
| Honor | −8 per level |
| Valor | +3 per level |
| Calculating | only a calculating lord sides with the winner: drawn in once the plot holds more than 30% of the realm's strength, put off below that |
| How big the plot is | up to +20, as it grows toward the whole realm |
| Clan without towns or castles | +10, only while the realm is [too large](#too-large) |
| The size of the realm | up to +10 (see [Great realms, restless lords](#great-realms-restless-lords)) |
| Close kin or in-law of the plot's leader or of its pretender | +20 |
| Being the plot's pretender | +10 (the pretender weighs only the leader, not himself) |
| Swore the [oath of fealty](royal-court.md#the-oath-to-a-new-ruler) to the current ruler | −10, for 120 days |
| Refused that oath, or let the time pass | +20, for 180 days |
| Dismissed from the [court](royal-court.md#the-offices) | up to +8, fading over about 120 days |
| The [claims](succession.md) of the plot's pretender and the ruler | up to +10 when the pretender's claim is the better one; up to −10 when the ruler's claim is beyond question |

A lord **joins at 25** and **leaves below 5**. A pretender who is not the plot's leader weighs it the same way each week: if he leaves, the plot ends. Example: a lord with −20 toward the ruler (+14) and +10 toward the plotter (+5), with the plot holding 30% of the realm (+6), reaches 25 and joins.

"The realm's strength" here means the Clan Strength of all its vassal clans together, the ruler's clan included and mercenaries left out. The plot's **share** is the part of that held by its clans.

**The plot's leader recruits.** Each week an AI plot leader tries to win over one undecided lord (score between 5 and 25), the closest to joining. The odds are 15%, plus 2% for every 10 points of the leader's Charm, plus 2% for each point the lord is above 5, between 5% and 60%. At the same feast or the same [hunt](hunts.md) the odds are 1.5 times higher. A lord won over this way stays in the plot for at least 30 days. Once the plot holds 60% of the realm, the leader stops recruiting (lords may still join by themselves).

**At a hunt.** An AI plot leader who hosts a hunt likes to invite wavering lords (score between 5 and 25). On the last day of the hunt they try once to win over each wavering guest who came, with the odds above, 1.5 times higher. A member of the plot who hosts a hunt tries with each wavering guest half the time. An AI ruler who knows of the plot and hosts a hunt tries to win back each guest who is in it, except its pretender.

**The ruler wins lords back.** Once the plot holds 25% of the realm, an AI ruler tries each week to win back the member who is least committed, never the leader nor the pretender. The deeper the lord is in it, the harder. A lord won back leaves the plot, gains **+5** relation with the ruler and stays loyal for at least **60 days**. If you are the ruler, this is your job (see below).

## Rumours

When a plot reaches **20%** of the realm's strength, and you are a vassal of that kingdom outside the plot, you hear: *"There is talk of a plot among the lords of {Kingdom} against {ruler}. Who is behind it, nobody will say."* If you are the ruler, it says "against you". From then on you know a plot exists, but not who leads it or who is in it.

## How a plot dies

- **It never grew:** a plot that has not reached **25%** within **60 days** comes to nothing.
- **It stalls (AI plots only):** after **120 days** without holding enough to rise (counted from its start, or from the last week it had enough), it gives up.
- **The realm shrank (AI plots only, and only with `PlotsOnlyInLargeRealms` on):** once the kingdom has been back below "too large" for **60 days in a row**, it ends. By default a kingdom that shrinks does not end its plots.
- **The leader is gone:** the leader dies, is replaced at the head of the clan, leaves the kingdom, becomes a mercenary or comes to the throne.
- **The pretender is gone:** the pretender's house dies out, leaves the plot, leaves the kingdom, becomes a mercenary, comes to the throne or loses its claim (see [Who it would crown](#who-it-would-crown)).
- **The leader or the pretender is talked out of it** (by you, see below).

If you knew of it you see *"The plot among the lords of {Kingdom} has come to nothing."* If you were in it and its pretender fell, you are told instead that there is no crowning that house now, and the plot falls apart; if the plot was crowning you and your house lost its claim, you are told that the lords no longer hold your house has any right to the throne.

## The rising

An AI plot may raise its banner when **all** of this is true:

- it holds **50%** of the realm's strength. From there it is a matter of nerve: each week there is a chance it rises, small at half the realm and growing with its strength, and from **70%** it always rises;
- it began at least **21 days** ago and has at least one clan besides its leader's;
- with `PlotsOnlyInLargeRealms` on (off by default), the kingdom is too large, or was within the last 14 days;
- the kingdom is **at peace with every other kingdom** (nobody rises while the realm fights a foreign war);
- at least one house of the plot holds a town or castle, and the crown keeps at least one of its own.

When it rises:

- The plot's leader founds a **new kingdom**, named *"{Clan} Pretenders"* after the house it would crown, with the leader's culture and emblem, on a banner of its own colours, distinct from the realm it rose against (if you lead the rising, your clan keeps its own colours). It claims the throne and is at war with the crown at once.
- Every clan of the plot goes over with its towns, castles and villages, keeps its influence, and must stay at least **60 days**.
- The news says whom the rising would crown when it is not its leader: *"{Leader} of the {Clan} has raised the banner against {ruler} to crown {pretender} of the {Clan}! Civil war in {Kingdom}."*
- You are told in the middle of the screen, wherever it happens: *"Civil war: {Leader} of the {Clan} has raised the banner against {ruler}, ruler of the {people}."* (or *"Civil war in your realm: ..."* in your own kingdom). If you led the rising, were in the plot or were asked whether you ride with it, you already know and get no extra notice.
- The log keeps a red line with the news and the houses that went over to the rebels.

## Winning the civil war

Each day the mod compares the two sides: the total Clan Strength of each side's vassal clans.

- **By strength:** from day **30** of the war, a side that holds **twice** the other's strength for **10 days in a row** wins.
- **By land:** a side left without a single town or castle loses at once, even before day 30.

Nothing is settled while you are in a battle or siege on either side; it waits for the fight to end.

## The outcomes

**The rebels win.** The **pretender's** house becomes the ruling clan of the old kingdom, even when another house led the rising (if the pretender's house is no longer with the rebels, the rebel kingdom's ruler takes the crown instead). Every rebel house comes back into it (and must stay 60 days), and the rebel kingdom disappears. The old ruler loses **20** relation with the new one. If that ruler was you: *"You have lost the throne of {Kingdom}. {New ruler} of the {Clan} now rules; your house remains as a vassal."*

If you were the pretender and win, you are told the crown of the kingdom is yours; if you led the rising for another house, that house is crowned and you return as its vassal. A new ruler means a new [oath of fealty](royal-court.md#the-oath-to-a-new-ruler): the houses that stayed loyal to the old crown are much less willing to swear to the winner.

**The crown wins.** The plot's leader loses every town and castle (they go to the ruler) and is banished: an AI clan goes to another kingdom, preferably of its own culture and whose ruler it likes best, never yours. If none will do, it is left without a kingdom. The other rebel houses come back pardoned, each with **−20** relation with the ruler, and must stay 60 days.

**A negotiated peace.** From day **120** either side may offer peace. It is never automatic: the side that receives the offer must want it (if that side is a kingdom you rule, you decide). Before day 120 a peace is refused with *"Blood is still too hot for talk of peace in this civil war. Unless one side wins outright, it will be some {N} days before either will hear of it."* A peace leaves **two kingdoms**: the rebels keep what they hold, and an AI rebel kingdom drops "Pretenders" and becomes *"Realm of the {Clan}"*. A side that has already lost every town and castle cannot make peace: it has lost.

**Afterwards:** every kingdom that comes out of a civil war gets **100 days of calm**: no new plots (and, with the old discontent on, no discontent, while the discontent of the past slowly mends).

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
| *"{Ruler} is leading this realm to ruin. Would you stand with me if it came to it?"* | You are not of the ruling house, you are in no plot, and the lord is not of the ruling house. | Starts **your own plot**, with **you as its pretender**, and tries to win this lord over. Greyed out if your house has no claim to the throne (*"Your house has no claim to the crown, and the lords would ask whom you mean to crown..."*), if your Clan Strength is below 500, if the realm is in its calm after a civil war (*"The lords of the realm are wary just now. It is too soon."*), if a plot you led ended in the last 60 days, or if you spoke to this lord about it too lately. If the realm already holds three plots, the lord answers *"Hush. You are not the first to say so..."* and you learn that they exist. |
| *"Your house has a claim to the crown. Will you press it?"* | You cannot be crowned yourself (no claim, or a Clan Strength below 500), you are in no plot, and the lord's house has a claim. | Persuades the lord to **press his house's claim**, with you leading the plot. Greyed out if his house's Clan Strength is below 500, if the realm is in its calm, if your plot or his ended in the last 60 days, or if you spoke to him too lately. A lord who likes the ruler too well (relation above +10) will not hear of it. If you win, the plot is born at once: you lead it, his house is its pretender and first member, and it stands by your plot for as long as the plot lasts (it falls only if the house dies out, loses its claim, leaves the realm or is talked out of it). |
| *"There are those of us who mean to set this realm right. Join our cause."* | You are in a plot, your own or an AI lord's. | Persuade the lord to join. |
| *"There is a plot against {ruler}. Stay loyal to the crown."* | You know of a plot and are not in it. | Persuade the lord to stay out of it, or to leave it. If you convince the plot's leader or its pretender, the whole plot falls apart and that lord stays loyal for 60 days. |
| *"There is talk of a plot. Where does your house stand?"* | You know of a plot, are not in it, and do not know this lord's stance. | The lord tells the truth if your relation is 10 or better, or else with a chance of 30% plus 2% for every 10 points of your Charm. Ask the same lord again within 7 days and you get nothing but *"Plots? I know nothing of plots..."* A member names the leader; a leader admits it; a pretender admits that it is his house the plot would crown; an outsider may know the leader's name. You remember the answer for 60 days. |
| *"I know what you are planning. Count me in."* | You are talking to the plot's leader and know they lead it. | You join if they would take you like any other lord: your relation with them and with the ruler and your traits count, and a score of 5 is enough. Otherwise: *"I do not trust you enough for that. Not yet."* Not possible while you are sworn to the crown. |
| *"I will have no more part in this plot of yours."* | You are a member of an AI lord's plot and talk to its leader. | You leave the plot. *"Then go, and keep your mouth shut."* |

**How persuasion works.** It uses the game's usual persuasion screen. Some lords agree at once (*"You need not persuade me..."*). Some refuse to discuss it at all, for example lords already sworn to the other side. When you ask a lord to stay loyal without knowing where they stand, they only open up if they would tell you the truth when asked (same roll as above); otherwise they answer *"Plots, loyalty... I will not speak of such things with you."* The rest want convincing, and how many arguments you need to win depends on how far they are from changing their mind and on your relation with them. A good relation (15 or more) makes it easier, a bad one harder, and being at the same feast or out at the same hunt makes it easier.

The four arguments for joining:

- *"Fortune favours the bold..."* (Leadership; suits a lord with Valor)
- *"Count the houses already with us..."* (Tactics; suits a Calculating lord, easier once the plot holds 30%)
- *"{Ruler} broke faith with the lords of this realm..."* (Charm; suits an honorable lord, easier if they dislike the ruler)
- *"There will be lands to give when this is over..."* (Roguery; suits a generous lord, easier with a clan that has no fiefs)

The four arguments for pressing a claim:

- *"A claim never pressed dies with the one who held it..."* (Leadership; suits a lord with Valor)
- *"Count the houses that have no love for {ruler}..."* (Tactics; suits a Calculating lord)
- *"{Ruler} broke faith with the lords of this realm. Your right gives you the duty to set it right."* (Charm; suits an honorable lord, easier if they dislike the ruler)
- *"I ask nothing for myself but to stand at your side when you are crowned."* (Charm; suits a generous lord, easier if they like you)

The four arguments for staying loyal:

- *"You swore an oath to {ruler}..."* (Charm; suits an honorable lord, easier if they like the ruler)
- *"This plot will fail..."* (Tactics; suits a Calculating lord)
- *"A war among ourselves burns our own villages..."* (Charm; suits a merciful lord)
- *"Do this for me, as a friend..."* (Charm; suits a generous lord, easier if they like you)

**Results:**

- A lord you win over to a plot is sworn to it for **30 days**. A lord who agrees to press his claim stays with your plot for as long as it lasts.
- A lord you keep loyal is sworn to the crown for **30 days**, or **60 days** if you are the ruler.
- If you fail, you must wait **45 days** before trying that lord again. A bad failure means **60 days** and **−4** relation.

### The Factions tab

Open the kingdom screen (**K**) and pick the **Factions** tab, from anywhere. It is laid out like the game's Diplomacy tab: on the left, the mood of every house of the realm, the feuds and factions, and the plots against the crown, one entry each; on the right, the two sides face to face with the game's comparison bars (strength, fiefs, houses) and the list of their houses. If you know of nothing, it says *"No whispers reach you."* Once you know of a plot, its entry lists every house of the realm by strength with what you know of its stance: *leads the plot* (only once you have found out who leads it), *the house the plot would crown* (likewise), *in the plot*, *in the plot, sworn*, *loyal*, *loyal, sworn*, *wavering* (could still go either way), *the ruler*, or *unknown*. *The crown's own* only appears with claims to the throne turned off, for the ruler's close kin, who then never plot.

If you are in the plot, the top line and a bar give its exact share of the realm's strength and when it can rise. If you are not, you only learn who leads it, and only once you have found out. Once you know who leads it, the text also says whom it would crown and by what right, for example *"... gathers the lords who would crown {pretender} of the {Clan}, brother to {ruler}."* Your journal entry for the plot says the same.

As ruler, the tab lists under **The crown's will** the lords who will vote with you to [take a fief from a house](royal-court.md#winning-the-votes-first), with the days they have left. Under **Fiefs and rights**, **Your house's rights** shows your [rights to fiefs](fief-rights.md), who of your house is forging a claim at a foreign court, who claims your fiefs, and the lords who will back your house when the next [fief is shared out](council.md#who-gets-a-fief).

### Leading your own plot

- You cannot start a plot while you are in another. To lead a plot that crowns you, your house needs a claim to the throne and a Clan Strength of 500; without them, find a lord whose house has a claim and urge him to press it. Like the AI, you can plot in **any** kingdom, large or not, as long as your house does not rule it; unlike the AI, you need no bad blood with the ruler.
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

- Every wrong your crown does a house costs a little of its head's goodwill toward you (more in a kingdom grown well beyond its fair share), but never your own clan or close kin; with the old discontent on, the size of the realm wears on it too. Your own clan never plots against you, but a brother, son or daughter heading a house of their own has a claim to your throne and may.
- Nobody wins lords back for you: talk to them yourself (*"There is a plot against {your name}. Stay loyal to the crown."*), or send an envoy. A lord you keep loyal stays so for 60 days. Talking the plot's leader out of it ends the plot.
- When the rumour reaches you, ask around, and watch the **Factions** tab, to find who is behind it.
- **You can lose the crown.** If the rebels win, the house they meant to crown rules your kingdom and your house stays on as a vassal.

### Envoys

With [Envoys](envoys.md) you can send a family member or companion to do this talking for you: **"Win a lord over to our plot"** (when you are in one) or **"Keep a lord loyal to the crown"** (when you know of one). An envoy sent to sound a lord out also reports where their house stands on the plot.

## Tips

- Conquest has a price at home: past its fair share, every wrong the crown does a house stings more, and its lords plot and band together more readily. At twice its fair share, a lord merely cool toward the ruler may start a plot.
- A plot's leader needs relation −5 or worse with the ruler (up to +5 in a kingdom of twice its fair share), and its pretender +10 or worse. Gaining relation with your discontented lords keeps them from starting one, and keeping on good terms with the strong houses that have a claim leaves a plot nobody to crown.
- Want the crown without a claim of your own? Marry the head of your house to the ruler's brother, sister, son or daughter, or find a claimant house and press its claim for it.
- Watch the **Calculating** lords: they hold back while a plot is small and rush in once it passes 30%.
- The AI only rises in peacetime. A ruler facing a strong plot is safe while at war with another kingdom, but a plot that already has enough waits for the peace.
- Feasts and hunts make winning lords over easier, for you and for the AI.
- Keep a town or castle of your plot in mind before you start: you can only raise the banner from inside one of them.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `RealmDiscontentEnabled` (off by default): `true` brings back the discontent of large kingdoms; off, what it already took comes back slowly.
- `ConspiracyEnabled` to `false`: no new plots, and plots under way are called off. A civil war already going on continues until it ends.
- `RealmSizeAmbitionEnabled` to `false`: the size of a kingdom no longer makes its lords more rancorous or ambitious. Numbers you can change: `RealmSizeFullAtTimesShare` (2, the size at which the effects are full), `RealmSizeGrievanceBoost` (1: grievances against the crown up to twice as heavy), `RealmSizePlotRelationBoost` (10, how much better the relation to start a plot may be), `RealmSizeJoinBoost` (10) and `RealmSizeReckoningGrudgeCut` (0.3).
- `PlotsOnlyInLargeRealms` to `true` (off by default): the old way, where the AI plots only in a kingdom that is too large or under a ruler with a weak claim, and an AI plot ends once its kingdom has been back below "too large" for 60 days.
- `ThroneClaimsEnabled` to `false`: plots work as before the claims to the throne: the house that starts a plot is always its pretender and needs a Clan Strength of 500, and the ruler's close kin never plot.
- `CivilWarOutsideRestraintEnabled` to `false`: other kingdoms treat a war against either side of a civil war like any other war.
- `EnvoyPlotJoinEnabled` / `EnvoyPlotLoyalEnabled` to `false`: removes the two envoy errands for plots.
- `HuntPlotRecruitEnabled` to `false`: hunts no longer make talking lords into or out of a plot easier.
