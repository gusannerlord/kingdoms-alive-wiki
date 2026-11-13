# War and peace

AI kingdoms now go to war for a reason, stay in it until it is settled, and rest for a while once it is over. You can also see why: lords say what they are fighting for, and when a kingdom declares war on yours, you are told its reason.

## Why a kingdom goes to war { #why-a-kingdom-goes-to-war }

The AI still weighs what it could win against what it could lose. On top of that, these causes push it toward a war:

- **A hated ruler.** A bad relation between the two ruling clans counts six times as much as in the base game, capped at about a third of what a war needs: it adds to a cause, but rarely makes a war on its own. It works both ways, and friendship weighs more than hatred: a good relation counts ten times as much, up to about half of what a war needs, so a ruler on good terms with another is much less likely to attack them.
- **Lost land.** A town or castle of the attacker's culture held by a kingdom of another culture counts up to ten times as much as in the base game (in full when the attacker is at least as strong; less the weaker it is). Between two kingdoms of the same culture it counts as in the base game.
- **The right moment.** A kingdom at peace with every other kingdom sees its chance when a stronger neighbour of another culture holds some of its land and has just gone to war with someone else (every war that neighbour has began no more than 20 days ago). The lost land then counts three times as much again. It still needs at least 60% of the neighbour's strength, and it will not do this to a ruler it is close friends with (relation 80 or more).
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

- **Strength is measured fairly.** Almost half of each kingdom's strength is counted from its size (its towns, castles and clans), not only from the men it has right now. A kingdom that has just lost an army is no longer everyone's prey.
- **Allies deter.** Half the strength of the target's allies counts on the target's side.
- **Spoils are shared.** A target that others are already fighting promises less: the first kingdom already at war with it lowers the expected gain by almost a third, and each one after that by half again: with three foes already on it, little is left to win. A cause of its own (lost land, its faith, its titles, a bad relation) still counts in full.
- **A kingdom is a little less afraid of a stronger one** (up to 10% less, when the other side is twice as strong).
- **Rich kingdoms are easier to attack.** In the base game, how much a lord must stand to win before he puts a war to his council rises with the wealth of the kingdom he would fight, so the richest kingdoms were seldom attacked and the poorest were the easy prey. That bar is now drawn toward that of a kingdom of middling wealth: against a kingdom twice as rich as the middle it is about 1.4 times the middle's instead of twice, and against one half as rich about 0.7 times instead of half.
- **"We are stronger" is not reason enough.** When a kingdom at peace weighs a new war, what it simply stands to win ("Right now we are stronger than them", "their lands are rich") counts for less than in the base game; a real cause weighs as before, and so does the fear of losing. Wars already under way, and the making of peace, are weighed as before: kingdoms only start fewer wars of plain greed, and rest longer between them. The number is `WarSpoilsWeight` (0.7) in the [settings file](../settings.md).

## A kingdom that grows too much

Every kingdom has an even share of the towns and castles on the map. Kingdoms that have been destroyed still count, so the share does not grow as kingdoms fall. With nine kingdoms and 133 towns and castles, the share is about 15.

- **Resentment** starts at 1.25 times the share (about 19). Other kingdoms weigh a war against it as if they liked its ruler less, up to 30 points of relation less at twice the share (about 30). The real relation is not changed, and this goes away when the kingdom shrinks.
- **Fear** starts at 1.3 times the share (about 20) and is full at 1.8 times (about 27). Its neighbours then expect up to 50% more from a war against it, the war gets an extra push of its own, and its land counts at full value (the base game counts the land of a very large kingdom above a certain value at half).
- **Coalition.** Weaker kingdoms do not open a war against it alone, but once someone is fighting it, others count part of that strength as their own and join in. Joining others against it costs little or nothing in shared spoils, the less the more dominant it is.
- **The right moment lasts longer** against it: up to 40 days after its wars began instead of 20 (it grows from about 19 towns and castles and is full at 21), and an attacker needs only half its strength alone, because the kingdoms already fighting it count too.
- **Good relations calm the fear.** Each 40 points of relation between the two ruling clans halve the fear (a quarter of it at +80), but it never drops below a quarter.

