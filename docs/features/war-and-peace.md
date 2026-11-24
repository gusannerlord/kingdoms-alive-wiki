# War and peace

AI kingdoms now go to war for a reason, stay in it until it is settled, and rest for a while once it is over. You can also see why: lords say what they are fighting for, and when a kingdom declares war on yours, you are told its reason. Every peace between realms, yours and the AI's, is made at one table, the **Terms of Peace** screen, and voted by the councils of both realms.

## Why a kingdom goes to war { #why-a-kingdom-goes-to-war }

The AI still weighs what it could win against what it could lose. On top of that, these causes push it toward a war:

- **A hated ruler.** A bad relation between the two ruling clans counts far more than in the base game, though it rarely makes a war on its own: it adds to a cause. It works both ways, and friendship weighs more than hatred: a ruler on good terms with another is much less likely to attack them.
- **Lost land.** A town or castle of the attacker's culture held by a kingdom of another culture counts many times as much as in the base game: in full when the attacker is at least as strong, less the weaker it is. Between two kingdoms of the same culture it counts as in the base game.
- **The right moment.** A kingdom at peace with every other kingdom sees its chance when a stronger neighbour of another culture holds some of its land and has just gone to war with someone else. The lost land then counts for much more again. It still needs a good part of the neighbour's strength, and it will not do this to a ruler it is close friends with.
- **A rival grown too large.** See [A kingdom that grows too much](#a-kingdom-that-grows-too-much) below.
- **An ally already at war** with the target.
- **A grievance.** Incidents between neighbouring kingdoms build up tension between them. See [Events between kingdoms](events-between-kingdoms.md).
- **Its holy city.** When the holy town of the ruler's faith (see [The faiths of Calradia](faiths.md)) is held by a kingdom whose ruler keeps another faith, the kingdom wants it back more than a town of its faith or of its duchies.
- **Lands of its faith.** Towns and castles whose people keep the ruler's faith, held by a kingdom whose ruler keeps another, are land the kingdom covets: their people look to it.
- **Its duchies and counties.** In a kingdom of [dukes and counts](titles.md), a town of one of its duchies, or a castle of one of its counties, that it held and lost to another kingdom counts as land to take back: a town of a duchy more than a castle of a county. The claim lasts as long as the house that lost it keeps its [right](fief-rights.md) and stays in the kingdom: it fades when the right passes on weak and is forgotten, or when that house leaves the kingdom, even only to ride out in a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses).
- **Rulers of different faiths** are a little readier for war with each other; rulers of the same faith a little slower to it.
- **One Empire.** Between two realms of the Empire, each emperor claims the whole of it, and that claim is a cause of its own (see [The Empire's own ways](empire.md)): *"there is one Empire, and Lucon is not its emperor"*.

For all of these, the two churches count as one faith, and so do the two northern faiths. A town or castle counts only for its strongest reason, and its lords name it for that: a holy city that is also lost land of the attacker's culture counts, and is named, as the holy city, not as both. The holy city, the lands of the faith, the towns of the duchies and the castles of the counties count in full only when the attacker is at least as strong, as lost land does; the rulers' faiths count whatever the odds. Among them the holy city weighs most, then a town of a duchy, then a castle of a county or a town of the faith, and the rulers' faiths least. Lost land of the attacker's culture still counts as above, and at "the right moment" it can weigh even more than the holy city.

A war with none of these behind it needs clearly better odds. Causes that are strong enough remove that handicap completely; weaker ones remove part of it.

## Dukes and counts in the vote { #dukes-and-counts-in-the-vote }

When a kingdom of dukes and counts votes on a war, a duke or count whose lands border the enemy, or who has lost one of them to it, is more eager for it; a duke more than a count. One whose lands lie far from the enemy is a little less keen. The same goes for you: your own vote is yours, but the AI lords of your kingdom weigh their lands when you propose a war.

## Less piling on { #less-piling-on }

- **Strength is measured fairly.** Much of each kingdom's strength is counted from its size (its towns, castles and clans), not only from the men it has right now. A kingdom that has just lost an army is no longer everyone's prey.
- **Allies deter.** Part of the strength of the target's allies counts on the target's side.
- **Spoils are shared.** A target that others are already fighting promises less, and less again with each kingdom already at war with it: with three foes already on it, little is left to win. A cause of its own (lost land, its faith, its titles, a bad relation) still counts in full.
- **A kingdom is a little less afraid of a stronger one.**
- **Rich kingdoms are easier to attack.** In the base game, how much a lord must stand to win before he puts a war to his council rises with the wealth of the kingdom he would fight, so the richest kingdoms were seldom attacked and the poorest were the easy prey. That bar is now drawn toward that of a kingdom of middling wealth: it still rises with wealth, but far less steeply.
- **"We are stronger" is not reason enough.** When a kingdom at peace weighs a new war, what it simply stands to win ("Right now we are stronger than them", "their lands are rich") counts for less than in the base game; a real cause weighs as before, and so does the fear of losing. Wars already under way, and the making of peace, are weighed as before: kingdoms only start fewer wars of plain greed, and rest longer between them.
- **No third front lightly.** A kingdom already at war with two realms (the hosts of its own feuds not counted) is very slow to declare a third war. What it simply stands to win, "we are the stronger side" above all, barely counts then, and the war must clear a much higher bar, higher still for a fourth. Only a strong cause carries it: land it lost, its holy city, its titles, a ruler it hates. This weighs only on a war it would declare itself, never on answering an ally's call, and your own realm's lords weigh it the same way. The kingdom screen says so when it holds your council back: *"we are already at war on two fronts, and will not open a third"*. Switch: `WarFrontsRestraintEnabled`.

## A kingdom that grows too much

Every kingdom has an even share of the towns and castles on the map. Kingdoms that have been destroyed still count, so the share does not grow as kingdoms fall.

- **Resentment.** A kingdom that holds clearly more than its share is resented: other kingdoms weigh a war against it as if they liked its ruler less, the more so the larger it grows. The real relation is not changed, and this goes away when the kingdom shrinks.
- **Fear.** A little larger still, it is feared: its neighbours expect more from a war against it, the war gets an extra push of its own, and its land counts at full value (the base game counts the land of a very large kingdom at less than its worth).
- **Coalition.** Weaker kingdoms do not open a war against it alone, but once someone is fighting it, others count part of that strength as their own and join in. Joining others against it costs little or nothing in shared spoils, the less the more dominant it is.
- **The right moment lasts longer** against it, and an attacker needs less of its strength alone, because the kingdoms already fighting it count too.
- **Fear weighs strength too.** A kingdom stronger than a dominant one fears it, and resents its growth, only as much as their strengths say: a large realm with a weak army is little threat to a mightier one, and its many fiefs give the stronger side little reason to attack it. A kingdom weaker than the dominant one fears it as before. Switch: `DominanceFearWeighsStrength`.
- **Good relations calm the fear.** The better the two ruling clans get on, the less the fear, though it never goes away entirely.

Your own kingdom counts like any other.

!!! tip
    If you rule a growing kingdom, make friends with the neighbouring rulers. It is the best protection you have against everyone turning on you.

## Wars that stop and start sensibly { #wars-that-stop-and-start-sensibly }

- **Weariness.** The men a kingdom has lost in the field in its current wars, and each peace it has signed lately (that fades with time), make it expect less from a new war. Only the men of lords' hosts count: villagers, caravans, militia and garrisons killed in a fight do not make a realm weary. The losses are weighed against all the men the realm can still put in the field (its hosts, its garrisons and the volunteers waiting in its towns and villages), so a realm that lost an army but keeps its lands is far from spent. The same losses make it want peace in the war it is fighting, whether it is winning or losing, but not at once: they weigh nothing towards a peace while the war is young, more each day once peace can be talked of, and fully once the war has dragged on.
- **Restlessness.** A kingdom with no war against another kingdom for a long while starts to expect more from a war, more with every further day of peace. This is a last resort against endless peace; most wars should come from real causes.
- **The ruler looks for a war.** In the base game, a lord who wants to put a war to his council picks a kingdom at random, often one on the far side of the map, so a kingdom could sit at peace for months beside a neighbour its ruler longed to fight. Now, once an AI kingdom has had a long, complete peace (no war with another kingdom, and no war within: no civil war, no feud fought in arms), its ruler weighs every day each kingdom it could fight: one with a common border, no truce, nothing in the rules that forbids it. He takes the one he would most gladly fight and, if that war is worth what any war needs and his council leans towards it, puts it to the council himself, paying the same influence as anyone. A ruler whose council would vote him down keeps his influence and waits. The council votes as always, and the reason given is the real one. If no war is worth it, nothing happens: peace goes on. A kingdom you rule is never pushed: you decide. If you serve an AI ruler, his proposal comes before the council, and to you, like any other. The other lords' own proposals go on as in the base game.
- **Feuds hold wars back.** A kingdom whose houses are fighting a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses), or have one waiting to resume, is slower to start a new war abroad: the larger the share of its strength caught up in feuds, the more it holds back, and more still while a feud is being fought in arms. This binds your council's vote as much as the AI's. While such a feud lasts, the restlessness of a long peace does not count and the ruler looks for no war; the days of peace still count, so once the last feud is over both come back as strong as those days make them.
- **A feud's hosts are the realm's border.** The towns and castles held by the hosts of a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) between a kingdom's houses count as that kingdom's border when it would otherwise have none with its foe: for its wars, so the game does not force a peace for lack of a border, and for who counts as its neighbour.
- **Civil war.** While a kingdom is in a [civil war](civil-war.md), other AI kingdoms find it harder (not impossible) to attack either side, and its war is never "the right moment" for them.

