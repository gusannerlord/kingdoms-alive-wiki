# Civil war

Any kingdom can rot from within, and the larger it grows, the more ambitious and rancorous its lords become. Lords wronged by the crown lose patience with the ruler, a discontented clan starts a plot to put another house on the throne, and if the plot grows strong enough it raises its banner and the realm splits in a civil war. A house that defies the crown and is named traitor raises its banner too. You can join a plot, lead one, urge a lord to press his claim to the crown, ride with a house that breaks away, work against them, or, if you wear the crown, fight to keep it.

## How large a kingdom is {#how-large-a-kingdom-is}

The mod compares each kingdom with its fair share of the map: all the towns and castles held by kingdoms, divided by the number of kingdoms. Kingdoms already destroyed still count in that number. Kingdoms born from a rising never do, so one civil war does not make every other realm look larger.

### Great realms, restless lords {#great-realms-restless-lords}

The larger a kingdom grows beyond its fair share, the more ambitious and rancorous its lords become. At its fair share or below, nothing changes; above it, the effects grow steadily and are full once the kingdom holds twice its fair share.

- Every [grievance against the crown](factions.md#lords-remember) weighs more when it is born, up to twice as much, and so does the goodwill toward the ruler it costs.
- A lord needs less bad blood with the ruler to [start a plot](#who-starts-one): in the greatest realms, a lord merely cool toward the ruler may start one.
- A house needs less to join a plot against the crown, and less still to join a [charter or a reckoning](factions.md).
- A house needs a smaller grudge to begin a [Reckoning](factions.md#the-reckoning-of-a-house).
- In the greatest realms, a house in a plot against the crown holds on to it a little longer before it gives up on it.

Grievances one house holds against another do not change with the size. A kingdom that shrinks back calms down at once for what comes next; what has already happened stays.

### "Too large" {#too-large}

A kingdom is **too large** once it holds a good deal more than its fair share; it need not reach twice it. This only counts for the old discontent below (off by default), for a clan without towns or castles weighing a plot (see [Who joins, and why](#who-joins-and-why)) and, if you turn on `PlotsOnlyInLargeRealms`, for where the AI may plot.

## Discontent (off by default) {#discontent-off-by-default}

This is off unless you turn it on (`RealmDiscontentEnabled`): lords turn on their ruler through what the crown has done to them (see [grudges against the crown](factions.md#lords-remember)), not for the size of the realm alone. With it on:

- In a kingdom that is too large, every vassal clan leader slowly thinks less of the ruler, **you included**, the more so the larger the kingdom. It does not reach the ruler's own clan, the ruler's close kin (parents, children, brothers and sisters, husband or wife) or mercenaries.
- **It stops at a limit that grows with the kingdom.** A kingdom that keeps growing wears its lords down further; one that shrinks gives back what is over its new limit, little by little. It never drags anyone deep into hatred of the ruler, and lords who already hate the ruler lose nothing more from it. Size alone rarely turns lords against a ruler badly enough for a civil war; [quarrels between clans](clan-events.md) and other grudges do the rest.
- A [Chancellor](royal-court.md#the-offices) softens it.
- Every so often you see a yellow message. As a vassal: *"{Kingdom} has grown too large to be ruled well. {ruler} has no time for lords like you any more, and your regard for your liege keeps wearing away."* As the ruler: *"The lords of {Kingdom} grumble that the realm has grown too large to be ruled well: {N} houses think less of you."*
- **Recovery:** once the kingdom is no longer too large, or while it rests after a civil war, each clan leader slowly gets back what the discontent took, and never more. That is lost if the ruler changes, the clan gets a new leader, or the clan leaves the kingdom.
- During a civil war nothing is lost and nothing comes back.

## How a plot starts {#how-a-plot-starts}

Every plot against the crown has two houses at its head, and they may be the same (a [plot to break away](#plots-to-break-away) has rules of its own):

- the **leader**, the house that starts the plot, gathers the lords and, if it comes to it, raises the banner;
- the **pretender**, the house the plot would put on the throne.

### Claims to the throne {#claims-to-the-throne}

Only a house with a **claim to the throne** can be a pretender. The claim belongs to the house and is judged with whoever heads it today: if the head dies, the new head may keep the claim or lose it. A house has a claim when:

- **its head is close kin of the ruler** while leading a house of their own: the ruler's father or mother, son or daughter, brother or sister, husband or wife;
- **it married into the royal house**: its head's husband or wife is close kin of the ruler;
- **it once ruled the realm**: a house that wore this crown before, for example one deposed in an earlier civil war or one that lost the throne in a vote;
- **the law of the realm counts it among the worthy**. Under a law that has the lords choose among the heads of houses (Senate, Acclamation, Tanistry, Shura, Thing, Feudal Elective, Veche, Rule of the Strongest; by custom, the Northern and Western Empire, Battania, the Aserai and the Nords), the three houses with the best [claim to rule](succession.md#what-makes-a-claim), besides the ruler's own, have a claim too;
- **it is among the mightiest of the realm**. Under a law of blood and under the Kurultai (by custom, Vlandia, Sturgia, the Southern Empire and the Khuzaits), the two houses with the best claim to rule, besides the ruler's own, have a claim too.

The ruling house itself never plots. Every civil war the rebels win adds the deposed house to those that once ruled, so claims grow with the realm's history.

In the realms of the Empire, a strategos may also plot a **coup**, a plot of its own kind with its own rules: see [The Empire's own ways](empire.md).

The houses with a claim are listed under **The Crown** in the Crown tab of the kingdom screen, and on each clan's page in the Encyclopedia (see [The crown and its claim](succession.md#where-you-see-it)).

### Who starts one {#who-starts-one}

Every week, in every kingdom, the AI clan leaders may start a plot. Any vassal house can start one if:

- its leader is on bad terms with the ruler, or merely cool toward him in a realm grown far beyond its fair share (see [Great realms, restless lords](#great-realms-restless-lords)); a house whose claim is better than a [weak](succession.md#what-a-claim-does) ruler's needs less bad blood still;
- it is not the ruling house nor a mercenary, is not already in a plot or a [faction](factions.md), and has given its word to no side at the moment, neither to the crown nor to a plot (see below).

No plot starts in a kingdom that is the vassal of another, during a civil war or in the calm after one, or while the kingdom already holds three plots; and at most one new plot is born in a kingdom each week.

A house needs no strength of its own to start a plot. The ruler's brother or son heading another house can start one too: he is the classic pretender.

A calculating leader is likelier to start one, an honourable one far less.

### Who it would crown {#who-it-would-crown}

A pretender needs a claim to the throne, a house of real strength (judged by the Clan Strength shown on the clan's page in the Encyclopedia), and no warm regard for the ruler: a lord who is merely cool toward the ruler will still take the crown if it is offered.

- If the house that starts the plot can be crowned itself, it is its own pretender. The plot then starts only if at least one other clan would join it straight away.
- If not, the plot is born together with the house with a claim that leans to it most, weighed like any lord deciding whether to join (see below), with the plot's leader as the man asking and the crown it would wear in the balance. That house joins at once as the plot's first member.
- If no house with a claim would have it, there is no plot. Nobody is ever forced.
- **A crown offered in secret.** Your house is weighed like any other. If it fits the lord best, he writes to you in secret (**"A crown offered in secret"**), in his own voice, with the reasons that truly moved him: your house's right to the throne and its strength, and what weighed most (your friendship, your quarrel with the ruler, a weak claim on the throne, kinship, faith, allies already in the plot...). Accept, and the plot is born to crown your house; burn the letter, and he looks elsewhere.

**The pretender is fixed** for the life of the plot: it is never replaced by another. If the pretender's house dies out, leaves the plot, leaves the kingdom or turns mercenary, comes to the throne, or **loses its claim**, the plot ends. A claim can be lost when the ruler dies and the new one is not kin, when the husband or wife who tied a house to the royal one dies, or when a house slips from among the worthy or the mightiest; once a house is a pretender, it keeps such a claim as long as it stays near the top of the realm's claims.

### Several plots at once {#several-plots-at-once}

A kingdom can hold **up to three plots at once**, each behind its own pretender. A house is in one plot at most, the one it leans to most, and goes over to another only if it leans to it clearly more (a house that gave its word stays where it swore). The house a plot would crown never goes over to another plot. The **first plot to rise ends all the others**.

A house whose plot has ended may start another whenever it likes, with no wait. No new plot starts in the calm after a civil war.

A [vassal realm](vassal-realms.md) never has a plot or a civil war: a plot under way dies quietly when its realm bends the knee. And no realm becomes a vassal while either side is in a civil war.

## Who joins, and why {#who-joins-and-why}

Every week, each clan leader of the kingdom weighs every plot. The ruler's own clan never joins. The rest weigh:

| What counts | How |
|---|---|
| Their regard for the plot's leader and its pretender | for or against; when the two are different houses, both count (the one who asks and the one who would reign) |
| Their regard for the ruler | the other way: liking the ruler holds them back, hating the ruler pushes them in |
| Devoted to the ruler | such a house can still be won, but only by a much stronger cause. The same holds for you when you ask to join a plot |
| Honor | holds them back |
| Calculating | only a calculating lord sides with the winner: drawn in once the plot holds a fair part of the realm, put off while it is small |
| How big the plot is | the bigger, the stronger the pull |
| Clan without towns or castles | pulled in, only while the realm is [too large](#too-large) |
| Close kin or in-law of the plot's leader or of its pretender | a strong pull |
| Being the plot's pretender | a pull (the pretender weighs only the leader, not himself) |
| Swore the [oath of fealty](royal-court.md#the-oath-to-a-new-ruler) to the current ruler | holds them back for a while |
| Refused that oath, or let the time pass | a strong pull for a good while |
| [Grievances](factions.md) against the crown | a pull, the more the house resents it |
| [Grievances](factions.md) against the plot's leading house, or the house it would crown | holds them back, the more the house resents it (the heavier of the two counts, not both) |
| Your house's [lord](titles.md) leads the plot or is in it | a strong pull (nothing among the Khuzaits, who all owe the khan before their noyan) |
| That lord stays out of it | holds them back |
| That lord is the crown itself, as the house's count or duke | holds them back hard |
| Of another faith than the ruler | a pull |
| The plot would crown a house of another people than the lord's own | holds them back hard (not for the plot's leader nor the house it would crown; your plots too). It also counts when a lord weighs leaving the plot |
| The ruler refused lately to [step down](factions.md#asking-a-ruler-to-step-down) | a pull for a while |
| The [claims](succession.md) of the plot's pretender and the ruler | a pull when the pretender's claim is the better one; holds them back when the ruler's claim is beyond question |

What a house owes its lord counts for nothing once its head is on very bad terms with that lord, and less the more the house holds against him.

**A house promised the crown.** A house that a peace named heir, or to which the votes were pledged, waits for that promise: it joins no plot or charter of another house, is not courted for one, and leaves one it was in. It may still lead a plot of its own.

When the weight of it all is enough, the lord **joins**. In a large realm, less is enough: the wider the realm, the more readily lords band together against the crown. A lord who has joined does not walk out over a passing chill: he **leaves** only once his leaning has fallen well below what it took to join him, and in the greatest realms it must fall further still. A pretender who is not the plot's leader weighs it the same way each week: if he leaves, the plot ends.

"The realm's strength" here means the Clan Strength of all its vassal clans together, the ruler's clan included and mercenaries left out. The plot's **share** is the part of that held by its clans.

**The plot's leader recruits.** Each week an AI plot leader tries to win over one undecided lord who is already close to joining, the closest of them. A lord further from it will not hear of it, from the AI or from you. Who the leader is moves them a little: a fine speaker, or one whose character sits well with the lord's, does better; a poor speaker, or one whose character grates, does worse. Charm helps, but a lord's own grudges and leanings weigh far more. At the same feast or the same [hunt](hunts.md) the odds are better. A lord won over this way stays in the plot for a while at least. Once the plot holds most of the realm, the leader stops recruiting (lords may still join by themselves).

**At a hunt.** An AI plot leader who hosts a hunt likes to invite wavering lords. On the last day of the hunt they try once to win over each wavering guest who came, with better odds. A member of the plot who hosts a hunt sometimes tries too. An AI ruler who knows of the plot and hosts a hunt tries to win back each guest who is in it, except its pretender.

**The ruler wins lords back.** Once the plot has grown to a real danger, an AI ruler tries each week to win back the member who is least committed, never the leader, the pretender, a house that swore to the plot lately, nor you. The deeper the lord is in it, the harder. A lord won back leaves the plot, thinks better of the ruler and stays loyal for a good while. If you are the ruler, this is your job (see below).

## Rumours

When a plot has gathered a fair part of the realm's strength, and you are a vassal of that kingdom outside the plot, you hear: *"There is talk of a plot among the lords of {Kingdom} against {ruler}. Who is behind it, nobody will say."* If you are the ruler, it says "against you". From then on you know a plot exists, but not who leads it or who is in it.

## How a plot dies

- **It never grew:** a plot that does not gather a real share of the realm in its first months comes to nothing.
- **It stalls:** a plot that goes a long while without holding enough of the realm to rise gives up. Yours too: the journal tells you how long you have, the houses of your plot warn you when time is running short, and if it falls apart you are told why.
- **The realm shrank (AI plots only, and only with `PlotsOnlyInLargeRealms` on):** once the kingdom has been back below "too large" for some months, it ends. By default a kingdom that shrinks does not end its plots.
- **The leader is gone:** the leader dies, is replaced at the head of the clan, leaves the kingdom, becomes a mercenary or comes to the throne.
- **The pretender is gone:** the pretender's house dies out, leaves the plot, leaves the kingdom, becomes a mercenary, comes to the throne or loses its claim (see [Who it would crown](#who-it-would-crown)).
- **The leader or the pretender is talked out of it** (by you, see below).

If you knew of it you see *"The plot among the lords of {Kingdom} has come to nothing."* If you were in it and its pretender fell, you are told instead that there is no crowning that house now, and the plot falls apart; if the plot was crowning you and your house lost its claim, you are told that the lords no longer hold your house has any right to the throne.

## The rising {#the-rising}

An AI plot may raise its banner when **all** of this is true:

- it holds about half of the realm's strength. From there it is a matter of nerve: each week there is a chance it rises, small at first and growing with its strength, and once it holds well over half the realm it always rises;
- it is some weeks old and has at least one clan besides its leader's;
- with `PlotsOnlyInLargeRealms` on (off by default), the kingdom is too large, or was very lately;
- at least one house of the plot holds a town or castle, and the crown keeps at least one of its own;
- the kingdom is not already in a civil war (several kingdoms may each have their own at the same time).

**A war abroad does not stop it.** A plot may rise while its realm fights another kingdom. But a realm that is **weak in its wars** makes the plotters think twice: while it is at war and either losing (the same mark as when an AI realm [turns to the defence](command-your-armies.md)) or small next to the average realm, every chance of a rising is cut to a fraction of what it would be, even for a plot that would otherwise surely rise. A realm that is losing but still **dominant**, far above its [fair share](#how-large-a-kingdom-is) of the map, is not held back. At peace, or at war and not weak, nothing changes.

**A battle only delays it.** If men of the plot's houses are in the thick of a battle when the plot decides to rise, the rising waits for the fighting to end, a day at most, and then goes ahead.

**A fief taken can set a plot alight.** When a house of a plot is to lose a town or castle (to a decree of the crown, a reckoning judged at the [assembly](assembly.md), its lord's demand, a sentence of the assembly or the khan's claim), or is judged as one of the [traitors](realm-houses.md#houses-marked-as-traitors):

- if a strong part of the realm stands behind the plot, the house will not give it up and the plot **rises within the hour** (at once after a decree);
- with less behind it, it depends on the head of the house and on the plot's strength: the stronger the plot and the bolder the head, the likelier it rises all the same; a calculating head holds back. If it does not rise, the house may still break with the realm alone (leaving the plot), or else it bows and yields;
- after [a fief taken for nothing](royal-court.md#a-fief-taken-for-nothing), a seizure by the crown, the plot rises surely with less of the realm behind it, and the other houses weigh it more readily still;
- in a realm weak in its wars abroad (above), each of these chances, the sure one too, is cut down.

Before such a rising, every house of the realm that is free to choose weighs the plot once more, angrier for what happened: more so if it is kin or friend of the house wronged, or already holds a grievance against the crown. Those who are won over ride with the plot.

Such a rising still needs at least one house besides its leader's once the others have weighed it (if none comes, the house answers again without that choice: it breaks alone or yields), a town or castle among them, and a crown that keeps one of its own; never two civil wars in one realm at once, never in a kingdom that is the vassal of another, and not while you are in the plot during a story quest. If the house is yours and the plot can rise then, you choose: bow, raise the plot's banner, or break with the realm alone. If you lead the plot, you are asked whether to raise the banner now; if you are one of its houses, whether you ride with it. As ruler or loyal vassal, you are told when it happens. Turn it off with `PlotStripRisingEnabled`.

When it rises:

- The plot's leader founds a **new kingdom**, named *"{Clan} Pretenders"* after the house it would crown, with the leader's culture and emblem, on a banner of its own colours, distinct from the realm it rose against (if you lead the rising, your clan keeps its own colours). It claims the throne and is at war with the crown at once.
- Every clan of the plot goes over with its towns, castles and villages, keeps its influence, and may not leave it for a good while. Nobody leaves a rebel realm while its war lasts, you included.
- The news says whom the rising would crown when it is not its leader: *"{Leader} of the {Clan} has raised the banner against {ruler} to crown {pretender} of the {Clan}! Civil war in {Kingdom}."*
- You are told in the middle of the screen, wherever it happens: *"Civil war: {Leader} of the {Clan} has raised the banner against {ruler}, ruler of the {people}."* (or *"Civil war in your realm: ..."* in your own kingdom). If you led the rising, were in the plot or were asked whether you ride with it, you already know and get no extra notice.
- The log keeps a red line with the news and the houses that went over to the rebels.

## A house that breaks with the realm {#a-house-that-breaks-with-the-realm}

A house that defies the crown and is named traitor does not slink away: it **raises its banner against the king**, and that is a civil war like any other, led by that house, with no plot behind it. It happens to a house that defies the taking of a fief and is not let off (see [Yield or defy](factions.md#yield-or-defy)), defies the crown's ban on a feud or a [right the crown has judged](factions.md#a-right-the-crown-has-judged), will not lay down its arms in a feud when the crown calls the houses against a foe at the walls, defies a sentence of the [assembly](assembly.md), refuses the crown's judgment of a [traitor](realm-houses.md#houses-marked-as-traitors), its banishment or its expulsion, or will not serve a realm that swallowed its own (that house fights to break away with its lands, as a [plot to break away](#plots-to-break-away) would). It is what happens to you, too, when you renounce your oath in any of those windows, or leave your kingdom keeping all your holdings.

- **The rising.** The house founds a rebel kingdom, *"{Clan} Pretenders"*, on a banner of its own colours, and is at war with the crown at once. Every plot of the realm ends, the war takes the realm's one place for a civil war, and a calm follows it like any other. A house breaks even in the calm after a civil war. If the realm is already in a civil war, the house goes over to the rebels with its lands instead.
- **Another king.** Very rarely, a house on bad terms with its own ruler and on good terms with a king at war with him goes over to that king with all its fiefs instead, hardly ever to one far away, and the less often the more honourable its head.
- **A house with no town or castle** rises only if a house with one rides with it. Otherwise it leaves the realm alone, at war with it, and makes its peace later as any house without a realm does, at the [peace table](war-and-peace.md#terms-of-peace), paying once for it if it must.
- **Who rides with it.** The houses sworn to it as their lord, its kin, its allies and the houses of a plot against that king each weigh riding with it when it rises: how just its cause looks (a fief taken for a house with no right to it, or a seizure with no cause, is the crown's wrong; a lawful sentence or a claim with no right behind it is the house's own; kin care far less, since blood weighs more than law), how strong the rising looks against the crown, their regard for the king and for the house that breaks, their honour (the oath they swore) and their grievances against the crown. A vassal is readier than kin, but weighs his oath to the king too. Never a house on the other side of the quarrel that caused it, a house that gave its word to the crown, a sellsword or a [landed knight](landed-knights.md) (he rides with his lord). While the war lasts, those who stayed home weigh it again when the tide turns or their feelings change.
- **What breaking costs.** Every house of the realm it leaves thinks much less of it.
- **How it is fought.** The war turns on the place the house broke over: the fief it refused to give up, or the one its cause was about (see [Winning the civil war](#winning-the-civil-war)).
- **If the peace has the ruler lay down the crown, the houses that rose choose the king** among themselves, each by the right to the crown of each head, its own house, kinship and regard. You cast your house's voice in a window, **"The crown of {Kingdom}"**. A peace that only names an heir names the rebel house with the best right to the crown that day.
- **If the crown wins**, or makes a peace that grants no pardon, it is as for any rising: the head of the house that broke is condemned and every house that rose comes home [marked as traitor](realm-houses.md#houses-marked-as-traitors).
- **The fief it broke over**, if it was being taken for another house, goes to that house whenever the crown has it back: retaken in the war, sent back by the peace or taken by the judgment (see [A house that breaks with its realm](realm-houses.md#a-house-that-breaks-with-its-realm)).

## Winning the civil war {#winning-the-civil-war}

A civil war is decided by the game's own **war score**, on the Diplomacy tab, as every war is (see [The war score](war-and-peace.md#the-war-score)). Within a realm the battles, sieges and raids are measured against the whole realm as it stood when the war began, so one castle taken counts for what it is worth to the realm, not for the whole of a lesser side. Two more lines count:

- **Prisoners**: the lords of the other side your side holds captive, its ruler or its leader most of all. A lord who escapes or is freed takes his part with him. Taking the king or the rebels' leader does not end the war by itself.
- **Objective**: what this war is fought for, named on the line. Each day the side that meets its war's objective gains ground, the side that has to take it faster than the side that already held it, up to a limit; if the objective changes hands, the ground goes back first.

| The war | The rebels gain ground while... | The crown gains ground while... |
|---|---|---|
| A plot for the crown (and a coup) | they hold the realm's seat (the ruling house's own, or the realm's richest town) | it holds its seat and has won back a good share of the towns and castles the rebels rose with |
| A plot to break away | they keep the great part of the towns and castles they rose with | it has won back much of them (in between, nobody) |
| A charter taken up in arms | they keep the great part of the towns and castles they rose with | it has taken a good share of them |
| A house that broke with the realm | they hold the place it broke over | it holds that place |

**Your journal.** If your house is on either side, an entry, **"The stakes of the war with the {enemy}"**, tells you what the war turns on and where (the place is marked on your map), who meets the objective today, a new line each time that changes, how ready both sides are for peace, and, at the end, how it went for your side.

**No time limit.** A civil war has no set end in days. It ends in a peace (below), or at once when one side is left without a single town or castle: rebels with nothing left have lost, as if the crown had crushed them; a crown with nothing left has lost its throne. Nothing is settled while you are in a battle or siege on either side; it waits for the fight to end.

### Peace in a civil war {#peace-in-a-civil-war}

Nobody is ever made to take a peace, and a peace follows the course of the war:

- **The first weeks.** Blood runs too hot: no talk of peace at all, unless one side is crushed.
- **Peace can be talked of.** Either side may set out terms, and the other must truly want them. So soon, no peace is made for nothing: the terms must give the side ahead something, if only a sum in silver, and while the two sides stand even there is no peace yet.
- **The war drags on.** The lords of both sides grow weary of it, and a peace is more welcome than it was, above all to the side behind. A peace that gives the side ahead nothing is possible again.
- **Both sides are sick of it.** Their lords want it ended more than they want to win it.

At any time the side behind wants peace more the further behind it falls, and badly once it is crushed; the side ahead takes a peace only if it suits it, and a side close to winning more waits a little for it. A side that has lost every town and castle cannot make peace: it has lost.

**At the table.** Every peace of a civil war is made on the [Terms of Peace](war-and-peace.md#terms-of-peace) screen, as between realms, with the crown on one side and the rebels on the other. Nothing comes of the war score by itself: the two sides agree each term.

- **Where.** In the Diplomacy tab of the kingdom screen, choose the war and press **Negotiate terms** (the game's own way of proposing a peace is gone here too); or speak to the ruler of the other side in person; or, if you lead your side, send an [envoy](envoys.md) with your terms. The AI's terms reach you by courier.
- **Who sets terms.** The head of each side (the ruler, or the rebels' leader) sets any terms, at no cost. A lord who does not lead his side may only put a pardon, or a modest sum in silver, before its council, and pays the game's influence for proposing a peace; an AI house does the same.
- **Both councils vote**, the crown's and the rebels', house by house, and each side's leader has the last word over his own. The leader of a side never votes against terms he has accepted himself; a house that would hand over a town or castle by the terms votes against them.
- **Refused terms** are not put again between the two sides for a while, a shorter while the longer the war has lasted, and once both sides are sick of it new terms may follow at once.

## The terms of a civil war {#the-outcomes}

What each kind of war can bring, term by term. Terms that do not fit the war, or the way it stands, are greyed on the screen with the reason.

| Term | Wars | What it brings |
|---|---|---|
| **A pardon** | every civil war | The rebel houses come home under the crown's pardon, none of them a traitor |
| **The crown after this reign**, or **votes pledged** | a plot for the crown, a coup, a house that broke with the realm | The ruler keeps the throne, and when the reign ends, by death or otherwise, it passes to the rising's house, whatever the law (after a house broke with the realm, the rebel house with the best right to the crown that day); in a realm that chooses its ruler, the crown's house and the houses that stood by it give that house their votes at the next choice. The pardon comes with it |
| **The crown laid down** | the same | The ruler steps down and the pretender's house is crowned; after a house broke with the realm, the houses that rose choose among themselves. A rising led by a house of another culture or faith than the crown's goes its own way instead, as **a kingdom of their own** |
| **The charter** | a charter taken up in arms | In four steps: its first clause alone; the whole charter; the whole charter, binding the crown for longer; and, besides, a seat at court for the head of the house that led it. Anything beyond the first clause carries the pardon |
| **A realm of their own** | a plot to break away | In three steps: a [vassal realm](vassal-realms.md) with all they hold, sworn to the crown; independence with the lands around their seat; independence with every town and castle they hold |
| **The fief broken over** | a house that broke with the realm over a fief | The fief goes to the house that broke, or back to the crown, and from the crown to the house it was being taken for, if one was named |
| **A sum in silver** | every civil war, from either side | Modest, heavy or great, paid once as the peace is sealed by the houses of the side that pays, each by its rank, never from the treasury, into the purse of the other side's ruler. If they can no longer raise all of it, there is no peace |

No tribute, and no town or castle but the one fought over, changes hands at the peace of a civil war. In every peace that brings the realm back together, what the rebels took from the houses that stood by the crown goes back to them.

**Without a pardon.** A peace with no pardon, where the crown keeps its throne, leaves every house that rose to be judged by the crown, as when the crown wins (below). The crown that lays down its crown, lets the rebels go their own way, seals the whole charter or names an heir from the rising judges nobody; with the charter's first clause alone, it still may. The side that would be judged weighs a peace without a pardon as heavily as the heaviest terms.

### What the AI gives and asks {#what-the-ai-gives-and-asks-in-a-civil-war}

- **It gives only what the war score has earned:** little when it is somewhat behind, more when clearly behind, the most when crushed. A peace that leaves its houses to be judged is the heaviest thing it can give: only a crushed side of the AI takes it. You may always give more than the war asks of you.
- **The side ahead asks for something.** A side well ahead that holds what the war is fought over keeps it by the terms: the fief broken over, or, in a plot to break away, the seat it rose around. A clear win asks at least the lighter form of the war's own stake (an heir or the pledged votes, the charter, a vassal realm, the fief broken over); a crushing win asks the stronger form (the crown laid down, the whole charter, independence). It asks only what the other side could give, and silver only fills out the rest. As the war drags on a side ahead asks less, but a crushing win still asks the stake. At your table the AI leader tells you what is missing: *"There will be no peace without the charter sealed whole."*
- **The AI makes its peace at the same table**, against you or against itself. When the side ahead is clearly the stronger it names its price; otherwise the side behind, once it wants a peace, offers the least the other side would take, what the war is about before silver, and only terms both councils would pass.

**The rebels win** (by a peace in which the ruler lays down the crown, or because the crown has nothing left). The **pretender's** house becomes the ruling clan of the old kingdom, even when another house led the rising (if the pretender's house is no longer with the rebels, the rebel kingdom's ruler takes the crown instead). Every rebel house comes back into it, and the rebel kingdom disappears. The old ruler thinks much less of the new one. If that ruler was you: *"You have lost the throne of {Kingdom}. {New ruler} of the {Clan} now rules; your house remains as a vassal."* If you were the pretender and win, you are told the crown of the kingdom is yours; if you led the rising for another house, that house is crowned and you return as its vassal. The new ruler is a usurper, his claim stained for a while (see [The ruler's own claim](succession.md#the-rulers-own-claim)), and a new ruler means a new [oath of fealty](royal-court.md#the-oath-to-a-new-ruler): the houses that stayed loyal to the old crown are much less willing to swear to the winner.

**The crown wins** (by a peace that grants no pardon, or because the rebels have nothing left). Every rebel house comes back to the realm with its towns and castles, each thinking much less of the ruler (hired mercenaries of the rebels simply leave). The crown gives back to its loyal houses the towns and castles the rebels took from them. The head of the house that led the rising is put to death (a merciful ruler may spare the life; as ruler you choose), and every house that rose is marked as traitor for a while: the ruler judges them one by one by decree, hardest on the house that led the rising. Few dare to defy the judgment, and a house stripped of its land may leave the realm instead. For a while, whatever the judgment, the houses that rose get no new land and no house holds of them, and one that comes home with no town or castle loses its duchy or ulus at once. See [Traitors and the houses of a realm](realm-houses.md#houses-marked-as-traitors).

**Two kingdoms.** Only when the ruler lays down the crown at the peace, and the house that led the rising is of **another culture or another faith** than the crown, does the realm stay split: the rebels keep what they hold, and an AI rebel kingdom drops "Pretenders" and becomes *"Realm of the {Clan}"*, after the house that rules it. A plot to break away has its own terms above. The heir or the pledge shows in the kingdom screen, and your journal tells you the terms of the peace when the war ends.

**Afterwards:** every kingdom that comes out of a civil war gets a long **calm**: no new plots, [factions](factions.md) or feuds (and, with the old discontent on, no discontent, while the discontent of the past slowly mends). You are told when it begins in your realm, and the Realm tab reminds you while it lasts.

## Plots to break away {#plots-to-break-away}

Not every plot wants the crown. Houses that have had enough of their ruler, and whose lands lie together, may plot to **leave the realm with their lands** and stand as a realm of their own: a great duke and the lords around him, for example. Such a plot is rare and hard to grow, and likelier in a large realm.

**No one is talked into it, or out of it.** A house is in it only by its own leaning. Its leader courts no one, the ruler wins no one back, you cannot persuade a lord to join or to stay loyal (those lines are not offered for it, and an envoy cannot do it either), and a hunt changes nothing. A house in such a plot will not be talked into any other cause either.

**Who can be in it.** Every house in it, its leader too, must:

- hold a **town or castle**, and not be the ruling house;
- be on **bad terms with the ruler**, though a large realm asks somewhat less (see [Great realms, restless lords](#great-realms-restless-lords));
- hold a town or castle in the **lands of the plot** (below);
- be in no [faction](factions.md) or feud, and have given its word to no side.

**The lands of the plot.** They grow from the **seat** of the house that leads it (a duke's most prosperous town in his own duchy; else its most prosperous town; else its best castle) and take in every town and castle of the plot's houses that **touches** them, one after another. Two towns or castles touch when one is among the nearest to the other on the map and no town or castle of a house outside the plot lies between them; a town on an isle touches none. A house's other holds may lie apart: they do not keep it out, but they stay with the old realm if it breaks away. If the house that leads it loses its seat, the plot gathers around another of its holds.

**How it starts.** Every week, each AI house that could be in one may start a plot to break away: rarely, likelier for a calculating head and less for an honourable one, likelier in a large realm and for a duke (or a strategos or noyan, see [titles](titles.md)). It needs no other house to start. **One** such plot at a time in a realm, besides (and not counted among) the three plots against the crown. None in a kingdom that is the vassal of another, during a civil war or in the calm after one.

**Who joins.** Every week each house that could be in it weighs it much as it would [a plot against the crown](#who-joins-and-why) (its regard for the leader and the ruler, its character, grievances, kin, allies, its lord), with no pretender to weigh, and a pull of its own for a house of another culture than the ruling house. In a large realm less is enough to join, and a house holds on to it longer. A house leaves once it is no longer on bad enough terms with the ruler (it has made its peace with the crown, a new ruler came, or the realm shrank and asks more), or when none of its holds touch the plot's lands any more, or when its leaning falls too low, as for any plot; the leader's peace with the crown, or the loss of all its holds, ends the plot. If you are in it, each house that joins or leaves writes to you, with its reason when one stands out.

**How it dies.** A plot that does not gather a real share of the realm in its first months comes to nothing; one that goes a long while without being strong enough to rise gives up.

**The rising.** It rises with less of the realm behind it than a plot for the crown, with at least **one other house** beside its leader, and under the other rules of a [rising](#the-rising): one civil war at a time, a war abroad no hindrance except in a weak realm, and a fief taken from one of its houses sets it alight, as for any plot. An AI plot waits some weeks; then each week there is a chance it rises, growing with its strength, and past a point it always rises. The rebels fight as the **League of the {Clan}**: *"{Leader} of the {Clan} has raised the banner against {ruler}: the houses with him mean to break away from {Kingdom} with their lands! Civil war in {Kingdom}."* The war is won and lost as [any civil war](#winning-the-civil-war), and its peace is set out at the table with terms of its own (see [The terms of a civil war](#the-outcomes)).

- **A realm of their own:** they stand as the **Realm of the {Clan}** after its ruling house (a realm you rule keeps the name you gave it). With independence and their core they keep the lands around their seat, and their towns and castles that lie apart go to the old ruler, to be shared out by its council; with independence and all they hold, they keep everything. If the crown is left with no town or castle at all, the rebels take its throne instead, as in any civil war.
- **A vassal realm:** they stand as a realm of their own with all their lands, sworn to the crown as its vassal.
- **The crown wins**, or makes a peace that grants no pardon: as for any rising, the head of the house that led it is put to death (unless the ruler spares him) and the rebel houses come home [marked as traitors](realm-houses.md).

## Other kingdoms stay out

While a civil war lasts, other AI kingdoms are reluctant to attack either side:

- they need a much stronger reason than usual to declare war;
- they weigh each side as if part of the other side's strength stood with it;
- they never see the civil war as a chance to retake lost lands.

It is not impossible: a kingdom with a strong grievance may still attack. In the council you may hear *"they are at war among themselves, and we will not meddle in it"* or *"their rivals in the civil war would be the ones to gain"*. None of this holds back a kingdom you rule, nor an ally of one side attacking the other.

### Alliances in a civil war {#alliances-in-a-civil-war}

- **The rebels swear no alliance.** While a civil war lasts, the realm of those who rose (by a plot, a coup, the charter, a plot to break away or a house that broke with the realm) neither offers nor accepts an alliance with another kingdom, and none can be offered to it: in the Diplomacy screen the choice is greyed with the reason. With no ally, it calls no one to its wars and is called by no one. An alliance it already held is undone when the campaign is loaded.
- **The crown answers few calls.** A ruler of the AI fighting his own rebels answers an ally's call to war by his own judgement, not for gold: he joins only a war he would think worth fighting for his realm on its own, and mostly refuses, however well paid. Nothing is paid when he refuses. When you call such a crown, you are told if it will not answer; an [envoy](envoys.md) sent to ask it finds that war greyed in his list, and its lord says so before naming any price. He is never barred from answering, and he may still call his own allies, against the rebels too, and make new alliances.
- **Refusing costs nothing.** While a crown fights its own civil war, turning down an ally's call costs it no goodwill with the ally, for you and the AI alike. If you wear that crown, you still choose whether to answer. If your realm is that crown and the AI rules it, its ruler may refuse whatever the council said, and you are told. The calls between an overlord and its [vassal realm](vassal-realms.md) are not touched.

## Your part in it

Everything below needs you to lead your clan as a vassal (not a mercenary) of the kingdom, and neither you nor the lord you talk to can be a prisoner. You talk to clan leaders of your own kingdom: choose *"There is something I'd like to discuss."* and the plot options appear among the others.

### What you can say to a clan leader {#what-you-can-say-to-a-clan-leader}

| You say | When it appears | What it does |
|---|---|---|
| *"{Ruler} is leading this realm to ruin. Would you stand with me if it came to it?"* | You are not of the ruling house, you are in no plot, and the lord is not of the ruling house. | Starts **your own plot**, with **you as its pretender**, and tries to win this lord over. Not offered if your house has no claim to the throne, if your house is too weak to be crowned, or if the realm is in its calm after a civil war. If you spoke to this lord about it too lately, they tell you their answer has not changed. If the realm already holds three plots, the lord answers *"Hush. You are not the first to say so..."* and you learn that they exist. |
| *"Your house has a claim to the crown. Will you press it?"* | You cannot be crowned yourself (no claim, or too weak a house), you are in no plot, and the lord's house has a claim. | Persuades the lord to **press his house's claim**, with you leading the plot. Not offered if his house is too weak to be crowned, or if the realm is in its calm. If you spoke to him too lately, he tells you his answer has not changed. A lord who likes the ruler will not hear of it. If you win, the plot is born at once: you lead it, his house is its pretender and first member, and it stands by your plot for as long as the plot lasts (it falls only if the house dies out, loses its claim, leaves the realm or is talked out of it). |
| *"There are those of us who mean to set this realm right. Join our cause."* | You are in a plot, your own or an AI lord's. | Persuade the lord to join. A lord who agrees tells you what truly moves him (his grudge against the ruler, his love for you or the pretender, his faith, his own claim...), or gives no reason at all when nothing stands out. |
| *"There is a plot against {ruler}. Stay loyal to the crown."* | You know of a plot and are not in it. | Persuade the lord to stay out of it, or to leave it. A lord already in the plot never gives it up at a word: he must truly be argued out of it. If you convince the plot's leader or its pretender, the whole plot falls apart and that lord stays loyal for a good while. |
| *"There is talk of a plot. Where does your house stand?"* | You know of a plot, are not in it, and do not know this lord's stance. | A lord who likes you tells the truth; any other may, the likelier the better your Charm. Ask the same lord again within the week and you get nothing but *"Plots? I know nothing of plots..."* A member names the leader; a leader admits it; a pretender admits that it is his house the plot would crown; an outsider may know the leader's name. You remember the answer for some time. |
| *"I know what you are planning. Count me in."* | You are talking to the plot's leader and know they lead it. | You join if they would take you like any other lord: your regard for them and for the ruler and your traits count, and you need only be as close as a lord they would court. Otherwise: *"I do not trust you enough for that. Not yet."* Not possible while you are sworn to the crown or to another plot. |
| *"I will have no more part in this plot of yours."* | You are a member of an AI lord's plot and talk to its leader. | You leave the plot. *"Then go, and keep your mouth shut."* |

**How persuasion works.** It uses the game's usual persuasion screen. Some lords agree at once (*"You need not persuade me..."*), but never a lord asked to leave a plot he is in. Some refuse to discuss it at all, for example lords already sworn to the other side. When you ask a lord to stay loyal without knowing where they stand, they only open up if they would tell you the truth when asked; otherwise they answer *"Plots, loyalty... I will not speak of such things with you."* A lord who is far from joining your plot (as far as a lord the AI would not court) will not hear of it. The rest want convincing, and how many arguments you need to win depends on how far they are from changing their mind and on your relation with them. A good relation makes it easier, a bad one harder, and being at the same feast or out at the same hunt makes it easier. A lord of your own blood (a parent, child, brother or sister, or one born into the other's house) is a little easier to persuade, except when you ask them to press their house's claim.

The four arguments for joining:

- *"Fortune favours the bold..."* (Leadership; suits a lord with Valor)
- *"Count the houses already with us..."* (Tactics; suits a Calculating lord, easier once the plot is strong)
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

- A lord you win over to a plot is sworn to it for a while. A lord who agrees to press his claim stays with your plot for as long as it lasts.
- A lord you keep loyal is sworn to the crown for a while, and for longer if you are the ruler.
- If you fail, you must wait before trying that lord again. A bad failure means a longer wait and costs you some of his regard.

### The Realm tab {#the-realm-tab}

Open the kingdom screen (**K**) and pick the **Realm** tab, from anywhere. Its sections are listed on the left; the plots are under **Causes**, each with its own entry, beside the houses' mood (*"The houses' mood"*) and **"Break away from the realm"**. Choose an entry and the middle shows it as the game's Diplomacy tab would: the two sides face to face with the game's comparison bars (strength, fiefs, houses) and the list of their houses. If you know of nothing, it says *"No whispers reach you."* Once you know of a plot, its entry lists every house of the realm by strength with what you know of its stance: *leads the plot* (only once you have found out who leads it), *the house the plot would crown* (likewise), *in the plot*, *in the plot, sworn*, *loyal*, *loyal, sworn*, *wavering* (could still go either way), *the ruler*, or *unknown*. *The crown's own* only appears with claims to the throne turned off, for the ruler's close kin, who then never plot.

If you are in the plot, the top line and a bar show how much of the realm it holds and how close it is to rising. If you are not, you only learn who leads it, and only once you have found out. Once you know who leads it, the text also says whom it would crown and by what right, for example *"... gathers the lords who would crown {pretender} of the {Clan}, brother to {ruler}."* Your journal entry for the plot says the same. Under the entry, **"How it stands"** tells you what a lord in your place would weigh before acting, in words, without the odds.

On the left, **Your standing** shows your house's bonds in the realm: its claim to the throne (and, without one, how a house comes by one), the oath, the plot or cause it is in, its mark of treason and its grievances. Under **Claims**, **Your house's rights** shows your [rights to fiefs](fief-rights.md). Under **Fealty**, choose any house to see what you can do with it: an envoy to win it to your plot, or, as ruler, to keep it loyal.

### Leading your own plot

- You cannot start a plot while you are in another. To lead a plot that crowns you, your house needs a claim to the throne and the strength to wear the crown; without them, find a lord whose house has a claim and urge him to press it. Like the AI, you can plot in **any** kingdom, large or not, as long as your house does not rule it; unlike the AI, you need no bad blood with the ruler.
- Lords also join and leave your plot by themselves each week, by the same weighing as above. An AI ruler tries to win your members back.
- Your plot fades like any other if it never grows, or goes too long without the strength to rise; the journal tells you how long you have. It does not die when the realm shrinks. Other plots may grow beside yours, and lords weigh yours against theirs; whichever rises first ends the rest.

### Raise the banner {#raise-the-banner}

When you lead the plot, its entry under **Causes** in the **Realm** tab has a **"Raise the banner"** button. It works only:

- while you are **inside a town or castle** of your kingdom held by a house of your plot (yours included);
- with the plot holding a good part of the realm's strength, less than an AI plot waits for; you need no other house beside yours, no waiting and no luck. A war abroad does not stop you, and your own choice is never held back by a weak realm;
- with the crown still holding a town or castle of its own;
- when no story quest is under way, you are not in the middle of a fight and you do not ride in an army (*"Not while you ride in an army: leave it first."*);
- while no men of the plot's houses are in the thick of a battle (*"Men of the plot's houses are in the thick of a battle: the banner waits until the fighting is over."*).

If something is missing, the button is greyed out and its tooltip says what. A confirmation explains that there is no going back, that it is war until one side is left with nothing or both accept a peace, which blood will run too hot for in the first weeks unless one side is crushed, that its terms are set out across the table and the further ahead your side stands the more it can ask, and what losing costs: if the crown crushes the rising, or makes a peace that grants no pardon, every house that rode comes back branded traitor, and the crown will want your head. Then you **name your kingdom** (it cannot take the name of the realm you rise against). Your plot's houses follow you with their lands, and the civil war begins.

### When an AI plot you are in rises {#when-an-ai-plot-you-are-in-rises}

You get a window, **"The banner is raised"**, once you are free to answer: while you are a prisoner or ride in an army, it waits.

- **"Ride with them":** your clan goes over to the rebel kingdom with its fiefs.
- **"Stay loyal to the crown":** you leave the plot and are sworn to the crown for a while. If the rising goes ahead without you, its leader thinks much less of you.

During a story quest you can only stay, with no penalty.

### Breaking away yourself {#breaking-away-yourself}

As a vassal of a realm you do not rule, **Causes** in the **Realm** tab has an entry **"Break away from the realm"**: what such a plot asks, and whether your house could begin one now or why not (*"You are not on bad enough terms with {ruler}: no house would believe you mean it."*, *"None of your towns and castles touch the lands around {seat}..."*). Its **"Seek independence"** button starts it, after a confirmation, with you at its head and the lands around your seat; greyed, it says what is missing. The rules are the AI's: the same bad blood with the ruler, a town or castle, no other plot, faction or feud, no word given, and one such plot per realm. Houses join and leave it by themselves, and you cannot talk anyone into it. You raise its banner as your own plot's (see [Raise the banner](#raise-the-banner)), but only with another house beside yours. Like its members, you leave it if you make your peace with the ruler.

To join an AI plot to break away, tell its leader, once you know who it is, *"I know what you are planning. Count me in."*: it is offered only when your house could be in it, and its leader takes you at once. Its entry under Causes says whether your house could stand with them, or why not, and, if you are in it, what it still lacks to rise.

### When your lord rises against the crown {#when-your-lord-rises-against-the-crown}

If your house is sworn to a [lord](titles.md) who rises against the crown (a plot for the throne, a plot to break away, a [charter](factions.md#the-charter) taken up in arms, or his house breaking with the realm), and your house was not in it and was not asked to ride already, a rider brings you the window **"Your lord raises his banner against the crown"** (or *her*), as soon as you are free on the map, at any time while the war lasts. Your lord is never the ruling house here.

- **"Ride with him"** (or *her*): your house goes over to the rebels with its towns and castles, as a house of the plot would. If the crown wins, you come back marked as a traitor and are [judged](realm-houses.md#houses-marked-as-traitors) with the others.
- **"Stand with the crown"**: you keep your oath and stay, at war with your own lord while the rising lasts. Your lord does not hold it against you: *"many a vassal stands apart in a quarrel with the crown."*

AI vassals weigh their lord when they decide whether to join a plot (see [Who joins, and why](#who-joins-and-why)), and the houses sworn to a house that breaks with the realm weigh riding with it (see [A house that breaks with the realm](#a-house-that-breaks-with-the-realm)).

### When a house of your blood or your allies breaks with the realm

If a house that is your kin or your ally, or the leader of a plot you are sworn to, [breaks with the realm](#a-house-that-breaks-with-the-realm), a window asks you once you are free (not in an army, a battle, a siege, a talk or a prison): **"Ride with him"** (or *her*) or **"Stand with the crown"**. It tells you what binds you, what its head asks of you by his character, how the realm reads the break, and that if they win, the houses that rose choose the king. You may answer at any time while the war lasts. Staying costs you nothing.

### When your realm falls into civil war {#when-your-realm-falls-into-civil-war}

When your realm falls into civil war and your house stays with the crown, as a vassal, a window **"Civil war in {Kingdom}"** tells you once, when you are free on the map, what the rebels want, which houses rose, that your house stands with the crown and the rebels are your enemies now, how the war is decided and what each side's victory would bring. Not if you rule the realm or serve it for pay. From then on, ask any lord *"What is happening in the realm?"* to hear how it goes (see [Asking how things stand](factions.md#asking-how-things-stand)).

### If you are the ruler

- Every wrong your crown does a house costs a little of its head's goodwill toward you (more in a kingdom grown well beyond its fair share), but never your own clan or close kin; with the old discontent on, the size of the realm wears on it too. Your own clan never plots against you, but a brother, son or daughter heading a house of their own has a claim to your throne and may.
- Nobody wins lords back for you: talk to them yourself (*"There is a plot against {your name}. Stay loyal to the crown."*), or send an envoy. A lord you keep loyal stays so for a good while. Talking the plot's leader out of it ends the plot.
- When the rumour reaches you, ask around, and watch **Causes** in the **Realm** tab, to find who is behind it.
- **You can lose the crown.** If the rebels win, the house they meant to crown rules your kingdom and your house stays on as a vassal.

### Envoys

With [Envoys](envoys.md) you can send a family member or companion to do this talking for you, from the lord's page in the encyclopedia: **"Win {lord} over to your plot"** (when you are in one) or **"Keep {lord} loyal to the crown"** (when you know of one). Under **Fealty** in the Realm tab, the house you choose offers the same errands, the second only to the ruler. The envoy argues it with their own skills and character, as you would. An envoy sent to sound a lord out also reports where their house stands on the plot.

## Tips {#tips}

- Conquest has a price at home: past its fair share, every wrong the crown does a house stings more, and its lords plot and band together more readily. In the greatest realms, a lord merely cool toward the ruler may start a plot.
- A plot's leader needs bad blood with the ruler, and its pretender no love for him. Gaining relation with your discontented lords keeps them from starting one, and keeping on good terms with the strong houses that have a claim leaves a plot nobody to crown.
- Want the crown without a claim of your own? Marry the head of your house to the ruler's brother, sister, son or daughter, or find a claimant house and press its claim for it.
- Watch the **Calculating** lords: they hold back while a plot is small and rush in once it grows.
- A war abroad is no shield: a strong plot may rise in the middle of it. Only a realm that is losing its wars, or small, makes the plotters hold back (see [The rising](#the-rising)).
- In a civil war, mind the **Objective** line: the side that holds what the war is about gains ground every day, and the further ahead a side stands, the more it can ask at the table. As a rebel, mind the pardon: a peace without one, where the crown keeps its throne, leaves every house that rose to its judgment.
- Feasts and hunts make winning lords over easier, for you and for the AI.
- Keep a town or castle of your plot in mind before you start: you can only raise the banner from inside one of them.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `RealmDiscontentEnabled` (off by default): `true` brings back the discontent of large kingdoms; off, what it already took comes back slowly.
- `ConspiracyEnabled` to `false`: no new plots, and plots under way are called off. A civil war already going on continues until it ends.
- `RealmSizeAmbitionEnabled` to `false`: the size of a kingdom no longer makes its lords more rancorous or ambitious.
- `PlotsOnlyInLargeRealms` to `true` (off by default): the old way, where the AI plots only in a kingdom that is too large or under a ruler with a weak claim, and an AI plot ends once its kingdom has been back below "too large" for a while.
- `ThroneClaimsEnabled` to `false`: plots work as before the claims to the throne: the house that starts a plot is always its pretender, and the ruler's close kin never plot.
- `InternalWarScoreEnabled` to `false`: civil wars and feuds keep the base game's war score, with no Objective line and the peace open from early on with the other side's consent.
- `WarPrisonersLineEnabled` to `false`: no Prisoners line in the war score.
- `NoWhitePeaceBeforeWearyEnabled` to `false`: a white peace may be made as soon as peace can be talked of.
- `CivilWarOutsideRestraintEnabled` to `false`: other kingdoms treat a war against either side of a civil war like any other war.
- `CivilWarNoAllianceEnabled` to `false`: the rebels of a civil war may make alliances as in the base game; `CivilWarCallReluctanceEnabled` to `false`: a crown in a civil war answers its allies' calls, and pays for refusing one, as in the base game.
- `RuptureJoinEnabled` to `false`: a house that breaks with the realm rises alone; `RuptureRejoinEnabled`: houses that stayed home do not weigh it again during the war; `RuptureElectionEnabled`: the rebels of a house that broke away crown the house with the best right, with no vote.
- `EnvoyPlotJoinEnabled` / `EnvoyPlotLoyalEnabled` to `false`: removes the two envoy errands for plots.
- `HuntPlotRecruitEnabled` to `false`: hunts no longer make talking lords into or out of a plot easier.
- `IndependencePlotEnabled` to `false`: no plots to break away. Its numbers are on the [Settings](../settings.md#kingdoms-and-court) page.
- `CivilWarBriefingEnabled` to `false`: no window when your realm falls into civil war.
- `InternalWarWeaknessEnabled` to `false`: a realm weak in its wars abroad no longer holds its plots back (nor its other quarrels, see [Factions and grievances](factions.md)).
