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
| `CouncilPersuasionEnabled` | Talking lords into backing a war or a peace. | [Council](features/council.md) |
| `FeastsEnabled` | Feasts. | [Feasts](features/feasts.md) |
| `GrandTournamentEnabled` | The grand tournament at a ruler's feast. | [Feasts](features/feasts.md) |
| `HallCrowdLimitEnabled` | A crowded hall lets in only as many nobles as it has seats. | [Feasts](features/feasts.md) |
| `ClanEventsEnabled` | Events between clans. | [Events between clans](features/clan-events.md) |
| `RealmDiscontentEnabled` | Discontent in kingdoms grown too large. | [Civil war](features/civil-war.md) |
| `ConspiracyEnabled` | Plots and civil wars. | [Civil war](features/civil-war.md) |
| `CivilWarOutsideRestraintEnabled` | Other kingdoms hold back from attacking either side of a civil war. | [Civil war](features/civil-war.md) |
| `EnvoysEnabled` | Envoys (all errands). | [Envoys](features/envoys.md) |
| `EnvoyCouncilEnabled`, `EnvoyRecruitEnabled`, `EnvoyMarriageEnabled`, `EnvoyTradeEnabled`, `EnvoySoundEnabled`, `EnvoyMeetingEnabled`, `EnvoyGiftEnabled`, `EnvoyPlotJoinEnabled`, `EnvoyPlotLoyalEnabled` | Each envoy errand on its own. | [Envoys](features/envoys.md) |
| `DuelsEnabled` | Lords may challenge you to a duel. | [Duels](features/duels.md) |
| `AiDuelsEnabled` | AI lords duel each other. | [Duels](features/duels.md) |
| `AiDuelsCanKillRulers` | Rulers can fight (and die) in AI duels. Off by default. | [Duels](features/duels.md) |
| `DuelRulersCanChallengePlayer` | Rulers can challenge you. Off by default. | [Duels](features/duels.md) |

### Your realm and household

| Switch | What it does |
|---|---|
| `RealmAffairsEnabled` | [Affairs of your kingdom](features/realm-affairs.md). Each affair also has its own switch: `RealmAffairFreeCompany`, `RealmAffairPeasantRevolt`, `RealmAffairFamine`, `RealmAffairClanFeud`, `RealmAffairRealmWorks`. |
| `CompanionErrandsEnabled` | [Companion errands](features/companion-errands.md). |

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
`EventLogEnabled` and `DiplomacyLogEnabled` write detailed lines to the game's log, useful only when I ask you for a log to track a bug. Off by default.
