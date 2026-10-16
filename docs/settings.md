# Settings

Every feature has an on/off switch. You do not need to touch anything: the defaults are what the mod is designed and tested with.

## Where the file is
The first time you start the game with the mod, it creates:

`Documents\Mount and Blade II Bannerlord\Configs\ModSettings\CampaignImprovements.json`

Open it with any text editor (Notepad is fine). It lists every switch as `true` (on) or `false` (off). Changes apply the next time you start the game.

!!! tip "Changing a number"
    The file only holds the switches. Every number (days, chances, prices...) is listed with its default in **CampaignImprovements.all-settings.json**, in the same folder. To change one, copy its line into `CampaignImprovements.json` and edit the value there. Editing `all-settings.json` itself does nothing: it is rewritten at every start, just for reference.

!!! note
    Keep the commas and quotes as they are. If the file gets broken, delete it and the mod writes a fresh one with the defaults.

## Switches

### War and peace
See [War and peace](features/war-and-peace.md).

| Switch | What it does |
|---|---|
| `WarScoringEnabled` | The mod's way of deciding wars. Off = the base game decides. |
| `WarStrengthEnabled` | A kingdom that just lost men is not seen as easy prey. |
| `WarSharedSpoilsEnabled` | A kingdom already at war promises less to one more attacker (less piling on). |
| `WarRulerRelationEnabled` | The relation between rulers counts much more. |
| `WarRelationIgnoresStrength` | That relation counts the same whatever the kingdoms' strengths. |
| `WarGoodRelationCounts` | Good relations count against war as much as bad ones count for it. |
| `WarReconquestEnabled` | Kingdoms want back lost towns and castles of their own culture. |
| `WarOpportunityEnabled` | "The right moment": a kingdom strikes to retake land while its holder is busy elsewhere. |
| `WarOpportunityStrengthCountsTargetEnemies` | That moment also counts who else is already fighting the holder. |
| `WarWearinessEnabled` | Losses make a kingdom want peace. |
| `WarNoCausePenaltyEnabled` | A war with no cause needs clearly better odds. |
| `WarAmbitionEnabled` | Restlessness after a long peace. |
| `DominanceEnabled` | Neighbours fear and gang up on a kingdom grown too large. |
| `DominanceLiftsSharedSpoils` | Piling on a dominant kingdom is not discouraged. |
| `DominanceRemovesSizeDiscount` | A dominant kingdom's lands keep their full value as a war prize (the base game counts a large kingdom's lands at half value). |
| `DominanceCountsDestroyedKingdoms` | Destroyed kingdoms still count when judging who is too large. Turn off for world scenarios that remove kingdoms at the start. |
| `ExpansionResentmentEnabled` | Neighbours grow wary of a kingdom that keeps growing. |
| `TruceEnabled` | 45 days of truce after a peace. |
| `NoWarOnTributePayers` | A kingdom will not attack one that is paying it tribute (for up to 72 days). |
| `PeaceNeedsOtherSideConsent` | Peace needs both sides, unless the war is decided or has lasted 80 days. |
| `DiplomacyRulesApplyToPlayerKingdom` | The truce, tribute and peace rules also bind your own kingdom. |
| `CallerPeaceCoversCalledAllies` | When a kingdom that called an ally makes peace, the ally makes peace too. |
| `CallerStaysWhileAlliesAreBound` | A kingdom that called an ally cannot walk out of that war early. |
| `HeirRelationEnabled` | An heir inherits 10% to 70% of each relation, at random, instead of 70%. |
| `WarSupportExplained` | The kingdom screen explains why your lords back or oppose a war. |
| `WarDeclaredOnPlayerShowsReason` | You are told why a kingdom declared war on yours. |
| `WarDeclaredOnPlayerPausesGame` | That message is a window that pauses the game. Off = a notice on the map. |

### Kingdoms and court