Your own kingdom counts like any other.

!!! tip
    If you rule a growing kingdom, make friends with the neighbouring rulers. It is the best protection you have against everyone turning on you.

## Wars that stop and start sensibly { #wars-that-stop-and-start-sensibly }

- **Weariness.** The men a kingdom has lost in its current wars, and each peace it has signed lately (the effect fades over 60 days), make it expect up to 30% less from a new war. The same losses make it want peace in the war it is fighting, whether it is winning or losing.
- **Restlessness.** A kingdom with no war against another kingdom for more than 40 days starts to expect more from a war: 2% more for each further day, up to 70% more after 75 days of peace. This is a last resort against endless peace; most wars should come from real causes.
- **The ruler looks for a war.** In the base game, a lord who wants to put a war to his council picks a kingdom at random, often one on the far side of the map, so a kingdom could sit at peace for months beside a neighbour its ruler longed to fight. Now, once an AI kingdom has had 50 days of complete peace (no war with another kingdom, a civil war included, and no war within: no house that broke away holding its fiefs against the crown), its ruler weighs every day each kingdom it could fight: one with a common border, no truce, nothing in the rules that forbids it. He takes the one he would most gladly fight and, if that war is worth what any war needs and his council leans towards it, puts it to the council himself, paying the same influence as anyone. A ruler whose council would vote him down keeps his influence and waits. The council votes as always, and the reason given is the real one. If no war is worth it, nothing happens: peace goes on. A kingdom you rule is never pushed: you decide. If you serve an AI ruler, his proposal comes before the council, and to you, like any other. The other lords' own proposals go on as in the base game.
- **Feuds hold wars back.** A kingdom whose houses are fighting a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses), or have one waiting to resume, is slower to start a new war abroad: the larger the share of its strength caught up in feuds, the more it holds back, and more still while a feud is being fought in arms. This binds your council's vote as much as the AI's. While such a feud lasts, the restlessness of a long peace does not count and the ruler looks for no war; the days of peace still count, so once the last feud is over both come back as strong as those days make them.
- **A feud's hosts are the realm's border.** The towns and castles held by the hosts of a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) between a kingdom's houses count as that kingdom's border when it would otherwise have none with its foe: for its wars, so the game does not force a peace for lack of a border, and for who counts as its neighbour.
- **Civil war.** While a kingdom is in a [civil war](civil-war.md), other AI kingdoms find it harder (not impossible) to attack either side, and its war is never "the right moment" for them.

## Peace needs both sides { #peace-needs-both-sides }

In the base game the kingdom that wants out just leaves, usually paying tribute. Now a kingdom can only make peace if:

