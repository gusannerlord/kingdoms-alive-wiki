# The royal court

Every kingdom now has a court. Five offices, held by real people whose skills matter, help run the realm. A ruler does not have to see to every small matter in person: they can send others to deal with the affairs of the realm, hold court in their own halls to hear petitions, and must win the oath of every house when they come to the throne. As a vassal you can be offered an office, hold court in your own fiefs and swear (or not) to each new ruler.

## The kingdom screen

The kingdom screen (**K**) has two new tabs after Diplomacy: **Crown** and **Factions**. The usual tabs are unchanged, and with War Sails the Fiefs tab still shows your ships.

The **Crown** tab lists:

- **The Crown**, picked first: the ruler's portrait, the realm's law of succession, the ruler's [right to rule](succession.md) as a bar with the words the lords use for it, the portraits of the heir and of the strongest pretender, the houses with a [claim to the throne](succession.md#claims-to-the-throne) and why, and the [laws of the crown](crown-laws.md#the-crown-screen) in force, with what each does to the houses' regard and the buttons to change them;
- the five **offices**, with each holder's portrait and name, or *Vacant*. Pick one to see who holds it, a bar with how much of the office's full effect their skill brings (their skill under it, with words such as *"a sure hand"*) and what it gives right now;
- **Petitions**: how many people are waiting for you to [hold court](#holding-court) (*"N waiting"*, or *"N waiting, fiefs losing loyalty"* once the wait starts to cost you);
- **Oaths of fealty**: while the houses are swearing to a new ruler, where each one stands;
- **Titles**: the duchies and counties of the realm, its themes or its ulus, and its landed knights (see [Dukes, counts and castellans](titles.md)); in a realm without titles, **Landed knights**;
- **Vassals of the Crown**: every house of the realm in the tree of lords and vassals, under the crown (see [Liege and Vassals](titles.md#liege-and-vassals));
- under **Tributaries**, the realms tied to yours: your vassal realms, your overlord, and an enemy that demands your fealty (see [Vassal realms and annexation](vassal-realms.md#tributaries-in-the-crown-tab)).

The **Factions** tab shows the mood of the houses and what you know of the feuds, factions and plots in your realm, and is where you raise the banner if you lead a plot. See [Civil war](civil-war.md#the-factions-tab) and [Factions and grievances](factions.md).

Kingdoms Alive adds to the game's screens instead of replacing them (it needs [UIExtenderEx](../getting-started.md#requirements)), so other mods that add to the same screens keep working beside it.

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
- One office per person. A holder who is a prisoner, in hiding or away on another task keeps the office, but it gives nothing until they are back. A Marshal whose house rides in a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses)'s host counts as away: while the realm is at war with another, an AI ruler names another, and you cannot name a lord riding in a host. Someone [sent](#sending-others-on-the-realms-business) on an affair that belongs to their own office keeps working while away.
- You see the bonus in the game's usual tooltips, for example *"Marshal (Name)"*.
- An office falls vacant when its holder dies, leaves the realm, becomes ruler or (a companion) leaves the ruler's household. You are told: *"The office of {office} of {realm} is vacant..."*

### Naming your court (as ruler)

Only the ruler names the court. Anyone adult in the realm can serve: nobles of any house of the kingdom (your own included) and, at your court, your family and **companions**. Mercenaries cannot.

You name someone **in person** (only the Marshal can also be offered by rider):

- **By talking to them.** Say *"I would have you serve at my court."* (for a lord of another house it is under *"There is something I'd like to discuss."*), then pick the office: *"As my {office}."*, or *"As my {office}, in place of {holder}."* Hovering shows what they would give.
- **From the Crown tab.** Pick an office and press **Appoint**. The list shows everyone who could take it, with their skill. Only people with you can be picked: in the same town or castle, in your party, or in your army. Anyone else is greyed out with *"Speak to her/him in person: she/he is not in this town or castle, nor in your party or army."*. Press **Dismiss** to relieve a holder.
- **By rider, for the Marshal only.** From any town or castle of your realm, or through a companion or family member riding with you, a rider can offer the office of Marshal to a lord of another house, wherever they are. See [Riders](command-your-armies.md#riders).

Who says no:

- Family and companions always accept.
- A lord with relation **below −10** with you refuses: *"An honour, but I would rather not serve you just now. Ask someone else."* In the Crown tab they are greyed out: *"She/He would not take an office from you now."*
- A lord secretly in a plot does not give himself away: he accepts the office.

What it costs or gives:

- **A place at court warms a house to its ruler** for as long as it lasts: the head of a house thinks better of the ruler for each office one of his house holds, and the warmth goes when the office does. It never builds up: naming the same house again and again adds nothing.
- Clan leaders with more renown than the house you chose, and less than 30 relation with you, feel passed over: **−3** each.
- **Putting someone of another house out of an office** while they serve, by dismissing or replacing them, leaves their house thinking less of the ruler for a good while, or until one of it is named again; each office lost counts, and it never builds up beyond that. The same for an AI ruler. None if they could not serve at the time. Dismissing your own family or companions costs nothing. The known leader of a plot leaves the court at no cost.
- **One house with more than one office** is resented: while it holds them, every other house of the realm thinks less of the ruler and of that house (if it is the ruler's own, of the ruler). An AI ruler is loath to give a second office to a house that already holds one.
- An office given as a term of a house's oath is kept while that oath binds it.

When you come to the throne, you inherit the old ruler's court and can keep it or change it.

### AI rulers and their courts

- Every AI ruler fills their court every 30 days, choosing the most skilled nobles of the realm, with a preference for those they like. They pass over houses involved in a plot and houses that refused them the oath.
- They replace a holder only for someone clearly better, or one who has been unable to serve for about a month.
- For **Marshal** they prefer a lord who leads their own party in the field over one who keeps to their hall, whatever the skill; they look elsewhere only if no such lord is to be had. When the Marshal's seat falls empty, the ruler fills it within a day or two, not at the next monthly look.
- They dismiss a holder who leads a plot once it is talked about in the realm, at no cost. Replacing anyone else costs them the same little regard it costs you.
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
- Up to **5** can wait at once. The Crown tab lists them under **Petitions**, by where they come from.
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
- Once **20 days** have passed since the oldest request arrived (or since your last court, if that is later), **each of your towns and castles loses 0.1 loyalty a day**. It shows as **"Petitions unheard"** in the loyalty breakdown of each fief, and the Crown tab shows *"N waiting, fiefs losing loyalty"*. Every 10 days the lords still waiting lose 1 relation with you, and a message tells you who waits where, which fiefs are losing loyalty and what to do.
- Before that, the **Petitions** panel of the Crown tab tells you how many days have gone by and when the loss would start.
- Holding court and hearing at least one petitioner starts the count again.

### The Chancellor hears them for you

As ruler, with a Chancellor able to act, the Crown tab offers **"Let the chancellor hear them ({N})"**. Your chancellor decides by their own character (a generous one pays, a merciful one forgives, a mean one refuses), and only a generous one spends your gold, never more than 10,000 per hearing. You see their answers first, in a window **"From your chancellor"**: **"Let it be done"** or **"I will hear them myself"**. Through the chancellor, relation gains are halved, and their Charm decides the rolls. The old soldier and the kinsman will only speak to you in person. A ruler with no town or castle of their own can only have petitions heard this way.

## The oath to a new ruler

When a kingdom gets a new ruler (by succession, by election or by winning a civil war), every house of the realm has **15 days** to swear fealty. A brand-new kingdom has no oath. Nor is there one when a [vassal realm](vassal-realms.md)'s council chooses its overlord's ruler: the realm is joined to the overlord's and its houses swear no oath.

A new ruler's [claim to the crown](succession.md) weighs in every house's answer: a ruler with a strong claim finds most houses ready to swear, one with a weak claim hears more demands and more refusals.

Each AI house weighs it up: its relation with the new ruler, its Honor, whether it voted for them, whether it stood against them for the throne or fought them in a civil war, how close it is to plotting, and kinship.

| A house... | What happens |
|---|---|
| **swears** | **+3** with the ruler; it is less inclined to plot for 120 days. |
| **asks for something** | An empty office, or a fief of the ruler's own clan. If the ruler grants it, the house swears on those terms, and the ruler thinks a little less of it for having to buy its oath (an honourable or valiant ruler more so, a generous or calculating one hardly at all). |
| *(houses riding in a feud's host)* | swear like the rest, within the same days. [Landed knights](landed-knights.md) swear no oath: they are their lord's men. |
| **refuses**, or lets the 15 days pass | **−10** with the ruler; the house is **marked** for 180 days: far more inclined to plot, and kept out of that ruler's court. Nobody leaves the realm. |

**AI rulers almost never give up a fief.** A ruler whose own clan holds only 2 towns and 2 castles or fewer never gives one. Otherwise there is a 5% chance, once per house, and at most one fief per oath. Most of the time a house that asks gets an empty office instead. When the 15 days end, about half the time an AI ruler wins back a house that refused, with gold or an office; otherwise it rebukes it (another −10).

### As a vassal

You are told: *"{ruler} is now ruler of {kingdom}. Every house is to swear fealty within 15 days: go to her/him in person to swear, ask for something, or refuse."* Go to the ruler in person, choose *"There is something I'd like to discuss."* and then *"I have come about my oath of fealty."*:

- *"I swear to be your faithful vassal..."*: **+5** relation and **+10 influence**.
- **By an envoy**: from the ruler's page in the encyclopedia you may send a family member or companion to swear in your name, with no terms (to ask for something, go in person). Your house is sworn the day the envoy stands before the ruler: the same regard any house gets for swearing, but not the extra of kneeling in person, nor the influence. Greyed with the reason if the envoy would arrive too late.
- *"I will swear, but I would ask something in return."* (once per oath): ask for an empty office, a fief of the ruler's own clan (only if they have one to spare by the rule above; much harder to argue), or **5,000 denars × your clan tier**. Then you argue it out with the game's persuasion. Win and you get it and swear, but the ruler thinks a little less of you for it, as of any house that names its price. Lose and the ruler says *"No. You will have nothing of me for an oath you owe in any case."* (**−5** relation); then swear without terms, refuse, or take more time.
- *"I will not swear to you."*: **−15** relation, and your house is marked for 180 days.
- Not going within 15 days costs **−10** relation, and your house is marked.

### As the new ruler

A window, **"The oaths of fealty"**, lists every house as *likely to swear*, *wavering* or *cold to you*. When a house asks its price (**"A house asks its price"**), you can grant an empty office, one of your clan's fiefs or **5,000 denars × its tier**, or answer *"Nothing: an oath is not for sale"* (it thinks again in 3 days, less willing). The window warns you whether granting it would sit ill with you, by your character.

You can also talk to a house that has not sworn: persuade it (*"Hear me out before your house decides."*, once per house), offer it an office or a fief (accepted at once), or press it: *"You will swear, or answer for it. (30 influence)"*, which costs **−10** relation either way and makes it swear 7 times in 10.

## Taking a fief: decree, demand or reckoning {#taking-a-fief-from-a-vassal}

The council votes on taking a fief from a house only in a reckoning. There are three roads, as in the great feudal kingdoms, where taking back land was a lord's own act and not a matter for a vote.

- **The ruler, by decree.** As ruler, the button on the kingdom screen's Fiefs tab reads **Decree**. It opens a confirmation, **"Take {fief} by decree"**, that says what it will cost; there is no vote, and the fief passes into the crown's own hands, with no share-out. The ruler also decrees when backing a [reckoning](factions.md#the-reckoning-of-a-house) or a lord's plea (below).
- **A lord, by demanding it of his own vassal.** As a [duke or count](titles.md#a-lord-takes-back-a-vassals-fief), the same button reads **Demand** on the fiefs of houses that hold their land of you: a fief of your duchy, or a castle of your county. It goes back into your own hands.
- **House against house, only through a reckoning,** which brings the fief to the council's vote. A right alone does not open the button: it is greyed, and tells you the ways open to you (win lords over to a reckoning, or press the right by the sword).

### What it costs

Every time, with no limit and nothing coming back:

- **30** relation with the head of the house that loses the fief, and **10** with the head of every other vassal house of the realm (for a lord: of each of his other vassals), who wonder whose fief is next. If the house that gets the fief holds a firm [right](fief-rights.md) to it, the others lose nothing; the house that loses it still does. The confirmation counts the houses it will cost you.
- The influence the button asks.
- The house that loses it holds it against the crown (or against its lord), and keeps an old right to the fief.

**Never a house's last town or castle.** Neither a decree of the ruler's own nor a lord's demand can take the last town or castle of a house, unless that house is marked as [traitors](realm-houses.md#houses-marked-as-traitors) or is a felon of the one taking it. Nothing is ever taken from the ruling house. The button is greyed with the reason, and the same holds for the AI.

The button is also greyed while the matter is still open (the house is weighing its answer, a reckoning is after it, it rides in a feud, your own feud or plea against that vassal is not settled), while the crown is not yet given after a ruler's death, and in a feud's host. Nothing is paid for a decree that cannot be carried out.

### AI rulers and lords

- **An AI ruler decrees only with a cause, and rarely:** a house he cannot stand, a house marked as traitors or felons of his, or his own coffers running low for a long time. His letter gives the true reason. He never does it during a civil war, nor against a house a reckoning is already after.
- **An AI lord demands only with the same causes, and seldom.** If you are the vassal, your lord's letter gives his true reason.
- **As ruler you decree at will**, with no cause needed.
- A lord never joins a reckoning against his own vassal: his only road to a vassal's fief is to demand it.

### How a house answers

**A decree of the crown.** The house:

- **yields**: the fief passes at once to the crown, or to the house the ruler backed;
- **breaks with the realm**, and founds a league of its own (see [A house that breaks with its realm](realm-houses.md#a-house-that-breaks-with-its-realm)). Lords do not give up their land lightly: the chance starts at **35%** for a town and **20%** for a castle, higher for a brave, proud head or one who hates the ruler, lower for an honourable or calculating one or one on good terms with the ruler, and never below 5% nor above 85%;
- or **raises its plot**, if it is sworn to one (see [A fief taken can set a plot alight](civil-war.md#the-rising)).

It never bars its gates against the crown.

**A lord's demand.** The vassal yields the fief to his lord, or **bars the gates**, by the same weighing, with his regard for his lord in place of the ruler's. Then the lord may take up arms against him in a [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses): if the vassal loses it, he answers for [felony](factions.md#felony); if he holds out to the end, he no longer owes the fief. A vassal never breaks with the realm over his lord's demand. If no feud can be fought that day, he keeps the fief.

**No fief is ever handed over by itself.** If a house that refused can no longer break away, or no sword can be drawn, it keeps the fief. An AI house that refuses while riding at your side (in your army, your battle or your siege, or while you are in one of its towns or castles) waits until it is no longer with you before it breaks away.

When a house does not yield to your decree or demand, a window, **"The answer of the {house}"**, tells you at once what it does.

### A lord's plea {#a-lords-plea}

Under [High Crown Authority](crown-laws.md#high-crown-authority) a lord may not take up arms against his vassal. The vassal who bars the gates keeps the fief, and the lord takes his plea to the throne.

- **An AI ruler** judges it by its cause: against a vassal marked as traitors, or a felon of that lord, he nearly always backs the lord. Otherwise he keeps out of it, unless he has reason: the lord holds a firm right to the fief, the ruler holds the lord very dear, or he hates the vassal; the more reasons, the likelier. He never backs a lord against a vassal he holds very dear.
- **If you are the ruler**, a window, **"A lord's plea"**, offers **"Back {lord} by decree"** or **"Keep out of it"**.
- **Backed**, it is a decree like any other: the vassal yields or breaks with the realm, and the crown pays its usual price (but not with the lord who asked).
- **Shielded**, the vassal keeps the fief, the lord holds it against the crown, and he may demand nothing of that vassal for a season, unless the vassal turns traitor or felon.

### If the fief is yours

- **"A decree of the crown"**: **"Give up the fief"**, **"Renounce your oath"** (you break with the realm and found your league; greyed with the reason if you have no town or castle, or the realm would be left with none), and, if you are sworn to a plot, **"Raise the plot's banner"**. If you choose to rise or renounce your oath and it cannot be done after all, you keep the fief, are told why, and are asked again.
- **"Your lord's demand"**, with your lord's letter and reason: **"Give it up to your lord"** or **"Bar the gates"**, whose tooltip warns you of felony if you lose the feud. You cannot renounce your oath against your lord alone; if you are sworn to a plot, you also have **"Raise the plot's banner"** and **"Renounce your oath"**.
- **"The council's verdict"**, after a reckoning's vote: see [What the stripped house does](factions.md#the-reckoning-of-a-house).

### In the Empire

In a realm of the [Empire](empire.md) the land is the emperor's to give: no lord demands a vassal's fief, and no house takes another's through a reckoning. A right is laid before the throne as a petition instead. The emperor decrees like any ruler.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `CourtOfficesEnabled` to `false`: the offices give nothing and nobody is named. The realm's armies then have a Marshal of their own (see [Command your armies](command-your-armies.md#one-marshal)).
- `CourtAiAppointEnabled` to `false`: AI rulers do not name their courts or offer you offices.
- `CourtChargeEnabled` to `false`: holding an office for an AI ruler does not bring you its affairs as the ruler's charge.
- `AffairDelegationEnabled` to `false`: affairs of your kingdom cannot be sent to companions, kin or houses.
- `AudiencesEnabled` to `false`: no petitions and no "Hold court".
- `OathEnabled` to `false`: no oath of fealty when a ruler changes.
- `FiefRevocationEnabled` to `false`: taking a fief from a vassal works as in the base game, with no lost relations and no revolt.
- `RevokeCrownDecreeAiEnabled` to `false`: AI rulers do not take fiefs by decree of their own accord (your Decree button stays).
- `TitleLordDemandEnabled` to `false`: a duke or count cannot demand a vassal's fief; `TitleLordDemandAiEnabled` to `false`: AI lords never do it of their own accord (your Demand button stays).