## The war score { #the-war-score }

How a war stands is the game's war score, on the Diplomacy tab, and it decides how much each side of the AI gives and asks at the peace table. Its lines:

- **Kills** count only the men lost in battle by lords' hosts, the same losses that make a realm weary: a slaughter of villagers or caravans gains no one ground.
- **Town Sieges**, **Castle Sieges** and **Raids**, as in the base game.
- **Prisoners**: the lords of the enemy your side holds captive, in its parties or in its towns and castles, the enemy's ruler most of all. A lord who escapes or is freed takes his part with him.

A war within a realm (a [civil war](civil-war.md#winning-the-civil-war) or a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) fought in arms) also has an **Objective** line: what that war is fought for. A war between realms has none: it is won in the field and at the walls.

What counts is how far apart the two sides are: a close war, one side somewhat ahead, clearly ahead, or the other side crushed.

## Peace needs both sides { #peace-needs-both-sides }

In the base game the kingdom that wants out just leaves, usually paying tribute. Now a peace between realms follows the course of the war, the same course as a war within a realm, and nobody is ever made to take one: your kingdom too answers every peace offered to it.

- **The first weeks.** No talk of peace at all, unless one side is crushed: *"The war with the Vlandians has barely begun, and blood runs too hot for talk of peace."*
- **Peace can be talked of.** Either side may offer it, and the other must want it, not merely lose nothing by it. So soon in the war, no peace is made for nothing: the side behind must pay the side ahead a tribute for it. *"So soon, and for nothing? My lords have bled for this war."*
- **The war drags on.** The lords on both sides grow weary of it, and a peace is more welcome than it was, above all to the side that is behind. A white peace, with nothing given either way, is possible again: it is for a long war that has stalled.
- **Both sides are sick of it.** Their lords want it ended more than they want to win it.

At any time, a side wants peace more the further behind it falls, and badly once it is crushed, while the side that crushes it makes peace only if it suits it. The side ahead does not ask for a peace out of weariness: it only takes one offered to it, so it is the side behind that asks, and that pays.

A house that [breaks with its realm](realm-houses.md#a-house-that-breaks-with-its-realm) raises a [civil war](civil-war.md) in it, and that war makes its peace at the same table, with terms of its own (see [Wars inside a realm](#wars-inside-a-realm)). A house that holds no realm, yours or the AI's, makes its peace at the same table as a realm (see [Terms of peace](#terms-of-peace)).

## Truce and tribute { #truce-and-tribute }

- **Truce.** For a good while after a peace, neither kingdom's council can declare war on the other (in the base game the truce is shorter, and binds only the AI).
- **Tribute.** A tribute does not forbid a war, but it weighs against one: a kingdom that is paid tribute by another thinks twice before attacking it, because the war would end the silver still owed, and breaking a peace whose price is still being paid looks bad. The weight fades as the tribute runs out. A strong cause, such as a hated ruler or lost land, can still outweigh it.

On the kingdom screen, a war you cannot propose shows the reason, for example *"A truce holds with Vlandia: the peace is barely sealed, and to break it now would shame the realm."*. When the tribute weighs, your lords say so among their reasons against a war: *"they still pay us tribute, and one does not take a man's silver and his throat in the same season"*.

The truce and the peace rules also bind your kingdom, whether you rule it or serve it, when it declares war or makes peace. Attacking someone on the map still starts a war as always.

## Allies called to war { #allies-called-to-war }

- **The caller stays.** A kingdom that called an ally into a war cannot make peace in that war while the ally is still bound to it, and its enemy cannot make peace with it either, unless one side is crushed; even then the peace must still pass the rules above. On the kingdom screen: *"The Battanians came to this war at this realm's call. It cannot be left while they are still bound to it."*
- **No ally is called into a lost war.** A kingdom clearly losing a war calls no ally into it: not when the war or an alliance begins, not by its council, not by you. A call already answered stands, and an overlord still comes to defend its [vassal realm](vassal-realms.md). This binds your kingdom too, if the rules bind it: an allied lord does not take up such a call in talk, your envoy is not offered that war, and a message tells you why when your council or a notice would have made the call.
- **A crown fighting a civil war answers few calls.** A crown of the AI joins an ally's war only if it would choose that war for its realm on its own, whatever it is paid; and any crown fighting a civil war, yours too, may refuse a call at no cost in goodwill (see [Alliances in a civil war](civil-war.md#alliances-in-a-civil-war)).
- **The ally leaves with the caller.** When the caller makes peace, the allies it called are at peace with that enemy soon after, with no tribute either way. In the base game they were left fighting alone.

This also applies to your kingdom: if you are called into a war, you leave it when the caller makes peace.

## Terms of peace { #terms-of-peace }

The **Terms of Peace** screen is the only road to a peace, for you and for the AI: between realms, in a civil war and between the hosts of a feud. The game's own way of proposing a peace is gone from the Diplomacy tab; a white peace is put on this table like any other terms.

- **Where.** In the kingdom screen's Diplomacy tab, choose a war and press **Negotiate terms**. Opening the table costs nothing; putting terms costs influence: the game's cost of proposing a peace for a white peace or a tribute, more for towns, castles or fealty. When terms cannot be put now, or you lack even the least of that influence, the button stays greyed and says why. Or tell the enemy ruler *"Our realms should make peace."* in person: he first says how he stands, in words, and if you go on (*"Then hear my terms."*) the same screen opens, at no cost; when you close it, he has a last word on how it ended. Any other enemy lord only tells you how his ruler feels. Or send an [envoy](envoys.md) from the enemy ruler's page in the encyclopedia: once they stand before the ruler, *"Carry your terms of peace to {ruler}"* opens the same screen, at no cost, and **Send these terms** (only for terms the ruler would accept now) has the envoy put them once you choose "Hear me on this, then." in the conversation that comes back under a flag of truce; the ruler answers there, as the war then stands.
- **Who sets terms.** A ruler sets any terms. As a lord of a realm you do not rule, **Negotiate terms** lets you put only a white peace or the tribute the war asks before your council: the enemy ruler answers first, then both councils vote. A mercenary makes no peace: the peace is for those who hire him. A vassal realm makes none either: its overlord's peace covers it (see [Vassal realms](#vassal-realms)).
- **The screen.** At the top, the two realms, the day of the war, the enemy ruler's words, and the towns and castles taken from them and lost to them in this war. In the middle, what each side gives: **A white peace** (nothing either way), on its own; or terms of your own: a light, heavy or crushing **tribute** (with the denars a day; the step that matches what the war asks says so), every **town and castle** of either realm, and **fealty**. What the rules forbid right now is greyed, and its tooltip says why (too soon for a peace for nothing, under siege, the realm not beaten badly enough, too little land left...). What the enemy ruler would not give can be ticked, but it is marked in red, and he says so. At the bottom, both councils (see below), and the ruler's answer: he would accept, wants a little more, is far from it, or will not have it. **Offer** is greyed until he would accept.
- **What can be put on the table:** the peace itself; a tribute either way (between realms a peace is paid in tribute, never in a sum paid once); **towns and castles** of either realm (one or two in a peace, never a realm's last ones, none under siege); **fealty**, one realm becoming the other's vassal (never annexation), under the rules of [vassal realms](#vassal-realms); between two realms of the Empire, an emperor clearly beaten by the other may **yield the purple** to them, and his realm is joined to theirs (see [The Empire's own ways](empire.md)). A realm weighs a town or castle it would give up more dearly when it lies deep in its land, is of its own culture, is a town or the seat of its ruler or of a duchy, or would cut its land in two. Land is never bought or sold: a realm that yields a town or castle is paid no tribute in the same terms.

### What the AI gives and asks { #what-the-ai-gives-and-asks }

An AI ruler gives, and asks, only what the war score has earned:

- **A close war:** a white peace, once the war has dragged on; before that, the side behind pays a light tribute.
- **One side ahead:** a tribute from the side behind, heavier the further ahead the other is.
- **One side crushed:** any tribute, and only then **towns and castles**, **fealty** or the purple.

Land asks more still. An AI kingdom gives up a castle only once this enemy has taken a good share of what it held when the war began, a town only after it has lost much more, and never more than one town in a peace; fealty only when it is beaten that badly and would accept it under the rules of [vassal realms](#vassal-realms). Tribute always comes first. A kingdom **held between two fronts** (at war with two realms or more that fight no one else, none of which would take its peace for a tribute) gives up a castle or a town a little sooner, to close one front; it still takes a crushing defeat for land to be asked of it.

At your table the AI ruler will not give more than that: what lies beyond is greyed, with his reason (*"{ruler} is not beaten so badly as to..."*). What you give of your own is yours to judge: you may always offer more than the war asks of you.

### The councils vote { #the-councils-vote }

Terms both rulers accept go to the councils of **both** realms. The other realm's council votes first; then yours. Each ruler has the last word over his own council alone, and the peace is made only if both say yes.

- **Before you offer**, each council shows whether it would agree, is divided or would refuse, a bar of support, and the portraits of the heads of its houses under *For*, *Against* and *Aside*. Hover over one to see how strongly that house backs its side and, when there is one, its real reason. For an AI council, you are also told how likely its ruler is to overrule it.
- **How the houses weigh it.** The lords whose towns or castles would be given away always vote against, and cannot be talked round. The other lords weigh the land their realm would lose, more so a place next to their own or in their duchy, or one held by their kin, and a bold or honourable head more than a calculating one; land their realm would receive, more so a place they could hope to be given, one near them, of their culture, or one taken from them in this war; and how the war goes for them: a realm that is losing, fighting more than one war, left with little land, or with the enemy at a house's own walls leans towards peace, one that is winning against it. A house says so: *"The war is lost if we fight on."*, *"Our own walls are next."*, *"The war is going our way. Why stop now?"*, *"would not see Pravend given away"*.
- **Each ruler decides at the end of his own council's vote, as in any vote of the realm.** His house votes like any other; he has no extra weight. An AI ruler may push terms through against his council, or throw them out against it, paying influence and the goodwill of the house that led the other side, or let the council's vote stand. When the vote is over the screen shows its result, house by house.
- **When your council votes**, it votes on the screen at once, not over days:
    - **As ruler:** you see how your lords voted, then **Carry the terms**, **Withdraw the terms** or **Abstain** (leave it to the custom of the realm, as you may in any vote). Following your council is free; going against it costs the influence the game charges a ruler to overrule his lords, and the button is greyed if you lack it. A realm with no other house has no council: your word is enough, at no cost.
    - **As a lord of a realm ruled by another:** you are told your voice is awaited, and the screen opens as soon as you are free on the map. Vote for or against, mildly, strongly or with all your influence (each at the game's cost, half if your side loses), or **Keep out of it**; the bar and the portraits change with your vote. If you do not answer in good time, the council votes without you. Then the ruler decides. A mercenary has no vote.
    - The houses that backed a side pay their influence as in any vote of the realm.
- A town or castle given away goes to the winner's share-out (or to its ruler, if his house is the only one of that realm), and its old holder bears a grudge against the crown that gave it. Terms refused are not heard again between the two realms for a while.

### The AI too { #the-ai-too }

The AI makes peace at the same table. When a lord would put a peace to his council, as in the base game, it becomes terms: a white peace or the tribute the war asks, within what the war score allows. A kingdom losing for real, whose enemy would not take that, offers the cheapest fuller terms its enemy would take; one clearly winning, and far stronger, names its price. Its ruling house pays influence to put terms, as you do from the Diplomacy tab, and both councils vote, as above.

Terms offered to you, plain or full, arrive by courier, as a notice on the map: it opens the same screen with their terms, the forecast of both councils, and **Accept the terms** or **Send the courier back**. Closing it, or letting it pass, is a refusal. When a lord of your own realm would put a peace, his proposal comes before your council the same way, and the enemy's council votes on it first.

**A house that holds no realm** (yours or the AI's) makes its peace with a realm on the same screen, face to face: a white peace, or gold paid once, never land or tribute. Its head decides for it, and the realm votes in its council. While the war is young the house must pay for its peace; once the war has dragged on, a white peace is possible, and a realm may pay a house to end it.

### Wars inside a realm { #wars-inside-a-realm }

A [civil war](civil-war.md#peace-in-a-civil-war) and a [feud](factions.md#how-a-feud-ends) fought in arms end at the same table, between the crown and the rebels or between the two hosts, with terms of their own instead of tribute and land: a pardon, the crown after this reign or laid down, the charter, a realm of their own, the fief or the title in dispute, a right weakened or given up, a vassal freed, and a sum in silver paid once. No other town or castle changes hands, and no tribute.

- **Who sets terms.** The head of each side (the ruler, the rebels' leader, the head of a host) sets any terms, at no cost. A lord who does not lead his side may only put a pardon (or, in a feud, a white peace) or a modest sum in silver before its council, at the game's cost of proposing a peace.
- **Both sides vote**, each in its own council, and each leader has the last word over his own.
- **The AI gives only what the war score has earned, and the side ahead asks for something.** A side well ahead that holds what the war is fought over keeps it; a clear win asks at least the lighter form of the war's own stake, a crushing win the stronger form, and silver only fills out the rest.
- **Without a pardon**, the crown or the lord who keeps his place judges those who rose against him: as traitors in a civil war, for felony in a feud.

## Vassal realms { #vassal-realms }

A clearly beaten kingdom may have to swear fealty instead of paying a tribute. See [Vassal realms and annexation](vassal-realms.md). In war and peace:

- **A vassal marches with its overlord** in every one of its wars, without a vote, and makes no wars, alliances or trade agreements of its own.
- **The overlord's peace covers the vassal** in that war. The vassal cannot make that peace itself (*"Only the {overlord} can make this peace for your realm."*), and its enemy has to make peace with the overlord.
- **No war on your own vassal.** To end the tie, release it or demand its annexation from its page under **Tributaries** in the Crown tab. Whoever may not attack the overlord (truce, alliance) may not attack its vassal either, an attacker counts the overlord's full strength against it, and the vassal's against whoever attacks the overlord.
- **Dominance counts a vassal's towns and castles at half** for its overlord.
- **The caller rule above does not bind an overlord and its vassal**: the overlord makes its peace when it likes, and that peace covers the vassal.

## Heirs and old grudges

When a clan leader dies, the heir inherits part of each of the dead leader's relations. The base game always passes on the same large share. Now the share is drawn at random for each person, from a little to that much. An heir may keep the late leader's friendships and feuds almost whole, or nearly forget them.

## Seeing why { #seeing-why }

- **War proposals.** A clan that proposes a war gives its real reason, for example *"Balgard is ours by right, and the Nords hold it. It is time to take it back."*, *"Our allies are already at war with the Aserai. We should stand with them."* or *"The Khuzaits have grown too powerful. They must be checked while it can still be done."* When recent [incidents between the two kingdoms](events-between-kingdoms.md) are not the main reason but still weigh a fair part as much, they are named after it, here and in the window when war is declared on your kingdom: *"... And the cattle raid on the border is not forgotten either."*
- **The kingdom screen.** When you look at proposing a war, the support shown by the game ("Low support", "Good support"...) is followed by the lords' two main reasons, for or against. For example *"Low support: we have no quarrel with them; the realm is weary of war"* or *"Good support: Sargot is ours by right; we are the stronger side"*. Faith and titles have their own words, for example *"Pravend, the holy city of the Church of Paravenos, is in the hands of the Battanians, who do not even keep the faith. We cannot suffer it a day longer than we must."*, *"Usanc Castle is a castle of our county of Sargot, and the Battanians hold it. The county must be made whole again."* or *"Caladog of the Battanians keeps the Old Ways, not the Church of Paravenos. Between us there can be no lasting trust."*; on the kingdom screen, *"Good support: they hold Pravend, the holy city of the Church of Paravenos; we are the stronger side"*. A lord only names a cause of faith or titles when it is the one that weighs most.
- **Peace on the kingdom screen.** The tooltip of **Negotiate terms** says how your lords lean towards a peace, and their main reasons, for it and against it.
- **When war is declared on your kingdom** by a vote of their council or because an ally called them in, a window titled **"War is declared on us"** pauses the game and gives what the attacker's lords say, for example *"What their lords give as the reason: "Our allies, the Sturgians, are at war with you and have called on us. We keep our word.""* If they have no cause, it says *"They give no reason beyond their own advantage."* You can switch the pause off and get a notice on the map instead.

## Turn it off

In the [settings file](../settings.md), set any of these to `false`:

- `WarScoringEnabled`: all the new reasons for war (everything below that changes how kingdoms weigh a war needs it).
- `WarStrengthEnabled`: strength measured by size, allies deterring, less fear of the stronger.
- `WarSharedSpoilsEnabled`: a target already at war promises less.
- `WarRulerRelationEnabled`: the rulers' relation weighing far more (`WarRelationIgnoresStrength` and `WarGoodRelationCounts` fine-tune it).
- `WarReconquestEnabled`: lost land weighing far more (also turns off the right moment).
- `WarOpportunityEnabled`: the right moment to take land back (`WarOpportunityStrengthCountsTargetEnemies` lets kingdoms already fighting a dominant target count toward it).
- `WarNoCausePenaltyEnabled`: wars without a cause needing better odds.
- `DominanceEnabled`: everything about a kingdom grown too large (`DominanceLiftsSharedSpoils`, `DominanceRemovesSizeDiscount` and `DominanceCountsDestroyedKingdoms` fine-tune it; switch the last one off in a campaign that starts with kingdoms removed).
- `ExpansionResentmentEnabled`: resentment of a growing kingdom.
- `DominanceFearWeighsStrength`: a stronger kingdom fearing a dominant one only as much as their strengths say.
- `WarFrontsRestraintEnabled`: the resistance to a third front.
- `WarHolyCityEnabled`: kingdoms want back the holy city of their faith.
- `WarFaithLandEnabled`: lands of the ruler's faith under a ruler of another faith are coveted.
- `WarRulersFaithEnabled`: rulers' faiths push toward war or peace.
- `WarTitlesEnabled`: towns of duchies and castles of counties lost to another kingdom count as land to take back.
- `WarTitleVotesEnabled`: dukes and counts of the border vote for a war more, those far away a little less.
- `WarWearinessEnabled`: war weariness and the wish for peace after losses; `PeaceWearinessRampEnabled`: losses weighing towards a peace only as the war goes on.
- `WarAmbitionEnabled`: restlessness after a long peace.
- `WarAfterLongPeaceEnabled`: the ruler looking for a war after a long peace.
- `WarPrisonersLineEnabled`: the Prisoners line of the war score.
- `PeaceNeedsOtherSideConsent`: peace between kingdoms following the course of the war, with the other side's consent.
- `NoWhitePeaceBeforeWearyEnabled`: no peace for nothing in a young war.
- `TruceEnabled`: the longer truce.
- `WarTributeWeightEnabled`: a tribute weighing against a war on the realm that pays it.
- `WarDuringFeudPenaltyEnabled`: feuds holding a kingdom back from new wars; `WarWaitsForFeudsEnabled`: restlessness and the ruler's search for a war waiting while a feud lasts.
- `DiplomacyRulesApplyToPlayerKingdom`: the truce and peace rules also binding your kingdom.
- `CallerStaysWhileAlliesAreBound`: a caller cannot leave while its ally is bound.
- `CallerPeaceCoversCalledAllies`: called allies make peace with the caller.
- `NoCallWhileLosingEnabled`: no ally called into a war the caller is clearly losing.
- `WarBarSmoothingEnabled`: the bar for a war against a rich kingdom rising less with its wealth.
- `HeirRelationEnabled`: heirs inheriting a random share of relations.
- `NegotiatedPeaceEnabled`: the Terms of Peace screen; `NegotiatedPeaceAiEnabled`: AI kingdoms offering and demanding fuller terms; `NegotiatedAiCedePinnedEnabled`: a kingdom held between two fronts giving land a little sooner.
- `WarSupportExplained`: the reasons for a war or a peace on the kingdom screen.
- `WarDeclaredOnPlayerShowsReason`: the window when war is declared on your kingdom; `WarDeclaredOnPlayerPausesGame` set to `false` shows it as a map notice instead.