- the other side also wants peace: not merely when it would lose nothing by it, but when it is at least three quarters of the way to wanting it enough to ask for it itself; or
- the war is clearly decided: the two war scores are at least 500 apart (on the base game's scale of 0 to 750). For a kingdom that started with six towns and nine castles, that is roughly three towns, or two towns and three castles, or less with heavy losses in the field; or
- the war has lasted 80 days. After that either side can leave as in the base game.

A peace offered to your kingdom always comes to you or to your council, as in the base game.

A house that [breaks with its realm](realm-houses.md#a-house-that-breaks-with-its-realm) founds a league of its own, and no peace is made between them for a long while; after that, they make peace as two realms do. A house with no town or castle that breaks away cannot make peace with the realm it left for as long. Other houses without a kingdom (rebels of the base game, mercenaries) make peace as before.

## Truce and tribute { #truce-and-tribute }

- **Truce.** For 45 days after a peace, neither kingdom's council can declare war on the other (base game: 20 days, and only for the AI).
- **Tribute.** A tribute no longer forbids a war, but it weighs against one: a kingdom that is paid tribute by another thinks twice before attacking it, because the war would end the silver still owed, and breaking a peace whose price is still being paid looks bad. The weight fades as the tribute runs out. A strong cause, such as a hated ruler or lost land, can still outweigh it.

On the kingdom screen, a war you cannot propose shows the reason, for example *"A truce holds with Vlandia: the peace is barely sealed, and to break it now would shame the realm. It has some 33 days yet to run."*. When the tribute weighs, your lords say so among their reasons against a war: *"they still pay us tribute, and one does not take a man's silver and his throat in the same season"*.

The truce and the peace rules also bind your kingdom, whether you rule it or serve it, when it declares war or asks for peace. Attacking someone on the map still starts a war as always.

## Allies called to war

- **The caller stays.** A kingdom that called an ally into a war cannot make peace in that war while the ally is still bound to it (42 days in the base game), and its enemy cannot make peace with it either. The exception is a war that is beyond doubt (war scores 500 or more apart), and even then the peace must still pass the rule above: the other side agrees, the war is decided, or it has lasted long enough. On the kingdom screen: *"The Battanians came to this war at this realm's call. It cannot be left while they are still bound to it."*
- **No ally is called into a lost war.** A kingdom clearly losing a war (its war score 450 or more behind its enemy's) calls no ally into it: not when the war or an alliance begins, not by its council, not by you. A call already answered stands, and an overlord still comes to defend its [vassal realm](vassal-realms.md). This binds your kingdom too, if the rules bind it: an allied lord does not take up such a call in talk, your envoy's errand shows that war greyed with the reason, a message tells you why when your council or a notice would have made the call, and an envoy who arrives after the war has turned brings that word back.
- **The ally leaves with the caller.** When the caller makes peace, the allies it called are at peace with that enemy an hour later, with no tribute either way. In the base game they were left fighting alone.

This also applies to your kingdom: if you are called into a war, you leave it when the caller makes peace.

## Terms of peace { #terms-of-peace }

Besides the kingdom screen's peace proposal (as before), a ruler can set **terms** with an enemy ruler on the **Terms of Peace** screen: he picks what each side gives, sees at once whether the enemy ruler would take it and how each council would vote, and offers it.

- **Where.** In the kingdom screen's Diplomacy tab, choose a war and press **Negotiate terms** beside the game's peace proposal. It costs **200 influence**, paid when you press it, whether or not a peace comes of it; without enough influence, or when terms cannot be set now, the button stays greyed and says why. Or tell the enemy ruler *"Our realms should make peace."* in person, at any time in the war: he first says how he stands, in words, and if you go on (*"Then hear my terms."*) the same screen opens, at no cost; when you close it, he has a last word on how it ended. Any other enemy lord only tells you how his ruler feels. Only a ruler sets terms. Or send an [envoy](envoys.md) from the enemy ruler's page in the encyclopedia: *"Carry your terms of peace to {ruler}"* opens the same screen, at no cost, and **Send these terms** (only for terms the ruler would accept now) sends them under a flag of truce; the ruler answers when the envoy arrives, as the war then stands.
- **The screen.** At the top, the two realms, the day of the war, the enemy ruler's words, and the towns and castles taken from them and lost to them in this war. In the middle, what each side gives: a light, heavy or crushing **tribute** (with the denars a day), every **town and castle** of either realm, and **fealty**. What the rules forbid right now is greyed, and its tooltip says why (under siege, the realm not beaten badly enough, too little land left, land is not bought or sold...). What the enemy ruler would not give can be ticked, but it is marked in red, and he says so. At the bottom, each council (see below), and the ruler's answer: he would accept, wants a little more, is far from it, or will not have it. **Offer** is greyed until he would accept.
- **An AI kingdom gives land only when it is truly beaten.** It gives up a castle only once this enemy has taken a quarter of what it held when the war began (never for a single place), a town only at two fifths (never for one or two places), and never more than one town in a peace; fealty only when it is beaten at least that badly and would accept it under the rules of [vassal realms](#vassal-realms) (in a war of independence, those rules alone). Tribute always comes first.
- **What can be put on the table:** the peace itself; a tribute either way; **towns and castles** of either realm (at most two in a peace, never a realm's last two, none under siege); **fealty**, one realm becoming the other's vassal (never annexation), under the rules of [vassal realms](#vassal-realms); between two realms of the Empire, an emperor clearly beaten by the other may **yield the purple** to them, and his realm is joined to theirs (see [The Empire's own ways](empire.md)). A realm weighs a town or castle it would give up more dearly when it lies deep in its land, is of its own culture, is a town or the seat of its ruler or of a duchy, or would cut its land in two. Land is never bought or sold: a realm that yields a town or castle is paid no tribute in the same terms.

### The councils vote

Terms the enemy ruler takes go at once to the vote of the council of the realm that gives most (the one that yields land, else the one that bends the knee, else the one that pays). The other council is shown dimmed as *"Not asked"*: only how its lords would lean.

- **Before you offer**, each council shows whether it would agree, is divided or would refuse, a bar of support, and the portraits of the heads of its houses under *For*, *Against* and *Aside*. Hover over one to see how strongly that house backs its side and, when there is one, its real reason. For an AI council, you are also told how likely its ruler is to overrule it.
- **How the houses weigh it.** The lords whose towns or castles would be given away always vote against, and cannot be talked round. The other lords weigh the land their realm would lose, more so a place next to their own or in their duchy, or one held by their kin, and a bold or honourable head more than a calculating one; land their realm would receive, more so a place they could hope to be given, one near them, of their culture, or one taken from them in this war; and how the war goes for them: a realm that is losing, fighting more than one war, left with little land, or with the enemy at a house's own walls leans towards peace, one that is winning against it. A house says so: *"The war is lost if we fight on."*, *"Our own walls are next."*, *"The war is going our way. Why stop now?"*, *"would not see Pravend given away"*.
- **The ruler decides at the end, as in any vote of the realm.** His house votes like any other; he has no extra weight. An AI ruler may push through terms he accepted at the table against his council, paying influence and the goodwill of the house that led the other side, or let the council's vote stand. When the vote is over the screen shows its result, house by house.
- **When your council votes**, it votes on the screen at once, not over days:
    - **As ruler:** you see how your lords voted, then **Carry the terms**, **Withdraw the terms** or **Abstain** (leave it to the custom of the realm, as you may in any vote). Following your council is free; going against it costs the influence the game charges a ruler to overrule his lords, and the button is greyed if you lack it. A realm with no other house has no council: your word is enough, at no cost.
    - **As a lord of a realm ruled by another:** you are told your voice is awaited, and the screen opens as soon as you are free on the map. Vote for or against, mildly, strongly or with all your influence (each at the game's cost, half if your side loses), or **Keep out of it**; the bar and the portraits change with your vote. If you do not answer within **3 days**, the council votes without you. Then the ruler decides. A mercenary has no vote.
    - The houses that backed a side pay their influence as in any vote of the realm.
- A town or castle given away goes to the winner's share-out (or to its ruler, if his house is the only one of that realm), and its old holder bears a grudge against the crown that gave it. Terms refused are not heard again between the two realms for a while.

### The AI too

An AI kingdom that is clearly losing (well behind in the war and short of a town or castle it held) and cannot get a plain peace offers the cheapest terms its enemy would take; one clearly winning, and far stronger, names its price, by the same rules of land, you included. Never before day 40. Its ruling house pays the same influence to put terms as you do from the Diplomacy tab. Terms offered to you arrive as the game's peace offers do, a notice on the map: it opens the same screen with their terms, the forecast of both councils, and **Accept the terms** or **Send the courier back**. Closing it, or letting it pass, is a refusal.

**You** may set terms at any time, whether or not either side is losing; the enemy ruler, and the council that votes, decide.

## Vassal realms

A clearly beaten kingdom may have to swear fealty instead of paying a tribute. See [Vassal realms and annexation](vassal-realms.md). In war and peace:

- **A vassal marches with its overlord** in every one of its wars, without a vote, and makes no wars, alliances or trade agreements of its own.
- **The overlord's peace covers the vassal** in that war. The vassal cannot make that peace itself (*"Only the {overlord} can make this peace for your realm."*), and its enemy has to make peace with the overlord.
- **No war on your own vassal.** To end the tie, release it or demand its annexation from its page under **Tributaries** in the Crown tab. Whoever may not attack the overlord (truce, alliance) may not attack its vassal either, an attacker counts the overlord's full strength against it, and the vassal's against whoever attacks the overlord.
- **Dominance counts a vassal's towns and castles at half** for its overlord.
- **The caller rule above does not bind an overlord and its vassal**: the overlord makes its peace when it likes, and that peace covers the vassal.

## Heirs and old grudges

When a clan leader dies, the heir inherits part of each of the dead leader's relations. The base game always passes on 70%. Now the share is drawn at random for each person, between 10% and 70%. An heir may keep the late leader's friendships and feuds almost whole, or nearly forget them.

## Seeing why { #seeing-why }

- **War proposals.** A clan that proposes a war gives its real reason, for example *"Balgard is ours by right, and the Nords hold it. It is time to take it back."*, *"Our allies are already at war with the Aserai. We should stand with them."* or *"The Khuzaits have grown too powerful. They must be checked while it can still be done."* When recent [incidents between the two kingdoms](events-between-kingdoms.md) are not the main reason but still weigh at least a third as much, they are named after it, here and in the window when war is declared on your kingdom: *"... And the cattle raid on the border is not forgotten either."*
- **The kingdom screen.** When you look at proposing a war, the support shown by the game ("Low support", "Good support"...) is followed by the lords' two main reasons, for or against. For example *"Low support: we have no quarrel with them; the realm is weary of war"* or *"Good support: Sargot is ours by right; we are the stronger side"*. Faith and titles have their own words, for example *"Pravend, the holy city of the Church of Paravenos, is in the hands of the Battanians, who do not even keep the faith. We cannot suffer it a day longer than we must."*, *"Usanc Castle is a castle of our county of Sargot, and the Battanians hold it. The county must be made whole again."* or *"Caladog of the Battanians keeps the Old Ways, not the Church of Paravenos. Between us there can be no lasting trust."*; on the kingdom screen, *"Good support: they hold Pravend, the holy city of the Church of Paravenos; we are the stronger side"*. A lord only names a cause of faith or titles when it is the one that weighs most.
- **Peace on the kingdom screen.** The tooltip of the game's peace proposal adds what is heard most in your council, and the one of **Negotiate terms** says how your lords lean towards a peace with nothing given either way, and their main reasons, for it and against it.
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
- `WarHolyCityEnabled`: kingdoms want back the holy city of their faith.
- `WarFaithLandEnabled`: lands of the ruler's faith under a ruler of another faith are coveted.
- `WarRulersFaithEnabled`: rulers' faiths push toward war or peace.
- `WarTitlesEnabled`: towns of duchies and castles of counties lost to another kingdom count as land to take back.
- `WarTitleVotesEnabled`: dukes and counts of the border vote for a war more, those far away a little less.
- `WarWearinessEnabled`: war weariness and the wish for peace after losses.
- `WarAmbitionEnabled`: restlessness after a long peace.
- `WarAfterLongPeaceEnabled`: the ruler looking for a war after a long peace (`WarAfterLongPeaceDays`, 50, is how long).
- `PeaceNeedsOtherSideConsent`: peace needing both sides.
- `TruceEnabled`: the 45-day truce.
- `WarTributeWeightEnabled`: a tribute weighing against a war on the realm that pays it.
- `WarDuringFeudPenaltyEnabled`: feuds holding a kingdom back from new wars; `WarWaitsForFeudsEnabled`: restlessness and the ruler's search for a war waiting while a feud lasts.
- `DiplomacyRulesApplyToPlayerKingdom`: the truce and peace rules also binding your kingdom.
- `CallerStaysWhileAlliesAreBound`: a caller cannot leave while its ally is bound.
- `CallerPeaceCoversCalledAllies`: called allies make peace with the caller.
- `NoCallWhileLosingEnabled`: no ally called into a war the caller is clearly losing (`NoCallWhileLosingWarScoreGap`, 450).
- `WarBarSmoothingEnabled`: the bar for a war against a rich kingdom rising less with its wealth.
- `HeirRelationEnabled`: heirs inheriting a random share of relations.
- `NegotiatedPeaceEnabled`: terms of peace; `NegotiatedPeaceAiEnabled`: AI kingdoms offering and demanding terms.
- `WarSupportExplained`: the reasons for a war or a peace on the kingdom screen.
- `WarDeclaredOnPlayerShowsReason`: the window when war is declared on your kingdom; `WarDeclaredOnPlayerPausesGame` set to `false` shows it as a map notice instead.