| Switch | What it does | Page |
|---|---|---|
| `RealmEventsEnabled` | Events and tension between kingdoms. | [Events between kingdoms](features/events-between-kingdoms.md) |
| `RealmTensionHoldsDuringTruce` | The tension between two kingdoms does not fade during the truce after their own peace; it starts fading once they could go to war again. | [Events between kingdoms](features/events-between-kingdoms.md) |
| `CouncilPersuasionEnabled` | Talking lords into backing a war or a peace. | [Council](features/council.md) |
| `FeastsEnabled` | Feasts. | [Feasts](features/feasts.md) |
| `GrandTournamentEnabled` | The grand tournament at a ruler's feast. | [Feasts](features/feasts.md) |
| `HallCrowdLimitEnabled` | A crowded lord's hall lets in only as many lords as it has places for; the rest can still be spoken to from the menu. | [Feasts](features/feasts.md) |
| `HuntsEnabled` | Hunts: AI lords call them, invite you, and you can host your own. | [Hunts](features/hunts.md) |
| `HuntForeignInvitesEnabled` | Lords of other kingdoms at peace with yours who like you can invite you to their hunts, and you can invite them to yours. | [Hunts](features/hunts.md) |
| `HuntWindowsEnabled` | Each day you hunt, a window asks you about something that happens out in the woods. | [Hunts](features/hunts.md) |
| `HuntSkillXpEnabled` | Doing well in those windows gives experience in the skill it tested. | [Hunts](features/hunts.md) |
| `HuntAccidentsEnabled` | Once in a long while an AI lord dies in a hunting accident. Never you or anyone of your house. | [Hunts](features/hunts.md) |
| `HuntAccidentsCanKillRulers` | Rulers can die in those accidents too (less often than other lords). | [Hunts](features/hunts.md) |
| `HuntPlotRecruitEnabled` | A hunt is a place for quiet words: talking a lord into or out of a plot, or about a war, a peace or a fief, is easier there, and AI plotters and rulers use their hunts to win lords over. | [Hunts](features/hunts.md) |
| `HuntPlotAccidentEnabled` | You can arrange an "accident" for a lord out hunting with you. | [Hunts](features/hunts.md) |
| `HuntPlotCanTargetRulers` | That accident can be aimed at a ruler too. | [Hunts](features/hunts.md) |
| `HuntingRightsEnabled` | The Hunting Rights policy makes hunts more frequent and friendlier in a kingdom, and harder on the villages they ride over. | [Hunts](features/hunts.md) |
| `ClanEventsEnabled` | Events between clans. | [Events between clans](features/clan-events.md) |
| `VoteRelationsEnabled` | Your council votes, and your decisions as ruler, change relations by the mod's fairer rules. | [Council](features/council.md#relations-from-council-votes) |
| `VoteRelationsAiEnabled` | AI lords' votes change relations between them too. | [Council](features/council.md#relations-from-council-votes) |
| `RealmDiscontentEnabled` | Discontent in kingdoms grown too large. | [Civil war](features/civil-war.md) |
| `ConspiracyEnabled` | Plots and civil wars. | [Civil war](features/civil-war.md) |
| `CivilWarOutsideRestraintEnabled` | Other kingdoms hold back from attacking either side of a civil war. | [Civil war](features/civil-war.md) |
| `CivilWarNotifyPlayer` | A notice in the middle of the screen when any kingdom falls into civil war. | [Civil war](features/civil-war.md) |
| `EnvoysEnabled` | Envoys (all errands). | [Envoys](features/envoys.md) |
| `EnvoyCouncilEnabled`, `EnvoyRecruitEnabled`, `EnvoyMarriageEnabled`, `EnvoyTradeEnabled`, `EnvoySoundEnabled`, `EnvoyMeetingEnabled`, `EnvoyGiftEnabled`, `EnvoyPlotJoinEnabled`, `EnvoyPlotLoyalEnabled` | Each envoy errand on its own. | [Envoys](features/envoys.md) |
| `DuelsEnabled` | Lords may challenge you to a duel. | [Duels](features/duels.md) |
| `AiDuelsEnabled` | AI lords duel each other. | [Duels](features/duels.md) |
| `AiDuelsCanKillRulers` | Rulers can fight (and die) in AI duels. Off by default. | [Duels](features/duels.md) |
| `DuelRulersCanChallengePlayer` | Rulers can challenge you. Off by default. | [Duels](features/duels.md) |

