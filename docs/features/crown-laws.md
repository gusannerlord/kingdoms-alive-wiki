# Laws of the crown

Four new laws sit in the game's own **Policies** tab of the kingdom screen, beside the realm's usual laws, and are voted like any other: one that forbids the houses to make war on one another, and three that set what each house pays its lord. Only the ruler may bring them before the council, and the houses weigh every one by their pride and their purse.

## High Crown Authority {#high-crown-authority}

*"The crown alone keeps the peace of the realm."* Without it, the realm lives under **Autonomous Vassals**: its houses may take up arms for their rights.

While High Crown Authority is the law of a realm:

- **No house may take up arms against another**, by any road: no [feud](factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) over a fief, no [feud for a title](titles.md#a-feud-for-a-title), no lord taking up arms against a vassal who bars the gates. A right to land goes before the council in a [reckoning](factions.md#the-reckoning-of-a-house), and only the ruler's decree makes the council's vote good. A title changes hands only when it falls vacant. Your buttons and lines that would start a feud are greyed: *"High Crown Authority is the law of {realm}: no house may take up arms against another."*
- **Every feud ends the day it passes.** Feuds being fought or waiting end with no victor: what was taken in them goes back, the grudge stays, and nobody answers for felony. Feuds still being prepared in silence are given up, and the holder keeps the fief.
- **The houses resent it.** While it lasts, the head of every house of the realm thinks **10** less of the ruler, and each house holds it against the crown as a grievance that does not fade (it weighs more in a great realm). [Charters](factions.md#the-charter) come sooner, and their first demand is always its repeal.
- **A vassal's quarrel goes to the throne.** A lord whose vassal will not yield a fief cannot ride against him: he takes his plea to the ruler (see [A lord's plea](royal-court.md#a-lords-plea)). A council's vote in a reckoning takes no fief by itself: it goes up to the ruler, who backs it by decree or keeps out of it.
- **Not in the Empire.** In a realm of the [Empire](empire.md) a lord who takes up arms against another is already a rebel: the law is greyed there, with that reason.

Plots, charters and reckonings go on under it, and a house may still break with the realm.

## The tax obligation {#the-tax-obligation}

What each house pays its lord, of what its towns and castles yield. There is one at a time, and the realm moves along it **one step at a time**: to raise it from Low you must first pass Normal; repealing the law in force lowers it one step.

| Law | Each house pays its lord | The heads of the houses think of the ruler |
|---|---|---|
| No tax obligation | nothing | **5** better |
| **Low Tax Obligation** | **2.5%** | no differently |
| **Normal Tax Obligation** | **5%** | **2** less |
| **High Tax Obligation** | **10%** | **5** less |

- **Who pays, who gets paid.** The chain of [dukes, counts and castellans](titles.md): a count pays his duke, a duke the crown, and so on. The ruler's own house, sellswords and [landed knights](landed-knights.md) neither pay this share nor count in the regard.
- **Each house votes by its own purse:** what it would collect from its vassals, less what it would pay its lord. A count who pays and collects nothing usually votes against raising it; a duke with many counts beneath him votes for it; the crown gains.
- **Where it binds.** Every realm whose houses hold their land of a lord (dukes and counts, the [themes](titles.md#themes-of-the-empires) of the Empires, the [ulus](titles.md#the-ulus-of-the-khuzaits) of the Khuzaits) begins with the **Low Tax Obligation**, and so does a realm born later (a rebel realm, or your own). Where no house holds its land of a lord, a tax obligation would bind nobody: the laws are greyed there, with that reason.

The two kinds add up: under High Crown Authority and a High Tax Obligation, the heads of the houses think 15 less of the ruler.

## Who brings them before the council

- **Only the ruler** proposes these laws or their repeal, you and an AI ruler alike, at the usual cost of a law. The houses can ask for a repeal (or a lower tax) only through a [charter](factions.md#the-charter), whose head puts it to the council. Only one of these four laws is before the council at a time.
- **The game's own AI never draws these laws** for its proposals: they come only from the ruler's will or a charter.
- **A charter the crown has sealed binds it for a good while**: a law it repealed, a law it passed or a tax it lowered stays as it is. A ruler who undoes it in that time breaks the charter, and the houses that sealed it remember. An AI ruler does not do it; your button stays lit, and its tooltip warns you.

### How an AI ruler weighs them

An AI ruler weighs these laws by his character and his needs, rarely, and never on a whim:

- **High Crown Authority** only an autocrat brings, one who is not a friend of the lords' councils, with no charter, plot or civil war against him and the influence to **overrule the council** (the houses stand against it). Even then, seldom. A ruler who is no autocrat repeals it of his own accord only when he needs his houses' goodwill. An autocrat facing a charter that asks its repeal may overrule that vote too, while he can pay for it: then the charter takes its case to him.
- **He lowers the tax** one step when he is disliked by many of his houses, or faces a charter or a civil war.
- **He raises it** one step when his coffers have been emptying fast.
- Between changes of the tax, he lets a good while pass. As ruler you change it whenever you will.

## The Crown, in the Court tab {#the-crown-screen}

In the kingdom screen's **Court** tab, **The Crown** now also shows:

- **Crown Authority:** the law in force (High Crown Authority or Autonomous Vassals), and **Tax Obligation:** with its share;
- one line for each part of the houses' regard for the crown and its cause, such as *"The houses' regard for the crown: -10 (High Crown Authority)"*;
- a vote already before the council, if any;
- three buttons: **Propose High Crown Authority** (or **Propose to repeal**), **Propose raising taxes** and **Propose lowering taxes**. They open the same vote as the Policies tab, at the same cost, and are greyed with the reason when you cannot: you are not the ruler, another of these laws is before the council, you lack the influence, it is not the next step, and so on.

## Turn it off

In the [settings file](../settings.md), set to `false`:

- `CrownAuthorityEnabled`: High Crown Authority (it stays in the list, greyed, and does nothing);
- `CrownTaxesEnabled`: the tax obligation (every house pays the low share, 2.5%);
- `CrownAiRulerEnabled`: AI rulers weighing these laws of their own accord.
