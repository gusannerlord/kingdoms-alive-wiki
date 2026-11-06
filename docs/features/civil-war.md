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

Every plot against the crown has two houses at its head, and they may be the same (a [plot to break away](#plots-to-break-away) has rules of its own):

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

In the realms of the Empire, a strategos may also plot a **coup**, a plot of its own kind with its own rules: see [The Empire's own ways](empire.md).

The houses with a claim are listed under **The Crown** in the Court tab of the kingdom screen, and on each clan's page in the Encyclopedia (see [The crown and its claim](succession.md#where-you-see-it)).

### Who starts one (very soon in 2.0.0) {#who-starts-one}

Every 7 days, in every kingdom, the AI clan leaders may start a plot. Any vassal house can start one if:

- its leader's relation with the ruler is **−5 or worse**, rising to **+5 or worse** in a kingdom of twice its fair share (see [Great realms, restless lords](#great-realms-restless-lords)); and 10 more than that if the ruler's claim is [weak](succession.md#what-a-claim-does) and theirs is better;
- it is not the ruling house nor a mercenary, is not already in a plot or a [faction](factions.md), and has given its word to no side at the moment, neither to the crown nor to a plot (see below).

No plot starts in a kingdom that is the vassal of another, during a civil war or in the 100 days of calm after one, or while the kingdom already holds three plots; and at most one new plot is born in a kingdom each week.

A house needs no strength of its own to start a plot. The ruler's brother or son heading another house can start one too: he is the classic pretender.

Each such leader has a **10% chance** a week, plus 5% for each level of Calculating, minus 10% for each level of Honor.

### Who it would crown (very soon in 2.0.0) {#who-it-would-crown}

A pretender needs a claim to the throne, a **Clan Strength of 500 or more** (the figure shown on the clan's page in the Encyclopedia), and a relation with the ruler of **+10 or worse**: a lord who is merely cool toward the ruler will still take the crown if it is offered.

- If the house that starts the plot can be crowned itself, it is its own pretender (its −5 with the ruler is already enough). The plot then starts only if at least one other clan would join it straight away.
- If not, the plot is born together with the house with a claim that leans to it most, weighed like any lord deciding whether to join (see below), with the plot's leader as the man asking and **+10** for being the one who would wear the crown. It needs a score of 30. Between two equal, the one with the better claim to rule. That house joins at once as the plot's first member.
- If no house with a claim would have it, there is no plot. Nobody is ever forced, and an AI plot never names your house: whether you press a claim is your choice (see [Your part in it](#your-part-in-it)).

**The pretender is fixed** for the life of the plot: it is never replaced by another. If the pretender's house dies out, leaves the plot, leaves the kingdom or turns mercenary, comes to the throne, or **loses its claim**, the plot ends. A claim can be lost when the ruler dies and the new one is not kin, when the husband or wife who tied a house to the royal one dies, or when a house slips from among the worthy or the old blood: once a house is a pretender, it keeps such a claim as long as it stays among the **five** best claims of the realm (the **four** best under a hereditary law or the founder's blood).

### Several plots at once (very soon in 2.0.0) {#several-plots-at-once}

A kingdom can hold **up to three plots at once**, each behind its own pretender. A house is in one plot at most, the one it leans to most, and goes over to another only if it leans to it clearly more (a house that gave its word stays where it swore). The house a plot would crown never goes over to another plot. The **first plot to rise ends all the others**.

A house whose plot has ended may start another whenever it likes, with no wait. No new plot starts for **100 days** after a civil war.

A [vassal realm](vassal-realms.md) never has a plot or a civil war: a plot under way dies quietly when its realm bends the knee. And no realm becomes a vassal while either side is in a civil war.

## Who joins, and why (very soon in 2.0.0) {#who-joins-and-why}

Every 7 days, each clan leader of the kingdom weighs every plot. The ruler's own clan never joins. The rest add up a score:

| What counts | Effect |
|---|---|
| Relation with the plot's leader and its pretender | half of it, for or against; when the two are different houses, the average of the two relations (the one who asks and the one who would reign both matter) |
| Relation with the ruler | 0.85 of it, the other way: liking the ruler holds them back, hating the ruler pushes them in |
| Devoted to the ruler (relation above +60) | a further −0.875 per point beyond 60 (−35 at +100): such a house can still be won, but only by a much stronger cause. The same holds for you when you ask to join a plot. |
| Honor | −8 per level |
| Calculating | only a calculating lord sides with the winner: drawn in once the plot holds more than 30% of the realm's strength, put off below that |
| How big the plot is | up to +20, as it grows toward the whole realm |
| Clan without towns or castles | +10, only while the realm is [too large](#too-large) |
| The size of the realm | up to +10 (see [Great realms, restless lords](#great-realms-restless-lords)) |
| Close kin or in-law of the plot's leader or of its pretender | +20 |
| Being the plot's pretender | +10 (the pretender weighs only the leader, not himself) |
| Swore the [oath of fealty](royal-court.md#the-oath-to-a-new-ruler) to the current ruler | −10, for 120 days |
| Refused that oath, or let the time pass | +20, for 180 days |
| Dismissed from the [court](royal-court.md#the-offices) | up to +8, fading over about 120 days |
| [Grievances](factions.md) against the crown | up to +30, the more the house resents it |
| [Grievances](factions.md) against the plot's leading house, or the house it would crown | up to −30, the more the house resents it (the heavier of the two counts, not both) |
| Your house's [lord](titles.md) leads the plot or is in it | +20 (nothing among the Khuzaits, who all owe the khan before their noyan) |
| That lord stays out of it | −8 |
| That lord is the crown itself, as the house's count or duke | −30 |
| Of another faith than the ruler | +6 |
| The ruler refused lately to [step down](factions.md) | +5, for 90 days |
| The [claims](succession.md) of the plot's pretender and the ruler | up to +10 when the pretender's claim is the better one; up to −10 when the ruler's claim is beyond question |

What a house owes its lord counts for nothing once its head is at −30 or worse with that lord, and less the more the house holds against him.

A lord **joins at 30** and **leaves below 5**. A pretender who is not the plot's leader weighs it the same way each week: if he leaves, the plot ends. Example: a lord with −20 toward the ruler (+17) and +10 toward the plotter (+5), with the plot holding 30% of the realm (+6), reaches 28: not yet enough, but close enough to be talked into it.

"The realm's strength" here means the Clan Strength of all its vassal clans together, the ruler's clan included and mercenaries left out. The plot's **share** is the part of that held by its clans.

**The plot's leader recruits.** Each week an AI plot leader tries to win over one undecided lord who is already close to joining (score between 10 and 30), the closest of them. A lord further from it will not hear of it, from the AI or from you. The odds are 5%, plus 2% for every 10 points of the leader's Charm, plus 3% for each point the lord is above 10, at most 45%. At the same feast or the same [hunt](hunts.md) the odds are 1.5 times higher (so up to about two in three). A lord won over this way stays in the plot for at least 30 days. Once the plot holds 60% of the realm, the leader stops recruiting (lords may still join by themselves).

**At a hunt.** An AI plot leader who hosts a hunt likes to invite wavering lords (score between 10 and 30). On the last day of the hunt they try once to win over each wavering guest who came, with the odds above, 1.5 times higher. A member of the plot who hosts a hunt tries with each wavering guest half the time. An AI ruler who knows of the plot and hosts a hunt tries to win back each guest who is in it, except its pretender.

**The ruler wins lords back.** Once the plot holds 25% of the realm, an AI ruler tries each week to win back the member who is least committed, never the leader, the pretender, a house that swore to the plot in the last 30 days, nor you. The deeper the lord is in it, the harder. A lord won back leaves the plot, gains **+5** relation with the ruler and stays loyal for at least **60 days**. If you are the ruler, this is your job (see below).

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

## The rising (very soon in 2.0.0) {#the-rising}

An AI plot may raise its banner when **all** of this is true:

- it holds **45%** of the realm's strength. From there it is a matter of nerve: each week there is a chance it rises, small at first and growing with its strength, and from **70%** it always rises;
- it began at least **21 days** ago and has at least one clan besides its leader's;
- with `PlotsOnlyInLargeRealms` on (off by default), the kingdom is too large, or was within the last 14 days;
- at least one house of the plot holds a town or castle, and the crown keeps at least one of its own;
- the kingdom is not already in a civil war (several kingdoms may each have their own at the same time).

**A war abroad does not stop it.** A plot may rise while its realm fights another kingdom. But a realm that is **weak in its wars** makes the plotters think twice: while it is at war and either losing (the same mark as when an AI realm [turns to the defence](command-your-armies.md)) or holding fewer than **half** the towns and castles of an average realm, every chance of a rising is cut to **0.3** of what it would be, even from 70% (then it rises about one week in three). A realm that is losing but still **dominant**, holding more than 1.3 times its [fair share](#how-large-a-kingdom-is) of the map, is not held back.
 At peace, or at war and not weak, nothing changes.

**A battle only delays it.** If men of the plot's houses are in the thick of a battle when the plot decides to rise, the rising waits for the fighting to end, a day at most, and then goes ahead.

**A fief taken can set a plot alight.** When the council votes a town or castle away from a house of a plot, or the crown gives one away from it by decree in a feud:

- if **40%** or more of the realm's strength stands behind the plot, the house will not give it up and the plot **rises within the hour** (at once after a decree);
- under that, it depends on the head of the house and on the plot's strength: the nearer the plot is to 40% and the bolder the head (Valor), the likelier it rises all the same; a calculating head holds back. If it does not rise, the house may still break with the realm alone (leaving the plot), by the same odds as any house that loses a fief, or else it bows and yields.
- in a realm weak in its wars abroad (above), each of these chances, the sure one at 40% too, is cut to 0.3.

Before such a rising, every house of the realm that is free to choose weighs the plot once more, angrier for what happened: more so if it is kin or friend of the house wronged, or already holds a grievance against the crown. Those who are won over ride with the plot.

Such a rising still needs at least one house besides its leader's once the others have weighed it (if none comes, the house bows and yields), a town or castle among them, and a crown that keeps one of its own; never two civil wars in one realm at once, never in a kingdom that is the vassal of another, and not while you are in the plot during a story quest. If the house is yours and the plot can rise then, you choose: bow, raise the plot's banner, or break with the realm alone. If you lead the plot, you are asked whether to raise the banner now; if you are one of its houses, whether you ride with it. As ruler or loyal vassal, you are told when it happens. Turn it off with `PlotStripRisingEnabled`.

When it rises:

- The plot's leader founds a **new kingdom**, named *"{Clan} Pretenders"* after the house it would crown, with the leader's culture and emblem, on a banner of its own colours, distinct from the realm it rose against (if you lead the rising, your clan keeps its own colours). It claims the throne and is at war with the crown at once.
- Every clan of the plot goes over with its towns, castles and villages, keeps its influence, and must stay at least **60 days**.
- The news says whom the rising would crown when it is not its leader: *"{Leader} of the {Clan} has raised the banner against {ruler} to crown {pretender} of the {Clan}! Civil war in {Kingdom}."*
- You are told in the middle of the screen, wherever it happens: *"Civil war: {Leader} of the {Clan} has raised the banner against {ruler}, ruler of the {people}."* (or *"Civil war in your realm: ..."* in your own kingdom). If you led the rising, were in the plot or were asked whether you ride with it, you already know and get no extra notice.
- The log keeps a red line with the news and the houses that went over to the rebels.

## Winning the civil war (very soon in 2.0.0) {#winning-the-civil-war}

Each day the mod compares the two sides: the total Clan Strength of each side's vassal clans.

- **By strength:** from day **30** of the war, a side that holds **twice** the other's strength for **10 days in a row** wins.
- **By land:** a side left without a single town or castle loses at once, even before day 30.
- **By fiefs taken:** from day **30**, a side that has taken from the other, less what it lost to it, **40%** of the towns and castles the other side held when the plot rose (at least **2**) wins. Whichever comes first, strength or fiefs.

Nothing is settled while you are in a battle or siege on either side; it waits for the fight to end.

## The outcomes (very soon in 2.0.0) {#the-outcomes}

**The rebels win.** The **pretender's** house becomes the ruling clan of the old kingdom, even when another house led the rising (if the pretender's house is no longer with the rebels, the rebel kingdom's ruler takes the crown instead). Every rebel house comes back into it (and must stay 60 days), and the rebel kingdom disappears. The old ruler loses **20** relation with the new one. If that ruler was you: *"You have lost the throne of {Kingdom}. {New ruler} of the {Clan} now rules; your house remains as a vassal."*

If you were the pretender and win, you are told the crown of the kingdom is yours; if you led the rising for another house, that house is crowned and you return as its vassal. A new ruler means a new [oath of fealty](royal-court.md#the-oath-to-a-new-ruler): the houses that stayed loyal to the old crown are much less willing to swear to the winner.

**The crown wins.** Every rebel house comes back to the realm with its towns and castles, each with **−20** relation with the ruler, and must stay 60 days (hired mercenaries of the rebels simply leave). A charter that rose and lost is treated the same way. The head of the house that led the plot is put to death (a merciful ruler may spare the life; as ruler you choose), and every house that rose is marked as traitor for a while: the ruler judges them one by one by decree, hardest on the house that led the rising. Few dare to defy the judgment, and a house stripped of its land may leave the realm instead. See [Traitors and the houses of a realm](realm-houses.md).

**A negotiated peace.** From day **120** either side may offer peace. It is never automatic: the side that receives the offer must want it (if that side is a kingdom you rule, you decide). Before day 120 a peace is refused with *"Blood is still too hot for talk of peace in this civil war. Unless one side wins outright, it will be some {N} days before either will hear of it."* A side that has already lost every town and castle cannot make peace: it has lost.

A peace **mends the realm**: the rebel kingdom is dissolved and every house comes home (and must stay 60 days), on terms that follow how the war stood. First by the towns and castles each side took from the other, measured against what the other held when the plot rose; only if neither side has taken enough, by their strength:

| How the war stands | The terms |
|---|---|
| The rebels have taken a great deal (35% or more), or, failing that, are far stronger | The king **steps down** and the pretender's house is crowned, as a usurper, as when the rebels win; no one is punished |
| The rebels have taken a fair share (15% or more), or are somewhat stronger | In a realm whose crown passes by blood, the **pretender's house inherits** the throne when the king leaves it, by death or otherwise. In a realm that chooses its ruler, the crown's house and the loyal houses **pledge their votes** to the pretender's house at the next choice: it stands for certain and nearly always wins, but the vote is real. A house that pledged and votes for another breaks its word: the pretender's house thinks less of it and holds it against it, you included |
| Neither side ahead | **Amnesty**: everyone comes home with what they hold; the grudges remain |
| The crown has taken a fair share (15% or more of the rebels' land), or is the stronger | The rebels give back the crown's towns and castles they took, and the house that led the rising yields its best town or castle to the crown (even its last), and holds it against the crown; no one is put to death or marked as traitor |

Only when the house that led the rising is of **another culture or another faith** than the crown does a peace leave **two kingdoms**: the rebels keep what they hold, and an AI rebel kingdom drops "Pretenders" and becomes *"Realm of the {Clan}"*, after the house that rules it. When you weigh a peace in a civil war, as ruler or as the rebels' leader, you are told what it would bring as things stand. The heir or the pledge shows in the kingdom screen.

**Afterwards:** every kingdom that comes out of a civil war gets **100 days of calm**: no new plots, [factions](factions.md) or feuds (and, with the old discontent on, no discontent, while the discontent of the past slowly mends).

## Plots to break away (very soon in 2.0.0) {#plots-to-break-away}

Not every plot wants the crown. Houses that have had enough of their ruler, and whose lands lie together, may plot to **leave the realm with their lands** and stand as a realm of their own: a great duke and the lords around him, for example. Such a plot is rare and hard to grow, and likelier in a large realm.

**No one is talked into it, or out of it.** A house is in it only by its own leaning. Its leader courts no one, the ruler wins no one back, you cannot persuade a lord to join or to stay loyal (those lines are not offered for it, and an envoy cannot do it either), and a hunt changes nothing. A house in such a plot will not be talked into any other cause either.

**Who can be in it.** Every house in it, its leader too, must:

- hold a **town or castle**, and not be the ruling house;
- be on **bad terms with the ruler**: a relation of **−30 or worse**, eased up to **−20** in a kingdom of twice its fair share (see [Great realms, restless lords](#great-realms-restless-lords));
- hold a town or castle in the **lands of the plot** (below);
- be in no [faction](factions.md) or feud, and have given its word to no side.

**The lands of the plot.** They grow from the **seat** of the house that leads it (a duke's most prosperous town in his own duchy; else its most prosperous town; else its best castle) and take in every town and castle of the plot's houses that **touches** them, one after another. Two towns or castles touch when one is among the **4** nearest the other on the map and no town or castle of a house outside the plot lies between them; a town on an isle touches none. A house's other holds may lie apart: they do not keep it out, but they stay with the old realm if it breaks away. If the house that leads it loses its seat, the plot gathers around another of its holds.

**How it starts.** Every 7 days, each AI house that could be in one may start a plot to break away: **2%** a week, plus 1% for each level of Calculating, minus 1% for each level of Honor; up to twice as likely in a kingdom of twice its fair share, and half as likely again for a duke (or a strategos or noyan, see [titles](titles.md)). It needs no other house to start. **One** such plot at a time in a realm, besides (and not counted among) the three plots against the crown. None in a kingdom that is the vassal of another, during a civil war or in the calm after one.

**Who joins.** Every 7 days each house that could be in it weighs it much as it would [a plot against the crown](#who-joins-and-why) (its relation with the leader and the ruler, its character, grievances, kin, allies, its lord), with no pretender to weigh, and two reasons of its own: **+10** for a house of another culture than the ruling house, and up to **+10** in a large realm (*"A realm this wide cannot hold us"*). It joins at **30**. It leaves once its relation with the ruler is more than **5** better than the plot needs (it has made its peace with the crown, a new ruler came, or the realm shrank), or when none of its holds touch the plot's lands any more, or when its leaning falls below 5 as for any plot; the leader's peace with the crown, or the loss of all its holds, ends the plot. If you are in it, each house that joins or leaves writes to you, with its reason when one stands out.

**How it dies.** A plot that has not reached **15%** of the realm's strength within **60 days** comes to nothing; an AI plot that has not had **30%** for **180 days** gives up.

**The rising.** It rises at **30%** of the realm's strength, with at least **one other house** beside its leader, and under the other rules of a [rising](#the-rising): one civil war at a time, a war abroad no hindrance except in a weak realm, and a fief taken from one of its houses sets it alight, as for any plot, with 30% and another house. An AI plot waits at least 21 days; from 30% each week there is a chance it rises, growing with its strength, and from **50%** it always rises. The rebels fight as the **League of the {Clan}**: *"{Leader} of the {Clan} has raised the banner against {ruler}: the houses with him mean to break away from {Kingdom} with their lands! Civil war in {Kingdom}."* The war is won and lost as [any civil war](#winning-the-civil-war).

- **The rebels win:** they stand as a realm of their own, the **Realm of the {Clan}** after its ruling house (a realm you rule keeps the name you gave it), with the lands around their seat. Their towns and castles that lie apart go to the old ruler, to be shared out by its council. Both realms get their 100 days of calm. If the crown is left with no town or castle at all, the rebels take its throne instead, as in any civil war.
- **The crown wins:** as for any rising: the head of the house that led it is put to death (unless the ruler spares him) and the rebel houses come home [marked as traitors](realm-houses.md).
- **A negotiated peace** (from day 120): the crown recognises the new realm only when the rebels are **far ahead** (35% of the crown's land taken, or else far stronger); then they go as if they had won. If they are merely ahead, or neither side is, every house comes home under an **amnesty**; if the crown is ahead, on the **crown's terms**. A peace with a leading house of another culture or faith than the crown leaves two kingdoms whatever the terms, as for any civil war, and then too the holds apart stay with the crown. The peace window and the council's vote tell you what a peace would bring.

## Other kingdoms stay out

While a civil war lasts, other AI kingdoms are reluctant to attack either side:

- they need a much stronger reason than usual to declare war;
- they weigh each side as if half of the other side's strength stood with it;
- they never see the civil war as a chance to retake lost lands.

It is not impossible: a kingdom with a strong grievance may still attack. In the council you may hear *"they are at war among themselves, and we will not meddle in it"* or *"their rivals in the civil war would be the ones to gain"*. None of this holds back a kingdom you rule, nor an ally of one side attacking the other.

## Your part in it

Everything below needs you to lead your clan as a vassal (not a mercenary) of the kingdom, and neither you nor the lord you talk to can be a prisoner. You talk to clan leaders of your own kingdom: choose *"There is something I'd like to discuss."* and the plot options appear among the others.

### What you can say to a clan leader (very soon in 2.0.0) {#what-you-can-say-to-a-clan-leader}

| You say | When it appears | What it does |
|---|---|---|
| *"{Ruler} is leading this realm to ruin. Would you stand with me if it came to it?"* | You are not of the ruling house, you are in no plot, and the lord is not of the ruling house. | Starts **your own plot**, with **you as its pretender**, and tries to win this lord over. Not offered if your house has no claim to the throne, if your Clan Strength is below 500, or if the realm is in its calm after a civil war. If you spoke to this lord about it too lately, they tell you their answer has not changed. If the realm already holds three plots, the lord answers *"Hush. You are not the first to say so..."* and you learn that they exist. |
| *"Your house has a claim to the crown. Will you press it?"* | You cannot be crowned yourself (no claim, or a Clan Strength below 500), you are in no plot, and the lord's house has a claim. | Persuades the lord to **press his house's claim**, with you leading the plot. Not offered if his house's Clan Strength is below 500, or if the realm is in its calm. If you spoke to him too lately, he tells you his answer has not changed. A lord who likes the ruler too well (relation above +10) will not hear of it. If you win, the plot is born at once: you lead it, his house is its pretender and first member, and it stands by your plot for as long as the plot lasts (it falls only if the house dies out, loses its claim, leaves the realm or is talked out of it). |
| *"There are those of us who mean to set this realm right. Join our cause."* | You are in a plot, your own or an AI lord's. | Persuade the lord to join. A lord who agrees tells you what truly moves him (his grudge against the ruler, his love for you or the pretender, his faith, his own claim...), or gives no reason at all when nothing stands out. |
| *"There is a plot against {ruler}. Stay loyal to the crown."* | You know of a plot and are not in it. | Persuade the lord to stay out of it, or to leave it. If you convince the plot's leader or its pretender, the whole plot falls apart and that lord stays loyal for 60 days. |
| *"There is talk of a plot. Where does your house stand?"* | You know of a plot, are not in it, and do not know this lord's stance. | The lord tells the truth if your relation is 10 or better, or else with a chance of 30% plus 2% for every 10 points of your Charm. Ask the same lord again within 7 days and you get nothing but *"Plots? I know nothing of plots..."* A member names the leader; a leader admits it; a pretender admits that it is his house the plot would crown; an outsider may know the leader's name. You remember the answer for 60 days. |
| *"I know what you are planning. Count me in."* | You are talking to the plot's leader and know they lead it. | You join if they would take you like any other lord: your relation with them and with the ruler and your traits count, and a score of 10 is enough, as for a lord they would court. Otherwise: *"I do not trust you enough for that. Not yet."* Not possible while you are sworn to the crown or to another plot. |
| *"I will have no more part in this plot of yours."* | You are a member of an AI lord's plot and talk to its leader. | You leave the plot. *"Then go, and keep your mouth shut."* |

**How persuasion works.** It uses the game's usual persuasion screen. Some lords agree at once (*"You need not persuade me..."*). Some refuse to discuss it at all, for example lords already sworn to the other side. When you ask a lord to stay loyal without knowing where they stand, they only open up if they would tell you the truth when asked (same roll as above); otherwise they answer *"Plots, loyalty... I will not speak of such things with you."* A lord who is far from joining your plot (the same mark as for the AI: a score below 10) will not hear of it. The rest want convincing, and how many arguments you need to win depends on how far they are from changing their mind and on your relation with them. A good relation (15 or more) makes it easier, a bad one harder, and being at the same feast or out at the same hunt makes it easier.

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

### Raise the banner (very soon in 2.0.0) {#raise-the-banner}

When you lead the plot, its entry in the **Factions** tab has a **"Raise the banner"** button. It works only:

- while you are **inside a town or castle** of your kingdom held by a house of your plot (yours included);
- with the plot holding **40%** of the realm's strength (the AI needs 45%); you need no other house beside yours, no number of days and no luck. A war abroad does not stop you, and your own choice is never held back by a weak realm;
- with the crown still holding a town or castle of its own;
- when no story quest is under way, you are not in the middle of a fight and you do not ride in an army (*"Not while you ride in an army: leave it first."*);
- while no men of the plot's houses are in the thick of a battle (*"Men of the plot's houses are in the thick of a battle: the banner waits until the fighting is over."*).

If something is missing, the button is greyed out and its tooltip says what. A confirmation explains that there is no going back, that peace is impossible for 120 days, and what losing costs: every house that rode comes back branded traitor, and the crown will want your head. Then you **name your kingdom** (it cannot take the name of the realm you rise against). Your plot's houses follow you with their lands, and the civil war begins.

### When an AI plot you are in rises (very soon in 2.0.0) {#when-an-ai-plot-you-are-in-rises}

You get a window, **"The banner is raised"**, once you are free to answer: while you are a prisoner or ride in an army, it waits.

- **"Ride with them":** your clan goes over to the rebel kingdom with its fiefs.
- **"Stay loyal to the crown":** you leave the plot and are sworn to the crown for 30 days. If the rising goes ahead without you, its leader loses **20** relation with you.

During a story quest you can only stay, with no penalty.

### Breaking away yourself (very soon in 2.0.0) {#breaking-away-yourself}

As a vassal of a realm you do not rule, the **Factions** tab has an entry **"Break away from the realm"**: what such a plot asks, and whether your house could begin one now or why not (*"You are not on bad enough terms with {ruler}: no house would believe you mean it."*, *"None of your towns and castles touch the lands around {seat}..."*). Its **"Seek independence"** button starts it, after a confirmation, with you at its head and the lands around your seat; greyed, it says what is missing. The rules are the AI's: the same relation with the ruler, a town or castle, no other plot, faction or feud, no word given, and one such plot per realm. Houses join and leave it by themselves, and you cannot talk anyone into it. You raise its banner as your own plot's (see [Raise the banner](#raise-the-banner)), but at **30%** of the realm's strength and only with another house beside yours. Like its members, you leave it if you make your peace with the ruler.

To join an AI plot to break away, tell its leader, once you know who it is, *"I know what you are planning. Count me in."*: it is offered only when your house could be in it, and its leader takes you at once. Its entry in the Factions tab says whether your house could stand with them, or why not, and, if you are in it, what it still lacks to rise.

### When your lord rises against the crown (very soon in 2.0.0) {#when-your-lord-rises-against-the-crown}

If your house is sworn to a [lord](titles.md) who rises against the crown (a plot for the throne, a plot to break away, or a [charter](factions.md#the-charter) taken up in arms), and your house was not in it and was not asked to ride already, a rider brings you the window **"Your lord raises his banner against the crown"** (or *her*), as soon as you are free on the map, at any time while the war lasts. Your lord is never the ruling house here.

- **"Ride with him"** (or *her*): your house goes over to the rebels with its towns and castles, as a house of the plot would. If the crown wins, you come back marked as a traitor and are [judged](realm-houses.md#houses-marked-as-traitors) with the others.
- **"Stand with the crown"**: you keep your oath and stay, at war with your own lord while the rising lasts. Your lord does not hold it against you: *"many a vassal stands apart in a quarrel with the crown."*

Only you are asked this way: AI vassals weigh their lord when they decide whether to join a plot (see [Who joins, and why](#who-joins-and-why)), and are not asked again when it rises.

### When your realm falls into civil war (very soon in 2.0.0) {#when-your-realm-falls-into-civil-war}

When your realm falls into civil war and your house stays with the crown, as a vassal, a window **"Civil war in {Kingdom}"** tells you once, when you are free on the map, what the rebels want, which houses rose, that your house stands with the crown and the rebels are your enemies now, how the war is decided and what each side's victory would bring. Not if you rule the realm or serve it for pay. From then on, ask any lord *"What is happening in the realm?"* to hear how it goes (see [Asking how things stand](factions.md#asking-how-things-stand)).

### If you are the ruler

- Every wrong your crown does a house costs a little of its head's goodwill toward you (more in a kingdom grown well beyond its fair share), but never your own clan or close kin; with the old discontent on, the size of the realm wears on it too. Your own clan never plots against you, but a brother, son or daughter heading a house of their own has a claim to your throne and may.
- Nobody wins lords back for you: talk to them yourself (*"There is a plot against {your name}. Stay loyal to the crown."*), or send an envoy. A lord you keep loyal stays so for 60 days. Talking the plot's leader out of it ends the plot.
- When the rumour reaches you, ask around, and watch the **Factions** tab, to find who is behind it.
- **You can lose the crown.** If the rebels win, the house they meant to crown rules your kingdom and your house stays on as a vassal.

### Envoys

With [Envoys](envoys.md) you can send a family member or companion to do this talking for you: **"Win a lord over to our plot"** (when you are in one) or **"Keep a lord loyal to the crown"** (when you know of one). An envoy sent to sound a lord out also reports where their house stands on the plot.

## Tips (very soon in 2.0.0) {#tips}

- Conquest has a price at home: past its fair share, every wrong the crown does a house stings more, and its lords plot and band together more readily. At twice its fair share, a lord merely cool toward the ruler may start a plot.
- A plot's leader needs relation −5 or worse with the ruler (up to +5 in a kingdom of twice its fair share), and its pretender +10 or worse. Gaining relation with your discontented lords keeps them from starting one, and keeping on good terms with the strong houses that have a claim leaves a plot nobody to crown.
- Want the crown without a claim of your own? Marry the head of your house to the ruler's brother, sister, son or daughter, or find a claimant house and press its claim for it.
- Watch the **Calculating** lords: they hold back while a plot is small and rush in once it passes 30%.
- A war abroad is no shield: a strong plot may rise in the middle of it. Only a realm that is losing its wars, or small, makes the plotters hold back, and then only somewhat (see [The rising](#the-rising)).
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
- `IndependencePlotEnabled` to `false`: no plots to break away. Numbers you can change: `IndependenceRelation` (−30) and `IndependenceLargeRealmRelation` (−20), `IndependenceRisesAt` (0.3), `IndependenceRisesSureAt` (0.5), `IndependenceStartChance` (0.02), `IndependenceDukeFactor` (1.5), `IndependenceJoinAt` (30), `IndependenceNeighbourFiefs` (4); the rest on the [Settings](../settings.md#kingdoms-and-court) page.
- `CivilWarBriefingEnabled` to `false`: no window when your realm falls into civil war.
- `InternalWarWeaknessEnabled` to `false`: a realm weak in its wars abroad no longer holds its plots back (nor its other quarrels, see [Factions and grievances](factions.md)). Numbers you can change: `InternalWarWhileLosingFactor` (0.3), `InternalWarWhileAtWarFactor` (1, for a realm at war that is not weak), `InternalWarSmallRealmBelow` (0.5).

