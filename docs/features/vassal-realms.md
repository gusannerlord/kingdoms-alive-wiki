# Vassal realms and annexation

A beaten kingdom no longer just pays and walks away. It can bend the knee: it keeps its ruler and its lands, pays tribute every day and marches in its overlord's wars. Over the years the two crowns may become one, or the vassal may rise and break free. AI kingdoms do this to each other too, and your own kingdom can end up on either side.

## How a realm becomes a vassal

### Fealty as the price of peace

A kingdom that is clearly winning a war can ask fealty instead of tribute. It can only ask when all of these hold:

- it is **300 or more** ahead in the war score (the same "decided war" mark as for [peace](war-and-peace.md#peace-needs-both-sides));
- the loser holds at most **0.85 times** a kingdom's even share of the towns and castles (about 12 on the usual map);
- the winner is at least **1.2 times** as strong;
- the winner has fewer than **2** vassal realms, and a free alliance place (see [What the overlord owes](#what-the-overlord-owes));
- neither of them is a vassal already, and neither is in a [civil war](civil-war.md).

It takes a crushing defeat. The loser will not even listen until the winner has taken from it, in this war, at least **40% of the towns and castles it held when the war began** (at least one). A realm of 10 fiefs must lose 4, a realm of 3 must lose 2.

Then the loser decides by adding up points. It bows at **7 points** or more:

| What weighs | Points |
|---|---|
| War score beyond 300 | +1 for each 150 more, up to +2 |
| Towns and castles the winner has taken from it in this war (net) | +1 each, up to +3 |
| Strength | 1.5 times as strong: +1; twice as strong or more: +2 |
| Relation of the two rulers | +1 at 30 or more, −1 at −30 or worse, −2 at −70 or worse |
| It is also at war with another kingdom | +1 |
| Its ruler is valorous | −1 |
| The crown itself is asked, not fealty (it refused to be annexed and lost the war that followed) | −2 |

Between AI kingdoms, a peace that carries such terms says so in the council vote: *"The {loser} swear fealty to the {winner}: they keep their crown, pay tribute and march in its wars."* Each house of the loser votes against it more the worse its leader stands with the winner's ruler. If the loser refuses, the winner insists for **30 days** and takes no other peace meanwhile; after that it settles for an ordinary peace. An AI winner only asks another AI kingdom when it would accept. Between AI kingdoms this is rare, an end-of-campaign event: it never happens before **day 500** of the campaign. A war of independence or of annexation between a vassal and its (former) overlord is the exception: there the beaten side bows at 5.5 points, with no share of fiefs needed and no day limit.

### Demanding it yourself

If you rule your kingdom, every enemy appears in the **Vassals** tab of the kingdom screen, with how the war stands told in words: *"You are at war with the {enemy}. The war has gone well enough for you that they could be made to listen. They still hold {N} towns and castles, and your hosts are stronger than theirs."* Then comes their answer as it stands: *"They are ready to bend the knee, if you demand it."* or *"They will not bow yet: ..."* with the two things that weigh most against it (for example *"their ruler is too proud to kneel"*).

- **"Demand fealty"** is greyed out with the reason while you cannot ask (*"The war has not yet turned far enough your way: beaten kings kneel, and they are not beaten yet."*, *"Their realm is still too great to kneel to anyone: [...] Cut it down to size first."*, *"You already have as many vassal crowns as one overlord can keep in hand."*...). If they would accept, you confirm and the war ends with them as your vassal. If not, they simply refuse: *"The {enemy} refuse: ..."*.
- **Face to face.** Talk to the enemy ruler, choose *"There is something I'd like to discuss."* and then *"Bend the knee to the {your realm}, and this war ends."* (the line only appears when you could ask). With 7 points they agree. A ruler who is close (5.5 points or more) answers *"You ask a great deal. Convince me that it is wiser to kneel than to fight on."* and you argue with the game's persuasion: three arguments (your hosts broken, using Leadership; the count of spears, Tactics; their crown kept, Charm), two must land. How hard each one is depends on the war and on the ruler's character. Further off, they refuse in their own manner (for example *"Kneel? To you? Never, while I can still sit a horse."*), followed by their two strongest reasons (such as *"I still hold the better part of my realm; take it from me first, if you can."*).
- After a refusal or a failed persuasion, that ruler will not hear of it again for **30 days** (**45 days** and **−4 relation** if an argument went very badly). Leaving before a single argument costs nothing.

The tab also counts the fiefs: *"Of the {start} towns and castles they held when this war began, you have taken {lost}. [...] take some {more} more from them, and they may think otherwise."*, until enough have fallen.

### Offered out of fear

A small AI kingdom (at most 0.35 times the even share, about 5 towns and castles or fewer) may offer fealty to the strongest enemy that is at least **1.3 times** as strong and **150** ahead in the war score, if it is surrounded: at war with two or more kingdoms, or having lost two or more towns and castles in the last 60 days. It only offers itself to an enemy that has taken at least **40% of the towns and castles it held when that war began**, as above. It is checked every 3 days with a 2% chance while it stays in that state. Between AI kingdoms, never before day 500. Refused, it does not offer to the same kingdom again for 30 days.

If the offer is made to you, a window **"An offer of fealty"** opens: an envoy of their ruler comes under a flag of truce, in words that depend on the ruler's character (for example *"The {loser} are beaten, my lord, and there are wolves at every border. My king offers to swear fealty to you, if there is peace."*), and the window tells you they would keep their crown, pay you tribute every day and march in your wars: **"Accept fealty"** or **"Refuse"**.

### When you are the one losing

An AI winner asks it of your kingdom by the same rules: 7 points, and 40% of your towns and castles taken in that war. If it does, a window **"A demand of fealty"** opens, and again 15 days later: a herald of {ruler} of the {winner} rides into your camp: *"Your realm is beaten. Swear fealty to my king, and you keep your lands and your crown; you will pay {N} a day and march in our wars. Refuse, and the war goes on."* Answer **"Swear fealty"** or **"Fight on"** (**"Yield the crown"** if they demand your crown). While the demand stands, no other peace with them is possible (*"The {winner} will only make peace if the {loser} swear fealty to them."*). In the Vassals tab that enemy shows *"Demands your fealty"*, with the button **"Offer fealty"** to accept at any time. After 30 days they give up and an ordinary peace is possible again.

## What a vassal owes

- **Relation:** the two rulers gain **10** relation when the vassal offered its fealty, and lose **10** when it was beaten into it.
- **Tribute every day**, for as long as it is a vassal: 3.5% of the combined prosperity of its towns and castles, between **200 and 2,500 denars a day**, worked out again every 6 days. It never runs out. In the Diplomacy tab it reads *"Vassal tribute: {N} per day, for as long as they are vassals."*
- **It marches in every one of its overlord's wars**, with no choice and no vote, a few hours after the war starts. If it is your kingdom: *"Word comes from {ruler}: the {overlord} are at war with the {enemy}, and by your oath your realm marches with them."* When the overlord makes peace, its peace covers the vassal in that war.
- **No wars, alliances or trade agreements of its own.** The buttons are greyed out with the reason: *"Your realm is a vassal of the {overlord} and cannot wage wars of its own."*, *"A vassal realm makes no alliances of its own..."*, *"A vassal realm makes no trade pacts of its own."* Alliances and trade agreements it had end when it bends the knee, and its wars where the overlord is at peace end too. It cannot make peace in its overlord's war either: *"Only the {overlord} can make this peace for your realm."*

If you attack someone on the map as a vassal, that war stands, but it is yours alone: your overlord's ruler likes you **10** less and does not come to help.

## What the overlord owes

- **Defending the vassal.** When someone attacks a vassal, its overlord is called. An AI overlord comes unless it already fights 2 or more kingdoms, the attacker is 1.5 times as strong, or the attacker is its own ally. If you are the overlord, you get the game's call to war (*"A rider of the {vassal} brings grim word: the {enemy} have fallen upon them, and they call on you as their overlord. Bring your realm to war on the {enemy} within 6 days. A vassal left to stand alone does not forget."*; in a realm with only your house: *"[...] Answer the courier before the day is out, or declare war on the {enemy} yourself within 6 days. [...]"*). Answering costs you nothing and your council backs it. Coming to its defence is a favour (**+10**); not coming is a grievance (**+25**): *"The {overlord} did not come to the defence of the {vassal} against the {enemy}. It will not be forgotten."*
- **No war on the vassal.** *"The {kingdom} are your vassals. Release them or demand their annexation from the Vassals tab."*
- **Giving back lost fiefs.** A town or castle the vassal lost to a third kingdom (in the last 120 days) and that the overlord retakes goes back to the house that held it: a favour (**+8**). If you are the overlord, a window **"A fief of your vassal"** asks: **"Return it"** or **"Keep it"**, which is a grievance (**+20**). If you took it as a lord of an AI overlord, you lose it: it goes back to the vassal, and you are told so.
- **Alliance places.** The tie rides on the game's own alliance, so the two show as allies. Each vassal takes one of the overlord's **two** alliance places.

Kingdoms that may not attack the overlord (a truce, tribute, an alliance) may not attack its vassal either: *"The {kingdom} are under the protection of the {overlord}."* An attacker counts the overlord's full strength against it, and the vassal's against whoever attacks the overlord. No [events between kingdoms](events-between-kingdoms.md) happen between an overlord and its vassal.

## Loyalty

Every vassal has a loyalty from 0 to 100. It starts at **55** if the vassal was beaten into it, **65** if it offered (10 less if it rebelled against the same overlord before). Each day it moves a little toward a target (about halfway in 17 days). The target starts at 60 and adds:

| Piece | Effect |
|---|---|
| Power of the overlord | 0 when the overlord is 1.25 times as strong; up to **+30** at 2.5 times; about −10 at equal strength, down to **−30** when the overlord is only 0.6 times as strong |
| Relation of the rulers | 0.3 per point (±30 at ±100) |
| Tribute | **−8** while it pays |
| Habit | +0.1 a day of fealty, up to **+15** after 150 days |
| Wear of the overlord's wars | grows while the vassal is dragged into its overlord's wars and fades in peace; about **−22** at most, after a long time always at war |
| Whispers of a rival | up to **−20** (see below) |
| Grievances and favours | from the defence, the fiefs and the rest; each halves every 60 days |

The **rival** is an AI kingdom on the vassal's border that is at war with the overlord, or whose ruler stands at −20 or worse with the overlord's. The stronger it is next to the overlord, the louder it whispers (nothing below 0.6 times, the full 20 at 1.2 times); half as loud if its ruler dislikes the vassal's, and half again if it is at war with the vassal itself. Other grievances: the overlord breaking with another of its vassals by force (**+15**), and a new ruler taking the overlord's throne while the old one lives, after a civil war (**+10**).

The loyalty reads as **Devoted** (80 or more), **Loyal** (60), **Restless** (40), **Defiant** (25) or **Rebellious** (below 25). The Vassals tab shows the same breakdown and a history of what happened (*"Day 412: its overlord came to its defence against the Vlandians"*). If you rule a vassal's overlord, ask its ruler *"How stands your realm toward ours?"*: from *"We stand with you, in this war and the next..."* down to *"I will not lie to you: my realm would be free of you if it could."*, and *"And the {rival} whisper sweet things in my ear."* when a rival is at work.

## Rebellion

An AI vassal whose loyalty stays **below 25 for 6 days** may rise, with a 1 in 10 chance each day, but only if its strength (plus its rival's, if the rival would fight with it) reaches 60% of the overlord's strength, counting only half of what the overlord's other enemies tie down. The rival fights at its side if its ruler likes the vassal's (relation 0 or more): the two ally and the rival declares war on the overlord.

The rising is a war of independence: *"The {vassal} have renounced their fealty to the {overlord} and taken up arms, with the {rival} at their side."* The two rulers lose **30** relation, the tribute stops, and the vassal makes peace with the enemies it fought only for its overlord. A peace without terms leaves it free. If the overlord wins clearly, it can ask fealty again.

If you rule a vassal realm, you choose when: **"Renounce fealty"** in the Vassals tab, or tell the overlord's ruler *"I renounce my fealty."* (*"So. Say it plainly, and know what follows."*). A window tells you how your hosts compare with theirs and whether a rival would ride at your side, then **"Renounce"** or **"Not yet"**.

## Release

If you rule an overlord, **"Release"** in the Vassals tab frees a vassal: *"They will owe you nothing more, and think the better of you for it."* The rulers gain **10** relation and a normal 45-day truce starts. A vassal whose overlord is destroyed is free too.

## Annexation

There are four ways for a vassal to be joined to its overlord's realm for good. Between AI kingdoms all of them are rare.

**1. Years of loyalty.** Once the vassal's loyalty has stayed at **70 or more for 90 days**, the realms may be joined. An AI overlord proposes it now and then (1 in 4 every 7 days). The vassal accepts if its ruler's relation with the overlord's is 0 or better; otherwise it refuses and the 90 days start again. If you rule the overlord, the button is **"Propose union"**: greyed while *"The {vassal} are not ready to give up their crown: they must first live content under you a good while yet. If their mood holds as it is, some {N} days more."*, then telling you *"They are ready: {ruler} would give the crown to you."* or *"They will refuse: {ruler} has no love for you. [...]"*.

**2. The vassal ruler's death.** When the vassal's ruler dies, the overlord's ruler stands in the game's own vote for the crown, always as a **fourth candidate** next to the usual three, from 48 days of fealty (at once with a marriage, below). Each house backs them more the higher the loyalty and the better its leader stands with them. If the council chooses them, the realm is joined: *"The council of the {kingdom} has chosen to bow to {ruler} of the {overlord}; the two crowns are one."* If you are that overlord, a window **"A crown offered"** lets you **"Accept"** or **"Let them choose their own"** (the next candidate takes the crown).

**3. A royal marriage.** A marriage between the two royal families (a ruler or a ruler's son or daughter, on each side) gives the overlord a strong claim: *"With the marriage of {A} and {B}, the {overlord} has a strong claim to the crown of the {vassal}: when {ruler} dies, its council will weigh it heavily."* It weighs heavily in that vote, lets them stand in it at once, and makes the houses far more willing to stay at the annexation.

**4. By force.** After **72 days** of fealty an overlord can demand the crown. The vassal gives it up if its loyalty is **60 or more** and the overlord is **1.8 times** as strong; otherwise it refuses and there is war: *"The {vassal} refuse to give up their crown, and the {overlord} march on them."* If they refuse and it comes to war, the overlord's ruler loses **10** relation with each honourable lord of their own realm and **100 influence**, and every other vassal of theirs takes a grievance (**+15**). An accepted demand costs nothing. An AI overlord only does this at peace, at least 2.2 times as strong, with a ruler without Honor, and rarely. If you rule the overlord, the button is **"Demand annexation"**, with their answer in the hint. Win the war that follows and you can demand the crown itself (**"Demand their crown"**, in the tab or face to face); a peace without terms leaves them free.

**If you rule the vassal**, you get the windows: **"A union of crowns"** (**"Accept"** / **"Decline"**) and **"A crown demanded"** (**"Accept"** / **"Refuse: war"**). Your house keeps its fiefs and joins the overlord's realm as a house of it.

### How each house decides

Each house of the vassal joins if its leader likes the overlord's ruler well enough (less so by force, more with a royal marriage, less if it loved its old ruler). One that hates them and holds a fief rises against the new realm; the rest leave for another kingdom (never yours), of their own culture first. The old ruling house keeps its word if it agreed. Mercenaries leave. The news: *"The {vassal} are no more: their houses now serve {ruler} of the {overlord}, save {N} that would not."*

If your house belongs to the annexed realm but is not its crown, a window **"A new liege"** asks: **"Swear"** or **"Leave, keeping my fiefs"** (with fiefs, your house rises against the new realm; without, it simply leaves).

## The Vassals tab

The kingdom screen (**K**) has a **Vassals** tab after Court and Factions. It lists your vassals (loyalty, mood and tribute a day), your overlord and its other vassals, the enemies you could ask fealty of, any enemy that *"Demands your fealty"*, and every other vassal realm in Calradia (*"Vassal of the {overlord}"*). Pick one for the details, the loyalty breakdown and its history. Only a ruler gets the buttons.

The encyclopedia page of a kingdom also says *"Vassal realm of the {overlord} since day {N} ({mood})."* or *"Overlord of the {list}."*

## Civil wars and large kingdoms

- A vassal realm never has a plot or a [civil war](civil-war.md). A plot under way in a realm that becomes a vassal dies quietly.
- In the fear of a [kingdom that grows too much](war-and-peace.md#a-kingdom-that-grows-too-much), a vassal's towns and castles count **half** for its overlord.

!!! note
    While the main story's quest is under way, your own kingdom cannot take or become a vassal, or renounce its fealty: *"Not while the story's quest is under way."*

## Turn it off

In the settings file, set a switch to `false`. See [Settings](../settings.md).

- `VassalageEnabled`: the whole feature. Ties already in your save sleep and wake up if you switch it back on.
- `VassalRealmsEnabled`: no new vassal realms, by demand, by offer or from the Vassals tab; existing ones go on.
- `VassalAiDemandsEnabled`: AI winners no longer ask fealty as the price of peace.
- `VassalFearOffersEnabled`: no offers of fealty out of fear.
- `VassalLoyaltyEnabled`: loyalty no longer moves.
- `VassalRebellionEnabled`: AI vassals never rise.
- `VassalFiefReturnEnabled`: lost fiefs are not given back.
- `VassalAnnexOnDeathEnabled`: the overlord's ruler no longer stands in the vote for the crown.
- `VassalAnnexLoyalEnabled`: no union after years of loyalty.
- `VassalAnnexForceEnabled`: AI overlords never demand annexation (you still can).
- `VassalAnnexMarriageEnabled`: a royal marriage gives no claim.
- `VassalDominanceHalfEnabled`: a vassal's fiefs count whole for its overlord's dominance.