### Your realm and household

| Switch | What it does |
|---|---|
| `RealmAffairsEnabled` | [Affairs of your kingdom](features/realm-affairs.md), brought to you by a messenger on the road. Each affair also has its own switch: `RealmAffairFreeCompany`, `RealmAffairPeasantRevolt`, `RealmAffairFamine`, `RealmAffairClanFeud`, `RealmAffairRealmWorks`. |
| `AffairDelegationEnabled` | The messenger's answers *"One of my companions or kin will see to it."* and, if you rule, *"My vassals will see to it."*: send someone of yours with men you pick, or hand the affair to a house of your realm. Off = you deal with affairs yourself. See [Affairs of your kingdom](features/realm-affairs.md). |
| `CompanionErrandsEnabled` | [Companion errands](features/companion-errands.md). |
| `AwayQuestLogEnabled` | A quest log entry, with the days until they are back, for everyone you send away: on an affair of your kingdom, or a companion on an errand. It closes by itself when they return. |

### The royal court
See [The royal court](features/royal-court.md).

| Switch | What it does |
|---|---|
| `CourtOfficesEnabled` | The four offices of the court (Marshal, Steward, Master of Works, Chancellor) and what they give. |
| `CourtAiAppointEnabled` | AI rulers name their own court and may offer you an office. |
| `CourtChargeEnabled` | When you hold an office for an AI ruler, the affairs of that office come to you as the ruler's charge, with greater rewards. |
| `AudiencesEnabled` | Petitioners come to you with requests, and **Hold court** in your own towns and castles calls them in and hears them, then the notables of the place with tasks for you. |
| `OathEnabled` | When a kingdom gets a new ruler, every house swears to them, asks for something or refuses. |
| `FiefRevocationEnabled` | Proposing to take a fief from a vassal worries your other vassals, and the holder may break away with its fiefs. |
| `FiefPlotEnabled` | As ruler, win lords over to vote for taking a fief from another house. |
| `FiefClaimFourCandidates` | Four candidates when a fief is shared out; right after a conquest, the house that led it always stands. See [Council](features/council.md#who-gets-a-fief). |
| `FiefClaimEnabled` | Ask a lord for their voice for your house when the next fief is shared out. |
| `FiefClaimFriendshipEnabled` | Every lord's vote for your house rises a little with how much they like you. |

### Campaign

| Switch | What it does |
|---|---|
| `FastModeMarriagesEnabled` | More AI marriages in fast mode. See [Fast mode families](features/fast-mode.md). |
| `FastModeChildrenEnabled` | More AI children in fast mode. |
| `ChildCultureEnabled` | A child of two AI characters takes the father's culture 9 times out of 10. |
| `SiegePreparationEnabled` | Siege preparations take twice as long. See [Other changes](features/other-changes.md). |
| `SiegePatienceIgnoresAddedPreparationTime` | The AI besieger is not made impatient by that extra time. |
| `AiPeaceTrainingEnabled` | AI troops train less in long peace. |
| `GearPricesEnabled` | Fairer prices of weapons and armour for the player. |
| `ApplyToWeapons` | Weapons get cheaper too. Off = only armour. |

### Logs
`EventLogEnabled`, `DiplomacyLogEnabled` and `CourtMeasureLogEnabled` write detailed lines to the game's log, useful only when I ask you for a log to track a bug. Off by default.
