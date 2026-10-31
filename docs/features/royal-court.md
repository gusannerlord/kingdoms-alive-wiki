# The royal court

Every kingdom now has a court. Five offices, held by real people whose skills matter, help run the realm. A ruler does not have to see to every small matter in person: they can send others to deal with the affairs of the realm, hold court in their own halls to hear petitions, and must win the oath of every house when they come to the throne. As a vassal you can be offered an office, hold court in your own fiefs and swear (or not) to each new ruler.

## The kingdom screen

The kingdom screen (**K**) has three new tabs after Diplomacy: **Court**, **Factions** and **Vassals** (see [Vassal realms and annexation](vassal-realms.md)). The usual tabs are unchanged, and with War Sails the Fiefs tab still shows your ships.

The **Court** tab lists:

- **The Crown**, picked first: the ruler's portrait, the realm's law of succession, the ruler's [right to rule](succession.md) as a bar with the words the lords use for it, the portraits of the heir and of the strongest pretender, and the houses with a [claim to the throne](succession.md#claims-to-the-throne) and why;
- the five **offices**, with each holder's portrait and name, or *Vacant*. Pick one to see who holds it, their skill, how much of the full effect they give (*"... 50% of the full effect"*) and what it gives right now;
- **Petitions**: how many people are waiting for you to [hold court](#holding-court) (*"N waiting"*, or *"N waiting, fiefs losing loyalty"* once the wait starts to cost you);
- **Oaths of fealty**: while the houses are swearing to a new ruler, where each one stands.

The **Factions** tab shows the mood of the houses and what you know of the feuds, factions and plots in your realm, and is where you raise the banner if you lead a plot. See [Civil war](civil-war.md#the-factions-tab) and [Factions and grievances](factions.md).

!!! note
    If another mod also replaces the kingdom screen, only one of them can work.

## The offices

| Office | Skill | Full effect |
|---|---|---|
| **Marshal** | Leadership and Tactics (the average) | +0.5 militia and +0.5 security a day in every town and castle of the realm, whoever holds it; villages +0.125 militia a day. Also leads the realm's armies and carries the ruler's orders to the lords (see [Command your armies](command-your-armies.md)) |
| **Steward** | Steward and Trade (the average) | +4% tax in the towns and castles of the ruler's own clan |
| **Master of Works** | Engineering | +8% construction in the towns and castles of the ruler's own clan |
| **Chancellor** | Charm | +0.5 influence a day for the ruler's clan; less of the goodwill toward the ruler a house loses over the [crown's wrongs](factions.md#lords-remember): a good one spares about a third, and only a truly exceptional one half (a small wrong may then cost no goodwill at all, now and then; the grievance itself is remembered just the same); with the old [discontent of large kingdoms](civil-war.md#discontent-off-by-default) turned on (off by default since 1.27.1), also 15% less of it |
| **Warden of the King's Peace** | Scouting and Leadership (the average) | +0.3 security a day in every town and castle of the realm, whoever holds it |

!!! note "The Warden and the King's Writ"
    A free man-hunter who carries an AI ruler's [writ](kings-writ.md) holds that realm's Warden seat for as long as the writ lasts, without being of the realm. AI rulers never give the Warden seat to your house any other way.

- **Skill decides how much.** A holder with skill 30 or less gives nothing; at 250 or more, the full effect. In between it grows steadily: about half at 140.
- **A place at court is an honour.** The clan of each holder gets **+0.3 influence a day** (once per clan, however many offices it holds). The ruler's own clan does not get this.
- **The Marshal leads the armies.** Whatever their skill, the Marshal is the one who takes the ruler's war aims and carries them to the lords; as ruler you give your orders through them, and as Marshal you take your liege's. See [Command your armies](command-your-armies.md).
- One office per person. A holder who is a prisoner, in hiding or away on another task keeps the office, but it gives nothing until they are back. Someone [sent](#sending-others-on-the-realms-business) on an affair that belongs to their own office keeps working while away.
- You see the bonus in the game's usual tooltips, for example *"Marshal (Name)"*.
- An office falls vacant when its holder dies, leaves the realm, becomes ruler or (a companion) leaves the ruler's household. You are told: *"The office of {office} of {realm} is vacant..."*

### Naming your court (as ruler)

Only the ruler names the court. Anyone adult in the realm can serve: nobles of any house of the kingdom (your own included) and, at your court, your family and **companions**. Mercenaries cannot.

You name someone **in person** (only the Marshal can also be offered by rider):

- **By talking to them.** Say *"I would have you serve at my court."* (for a lord of another house it is under *"There is something I'd like to discuss."*), then pick the office: *"As my {office}."*, or *"As my {office}, in place of {holder}."* Hovering shows what they would give.
- **From the Court tab.** Pick an office and press **Appoint**. The list shows everyone who could take it, with their skill. Only people with you can be picked: in the same town or castle, in your party, or in your army. Anyone else is greyed out with *"Speak to her/him in person: she/he is not in this town or castle, nor in your party or army."*. Press **Dismiss** to relieve a holder.
- **By rider, for the Marshal only.** From any town or castle of your realm, or through a companion or family member riding with you, a rider can offer the office of Marshal to a lord of another house, wherever they are. See [Riders](command-your-armies.md#riders).

Who says no:

- Family and companions always accept.
- A lord with relation **below −10** with you refuses: *"An honour, but I would rather not serve you just now. Ask someone else."* In the Court tab they are greyed out: *"She/He would not take an office from you now."*
- A lord secretly in a plot does not give himself away: he accepts the office.

What it costs or gives:

- Naming a lord of another house pleases that house: **+5** with its head (once every 120 days per house).
- Clan leaders with more renown than the house you chose, and less than 30 relation with you, feel passed over: **−3** each.
- Dismissing or replacing someone of another house costs **−15** relation, they cannot be named again for 60 days, and their house leans a little towards plots for a while. Dismissing your own family or companions costs nothing.

When you come to the throne, you inherit the old ruler's court and can keep it or change it.

### AI rulers and their courts

- Every AI ruler fills their court every 30 days, choosing the most skilled nobles of the realm, with a preference for those they like. They pass over houses involved in a plot and houses that refused them the oath.
- They replace a holder only for someone clearly better, or one who has been unable to serve for about a month.
- For **Marshal** they prefer a lord who leads their own party in the field over one who keeps to their hall, whatever the skill; they look elsewhere only if no such lord is to be had. When the Marshal's seat falls empty, the ruler fills it within a day or two, not at the next monthly look.
- They dismiss a holder who leads a plot once it is talked about in the realm.
- A new AI ruler keeps the old court for 15 days before changing it.
- An empty office does not wait for the monthly look: an AI ruler fills it within a few days (4 to 8), once a new ruler's first 15 days are over. If the best choice is of your house while an office is already being offered to you, the seat goes to the best of the others instead of staying empty.

### The Marshal's burden

When a fief of the realm falls to a siege and no army of the realm marched to it or lingered near it, nor any lord fought for it or stood within its walls, its house blames the crown and the **Marshal** too: a smaller grudge against the Marshal's house, and the head of the house thinks less of the Marshal (about half of what the ruler loses for it, a good Chancellor or not). Not when the Marshal is of the house that lost it, or of the ruler's own house or family: then the crown already answers for it. If you are the Marshal, you will hear of it. See [Factions and grievances](factions.md#lords-remember).

**Offers to you.** If you or a noble of your family is the best choice for an office, the ruler sends a letter, **"An office at court"**, saying what the office would give. **Accept** for the office and **+10** relation with the ruler. **Decline** costs **−5** relation, and that ruler will not ask again for 60 days. Your companions are never offered offices by an AI ruler.

**Holding an office for an AI ruler.** Your office works for the whole realm according to your skill, and your clan gets the +0.3 influence a day. As **Marshal** you also take your ruler's war orders (see [Command your armies](command-your-armies.md#as-a-vassal-the-marshal)), and you can ask your ruler for that office yourself. A ruler never replaces you as Marshal with someone better suited: only if you have been unable to serve (a captive, or away) for about a month, or no longer may hold it (you leave the realm, for instance). The [affairs of your kingdom](realm-affairs.md) that belong to your office come to you as the ruler's charge: the messenger rides from the ruler, and the rewards are bigger. Leaving a charge undone as Marshal or Steward costs relation with the ruler.

## Sending others on the realm's business

When an [affair of your kingdom](realm-affairs.md) comes up (a free company, a revolt, a hungry town, bad blood between two houses), a messenger brings you the news on the road and you can answer, as with the game's own quests, that someone else will see to it:

- *"One of my companions or kin will see to it."*: someone riding in your party goes, with men you pick in the game's troop screen.
- *"My vassals will see to it."* (if you rule): a house of your realm sends one of its lords (never its head) with soldiers from its own garrison. The list shows your relation with the head of each house, the chance it accepts and the influence it costs (30 at relation 0, less the better you stand with them, between 10 and 50). A house on bad terms with you may refuse: never at relation 0 or better, always at −30 or worse.
- The holder of the fitting office is listed first: Marshal for sellswords and revolts, Steward for hunger, Chancellor for bad blood.

Whoever goes is away for some days and has an entry in your quest log until they are back. How it goes depends on their skill: at 120 it is safe, below that it takes longer and may fail. What you entrust never gives you more than doing it yourself. The work of the realm cannot be entrusted. Full details: [Someone else sees to it](realm-affairs.md#someone-else-sees-to-it).

## Holding court

People come to ask you for things, and you hear them by holding court in one of your own towns or castles.

### Who comes, and how often

- As **ruler**, a new request arrives every **25 to 30 days**, from anywhere in the realm. As a **vassal** with fiefs of your own, every **62 to 75 days**, only from your own fiefs, and never the requests marked "ruler" below.
- You are told who asks and for what, for example: *"{Who} has come to ask you for {what}, and waits to be heard at {place}."* As ruler, a lord's request reads *"... Hold court in one of your own towns or castles and they will ride there to be heard."*
- Up to **5** can wait at once. The Court tab lists them under **Petitions**, by where they come from.
- While your realm is at war, no new request comes, and the waiting of those already there does not count: nobody gives up and nothing is held against you. A ruler with no town or castle of their own gets no new requests, and the waiting does not count either.

### "Hold court"

In the menu of one of **your own** towns or castles, choose **"Hold court"**. Hovering over it shows who is there now, which notables have a task for you, who would ride there and in about how many days, who cannot come and why (*"at war with us"*, *"with an army"*, *"hosting guests"*...), and about how long it should take.

- Riders go out to every lord who asked to be heard, **however far** they are. A lord with a party rides there; one without travels on their own. When one arrives you are told: *"{Lord} has arrived at {place} and waits to be heard."*
- You wait in the hall with the game's progress bar. The hall takes a couple of hours to make ready. Then each petitioner comes before you **in turn, as they arrive**: the conversation opens by itself, and the clock stops while you talk. Each request has two to four answers.
- **As ruler**, everyone else with a request (notables and common folk from any town or castle of the realm) comes to whichever of your halls you sit in. **As a vassal**, each is heard in the town or castle their request belongs to.
- **Then the notables.** Notables of the town and its villages who have one of the game's own quests to offer come before you too, with the game's usual quest conversation: accept it, turn it down or send a companion, as in the base game.
- The court ends by itself when everyone who could come has been heard, or when the bar runs out (those still on the road go home). **"Rise from court"** ends it early, and leaving the place ends it too.
- With nobody to hear, the button is greyed out and says why: *"Nobody is waiting to be heard."*, *"Nobody here asks to be heard. Those waiting are at: ..."* or who cannot come now.
- It cannot be held while the place is under siege.

### The requests

| Request | Who asks | Your answers |
|---|---|---|
| **a fief** (ruler) | the head of a house of your realm without land | Promise the next fief the crown grants (**+8**; **−15** if it goes to someone else or none comes within 120 days), put them off kindly (a Charm roll; −3 if it fails), or refuse (**−6**). |
| **gold to raise troops** (ruler) | a lord whose party is under half strength | Give 3,000 denars plus 1,000 per clan tier, at most 8,000 (**+6**), or refuse (−2). |
| **abuses of a lord** (ruler) | a village notable, against the lord who holds their town or castle | Reprimand the lord yourself (−8 with them, +10 loyalty there, +5 with the notable), send it back to the lord (−5 with the notable), or have your **Marshal** look into it: after 5 days the complaint may turn out false. |
| **freedom from dues** | a merchant of your town | Grant 60 days without dues (10% less tax there, **+1 prosperity a day**, shown as *"Merchants' exemption"*, and +6), lend 5,000 denars to be repaid in 60 days (+3), or refuse (−4). |
| **a quarrel over land** | two notables of one place | Give the land to one or the other (+6 / −6; the two also grow **5** closer to each other), split it (+2 each; the two grow **15** closer), or let them settle it. Heard or not, the same two do not bring it again for 120 days. |
| **a widow's pension** | a soldier's widow, after a battle you fought | Pay 500 denars (+2 loyalty there) or refuse. |
| **a prisoner's freedom** | the house of a lord you hold prisoner | Free them (+10 with the house head), ransom them for twice the usual price, or keep them (−5). |
| **a place in your guard** | an old soldier | Take him: a seasoned (tier 5) soldier of your culture joins you. |
| **works for the town** | a master builder, in your town or castle | Pay 85% of a building's cost: it goes into the town's building fund and that building goes first. |
| **refuge in your realm** (ruler) | a lord of a foreign kingdom at war with another | Shelter them: **+8** with their ruler, but tension with the enemy kingdom rises (see [Events between kingdoms](events-between-kingdoms.md)). Or stay out of it. |
| **a place in your house** | a distant kinsman (needs a free companion slot; at most once every 3 courts) | Take them in: a new companion of your culture joins your party. |
| **help with a marriage** (ruler) | two unmarried lords of different houses | Speak to both houses: a Charm roll; on success they marry and both house heads think better of you (+5). |
| **a fief of yours their house claims by right** (ruler) | the head of a house of your realm with a [right](fief-rights.md) to one of your own towns or castles; most often one near its own lands, and a firm right more often than a weak one | Grant it: the fief is theirs (**+15**; not your last town or castle, nor one under siege). Put it off: a Charm roll, −3 if it fails. Refuse: **−6**, and the house holds it against the crown (see [Lords remember](factions.md#lords-remember)). Heard or left waiting, the same house does not ask for the same fief again for 120 days. |

Charm rolls show their odds in the answer: 35%, plus 0.25% per point of Charm (+25% per 100), up to 85% at 200 Charm.

### Leaving them waiting

- A request left unheard for **30 days** lapses, usually with a small loss of relation: *"{Who} has given up waiting to be heard at {place}."*
- Once **20 days** have passed since the oldest request arrived (or since your last court, if that is later), **each of your towns and castles loses 0.1 loyalty a day**. It shows as **"Petitions unheard"** in the loyalty breakdown of each fief, and the Court tab shows *"N waiting, fiefs losing loyalty"*. Every 10 days the lords still waiting lose 1 relation with you, and a message tells you who waits where, which fiefs are losing loyalty and what to do.
- Before that, the **Petitions** panel of the Court tab tells you how many days have gone by and when the loss would start.
- Holding court and hearing at least one petitioner starts the count again.

### The Chancellor hears them for you

As ruler, with a Chancellor able to act, the Court tab offers **"Let the chancellor hear them ({N})"**. Your chancellor decides by their own character (a generous one pays, a merciful one forgives, a mean one refuses), and only a generous one spends your gold, never more than 10,000 per hearing. You see their answers first, in a window **"From your chancellor"**: **"Let it be done"** or **"I will hear them myself"**. Through the chancellor, relation gains are halved, and their Charm decides the rolls. The old soldier and the kinsman will only speak to you in person. A ruler with no town or castle of their own can only have petitions heard this way.

## The oath to a new ruler

When a kingdom gets a new ruler (by succession, by election or by winning a civil war), every house of the realm has **15 days** to swear fealty. A brand-new kingdom has no oath. Nor is there one when a [vassal realm](vassal-realms.md)'s council chooses its overlord's ruler: the realm is joined to the overlord's and its houses swear no oath.

A new ruler's [claim to the crown](succession.md) weighs in every house's answer: a ruler with a strong claim finds most houses ready to swear, one with a weak claim hears more demands and more refusals.

Each AI house weighs it up: its relation with the new ruler, its Honor, whether it voted for them, whether it stood against them for the throne or fought them in a civil war, how close it is to plotting, and kinship.

| A house... | What happens |
|---|---|
| **swears** | **+3** with the ruler; it is less inclined to plot for 120 days. |
| **asks for something** | An empty office, or a fief of the ruler's own clan. If the ruler grants it, the house swears on those terms. |
| **refuses**, or lets the 15 days pass | **−10** with the ruler; the house is **marked** for 180 days: far more inclined to plot, and kept out of that ruler's court. Nobody leaves the realm. |

**AI rulers almost never give up a fief.** A ruler whose own clan holds only 2 towns and 2 castles or fewer never gives one. Otherwise there is a 5% chance, once per house, and at most one fief per oath. Most of the time a house that asks gets an empty office instead. When the 15 days end, about half the time an AI ruler wins back a house that refused, with gold or an office; otherwise it rebukes it (another −10).

### As a vassal

You are told: *"{ruler} is now ruler of {kingdom}. Every house is to swear fealty within 15 days: go to her/him in person to swear, ask for something, or refuse."* Go to the ruler in person, choose *"There is something I'd like to discuss."* and then *"I have come about my oath of fealty."*:

- *"I swear to be your faithful vassal..."*: **+5** relation and **+10 influence**.
- *"I will swear, but I would ask something in return."* (once per oath): ask for an empty office, a fief of the ruler's own clan (only if they have one to spare by the rule above; much harder to argue), or **5,000 denars × your clan tier**. Then you argue it out with the game's persuasion. Win and you get it and swear. Lose and the ruler says *"No. You will have nothing of me for an oath you owe in any case."* (**−5** relation); then swear without terms, refuse, or take more time.
- *"I will not swear to you."*: **−15** relation, and your house is marked for 180 days.
- Not going within 15 days costs **−10** relation, and your house is marked.

### As the new ruler

A window, **"The oaths of fealty"**, lists every house as *likely to swear*, *wavering* or *cold to you*. When a house asks its price (**"A house asks its price"**), you can grant an empty office, one of your clan's fiefs or **5,000 denars × its tier**, or answer *"Nothing: an oath is not for sale"* (it thinks again in 3 days, less willing).

You can also talk to a house that has not sworn: persuade it (*"Hear me out before your house decides."*, once per house), offer it an office or a fief (accepted at once), or press it: *"You will swear, or answer for it. (30 influence)"*, which costs **−10** relation either way and makes it swear 7 times in 10.

## Taking a fief from a vassal

As ruler, you can still put a vassal's town or castle to the council's vote (the **Propose** button on the Fiefs tab of the kingdom screen), but it is no longer free of consequences.

- **Every vassal house worries it is next.** The moment you propose it, you lose **5** relation with the head of every house of your realm: *"Word spreads that you mean to take {fief} from the {clan}. Your vassals wonder whose fief is next..."* What this costs you with any one lord never goes past **−25** in all; the lost relation does not come back, but the room under that limit reopens slowly, about 5 points every 120 days.
- **The holder may refuse.** If the vote passes, the house that held the fief may refuse to give it up, renounce its oath to you and leave your kingdom **with all its fiefs**, at war with you. The same goes for every vote to take a fief, whoever proposed it: an AI ruler, a vassal with a right to it, or you as a vassal; and the same when your own house loses one (you are asked whether you bow or renounce your oath). A window **"A house in revolt"** tells you. Few houses dare it: one house alone against a whole kingdom is a desperate thing. The chance starts at only **10%**. It is higher for a brave, proud head (+15% per level of Valor) or one who hates you, and lower for an honorable one (−10% per level of Honor) or a calculating one (−10% per level of Calculating), who will not take on a kingdom alone. It never goes past 70%. A house that refuses keeps the fief; the vote on who gets it is dropped.
- Otherwise the house **bows** and yields the fief. **What the ruler takes, the ruler keeps:** when the ruler (you or an AI ruler) proposed the vote, the fief passes straight into the crown's hands, with no second vote on who gets it. Since a ruler cannot plot or press a claim, this is how a crown wins a fief it wants. As when a ruler picks their own house in a share-out, the house keeps an old right to it, and a sealed charter that gives conquests to the realm is broken. When anyone else proposed it, the vote on its new holder goes ahead as usual. During the vote, the option to take it reads *"The crown should take this fief into its own hands"* when the crown will keep it.
- A house that is part of a [plot](civil-war.md) may answer with its plot: a strong plot rises at once over the fief, even in a war with another kingdom, and a weaker one may rise, or the house break away alone, or bow, by its head's character (see [A fief taken can set a plot alight](civil-war.md#the-rising)). During a [civil war](civil-war.md), an AI house that refuses goes over to the other side instead (if you renounce your oath, your house stands alone).
- A house riding at your side (in your army, your battle or your siege, or while you are in one of its towns or castles) waits until it is no longer with you before it breaks away.
- **No easy way back.** A house that broke away over a fief does not slip back into peace with the kingdom it left on a whim, as houses without a kingdom do in the base game. It makes peace on the same terms as two kingdoms (see [Peace needs both sides](war-and-peace.md#peace-needs-both-sides)): the crown must be willing, or the war must be clearly decided, or it must have lasted 80 days.

### Winning the votes first

The council usually votes against taking a fief: every lord sides with the holder unless they truly hate them. As ruler you can still force it through with influence, but you can also prepare the ground. This is the second kind of plot, next to the [civil war](civil-war.md).

This is the crown's own business, not a plot: a ruler needs no [right](fief-rights.md) to take a fief back. Talk to the head of another house of your realm and say *"I mean to take a fief back into the crown's hands. When it comes before the council, will your house stand with its king?"*, then pick the house you have in mind. The house you take it from keeps an old right to it.

- **Only a lord with few scruples listens.** Below **30** relation with you they say *"That is not talk for the two of us"*. A lord who is honorable, merciful or generous (any level of Honor, Mercy or Generosity) will not be party to it at all. Valor does not count against them.
- **They will not move against a friend.** If they like the head of that house 20 points or more above you, they refuse outright. The better they like that house, the harder they are to win; if they hate it (−30 or worse), it gets easier.
- **Then you argue it out** with the game's persuasion. Friendship alone does not get you far: your **Charm** counts (one step easier per 100), and so does talking to them at a [feast](feasts.md) or a [hunt](hunts.md) you both attend (one step easier; the two do not add up).

Your chances against a house they have no feelings about:

| Relation with you | Charm 0 | Charm 100 | Charm 200 |
|---|---|---|---|
| 30 to 54 | 1% | 4% | 24% |
| 55 to 79 | 4% | 24% | 32% |
| 80 or more | 24% | 32% | 49% |

If they hate that house, the 30–54 row becomes 7%, 32% and 48%.

- **Won over**, they vote to take a fief from that house the next time you put one to the council, within **60 days**. That vote uses up the promises against that house, whatever comes of it. The [Factions tab](civil-war.md#the-factions-tab) lists them.
- **Failed**, they will not hear of it again for 45 days; a bad failure means 60 days and −4 relation.
- **Word may get out.** Every attempt, won or lost, has a **1 in 5** chance of reaching the house you mean to rob: its head loses **10** relation with you, and you are told.
- Proposing the vote still costs you with every vassal, accomplices included, and the holder may still refuse and break away. Lords who vote to take a fief also lose relation with its holder, as in the base game.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `CourtOfficesEnabled` to `false`: the offices give nothing and nobody is named. The realm's armies then have a Marshal of their own (see [Command your armies](command-your-armies.md#one-marshal)).
- `CourtAiAppointEnabled` to `false`: AI rulers do not name their courts or offer you offices.
- `CourtChargeEnabled` to `false`: holding an office for an AI ruler does not bring you its affairs as the ruler's charge.
- `AffairDelegationEnabled` to `false`: affairs of your kingdom cannot be sent to companions, kin or houses.
- `AudiencesEnabled` to `false`: no petitions and no "Hold court".
- `OathEnabled` to `false`: no oath of fealty when a ruler changes.
- `FiefRevocationEnabled` to `false`: taking a fief from a vassal works as in the base game, with no lost relations and no revolt.
- `RevokeAnyProposerEnabled` to `false`: only the house a vote of yours as ruler (or of a reckoning) strips may refuse.
- `RevokeRulerKeepsFiefEnabled` to `false`: a fief the ruler takes goes to the vote on its new holder, as in the base game.
- `BreakawayPeaceRulesEnabled` to `false`: a house that broke away makes peace with its old kingdom as easily as in the base game.
