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

### Vassal realms and annexation
See [Vassal realms](features/vassal-realms.md).

| Switch | What it does |
|---|---|
| `VassalageEnabled` | The whole feature. Off = it sleeps: nothing new happens, and realms that were already vassals are left as they are until you turn it back on. |
| `VassalRealmsEnabled` | New vassal realms can be made. Off = no new ones; those that exist carry on. |
| `VassalAiDemandsEnabled` | An AI kingdom that is clearly winning a war can ask fealty as the price of peace. |
| `VassalFearOffersEnabled` | A small, beaten and surrounded AI kingdom can offer fealty to its enemy for peace. |
| `VassalLoyaltyEnabled` | A vassal realm's loyalty moves day by day. Off = it stays where it is. |
| `VassalRebellionEnabled` | An AI vassal realm rebels when its loyalty stays low. |
| `VassalFiefReturnEnabled` | A fief a vassal realm lost and its overlord retakes is given back to it (if you are the overlord, you are asked). |
| `VassalAnnexOnDeathEnabled` | When a vassal realm's ruler dies, the overlord's ruler stands in the vote for its crown. |
| `VassalAnnexLoyalEnabled` | After 90 days with loyalty at 70 or more, a vassal realm can be joined to its overlord's for good. |
| `VassalAnnexForceEnabled` | AI overlords can demand annexation, at the risk of war. You can always demand it. |
| `VassalAnnexMarriageEnabled` | A marriage between the two royal houses strengthens the overlord's claim to the vassal's crown. |
| `VassalDominanceHalfEnabled` | A vassal realm's towns and castles count half for its overlord when neighbours judge who is too large. Off = they count whole. |

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
| `DuelsEnabled` | Duels between AI lords, and the challenges from houses that hate you (if those are on). Your rival's duel has its own switch. | [Duels](features/duels.md) |
| `DuelPlayerChallengesEnabled` | Houses that hate you challenge you to a duel on their own. **Off by default**: only your rival challenges you. | [Duels](features/duels.md) |
| `AiDuelsEnabled` | AI lords duel each other. | [Duels](features/duels.md) |
| `AiDuelsCanKillRulers` | Rulers can fight (and die) in AI duels. Off by default. | [Duels](features/duels.md) |
| `DuelRulersCanChallengePlayer` | Rulers can challenge you. Off by default. | [Duels](features/duels.md) |
| `DuelQuestLogEnabled` | A duel you agreed to has its quest log entry naming the arena town, and moves to another arena if its town turns hostile instead of being called off. | [Duels](features/duels.md) |
| `RivalsEnabled` | A lord may swear a blood feud against you and become your rival. | [Your rival](features/rival.md) |
| `RivalHideoutEnabled` | Your rival can set up a hideout of hired blades marked on the map. | [Your rival](features/rival.md) |
| `RivalBountyEnabled` | Your rival can send bands of hired blades after you, and a larger company after them. | [Your rival](features/rival.md) |
| `RivalTownAmbushEnabled` | Your rival's thugs can ambush you in a town's streets. | [Your rival](features/rival.md) |
| `RivalDuelEnabled` | The rivalry ends in a duel to the death in the arena. | [Your rival](features/rival.md) |
| `RivalSmearEnabled` | Your rival can speak against you to the ruler of their realm (-3 relation, once). | [Your rival](features/rival.md) |

### Your realm and household

| Switch | What it does |
|---|---|
| `RealmAffairsEnabled` | [Affairs of your kingdom](features/realm-affairs.md), brought to you by a messenger on the road. Each affair also has its own switch: `RealmAffairFreeCompany`, `RealmAffairPeasantRevolt`, `RealmAffairFamine`, `RealmAffairClanFeud`, `RealmAffairRealmWorks`. |
| `RealmAffairQuestLogEnabled` | Each affair of your kingdom has its own quest log entry for as long as it lasts, with its places and rebel bands marked on the map. |
| `AffairDelegationEnabled` | The messenger's answers *"One of my companions or kin will see to it."* and, if you rule, *"My vassals will see to it."*: send someone of yours with men you pick, or hand the affair to a house of your realm. Off = you deal with affairs yourself. See [Affairs of your kingdom](features/realm-affairs.md). |
| `CompanionErrandsEnabled` | [Companion errands](features/companion-errands.md). |
| `AwayQuestLogEnabled` | A quest log entry, with the days until they are back, for everyone you send away: on an affair of your kingdom, or a companion on an errand. It closes by itself when they return. |
| `TaskQuestLogEnabled` | A quest log entry, with its places marked on the map, for the mod's other tasks: feasts and hunts you are bound to, envoys and meetings, council promises, plots and civil war, petitions, promised fiefs, the oath to a new ruler, a vassal's call for help and your overlord's wars, and the like. |

### Mercenary contracts and the Unsworn
See [Mercenary contracts](features/mercenary-contracts.md).

| Switch | What it does |
|---|---|
| `MercContractsEnabled` | While you serve a realm as a mercenary, its ruler sends you tasks by messenger. Off = no new tasks and no "In the service of the crown" quest; one under way ends as usual. |
| `MercContractRaid` | The task of raiding enemy villages (the game's own "Raid an Enemy Territory" quest). |
| `MercContractProtect` | The tasks of escorting a caravan of the realm and guarding a border village. |
| `MercContractUnswornHideout` | The task of clearing a hideout of the Unsworn. |
| `MercContractUnswornSweep` | The task of beating three bands of the Unsworn that roam the realm's villages. |
| `MercContractRescue` | The task of freeing a lord of the realm from an enemy town's dungeon. |
| `MercContractRescueRuler` | When the ruler is held in an enemy town, their house asks you to bring them home. Off = no task while the ruler is a prisoner. |
| `MercContractVassalPath` | After 5 tasks fulfilled, with your clan at tier 2 or more, the ruler offers you vassalage, and maybe a castle. |
| `UnswornTroopsEnabled` | Taverns sometimes offer Unsworn sellswords for hire. Off = they are no longer offered, and there are no Unsworn tasks. |
| `FixMercHideoutMenEnabled` | The hideouts of the Unsworn and of your rival hold 35 to 40 men. Off = only as many as the game's own hideouts. |

### Companies for hire
See [Companies for hire](features/free-companies.md).

| Switch | What it does |
|---|---|
| `CompanyHireEnabled` | The four sellsword companies can be hired. Off = nobody hires them any more; a contract under way runs to its end. |
| `CompanyAiHireEnabled` | AI lords hard pressed in a war can hire them too. |
| `CompanyCourierEnabled` | You can send a rider from a tavern to hire a company without going to its town. |
| `CompanyBloodMoneyEnabled` | At the end of a contract you pay blood money for each of their men who died. |
| `CompanyRelocateEnabled` | Companies move to another town every couple of months, drawn to the wars. |
| `CompanyRemounts` | A company brings spare horses that keep your party from slowing to a crawl. |

### Squire service
See [Squire service](features/squire.md).

| Switch | What it does |
|---|---|
| `SquireEnabled` | Lords take you as their squire. Off = no new service; one under way ends within the hour, without blame. |
| `SquireTournament` | The errand of fighting in a tournament for your lord's house (or losing the final on purpose, for a lord without honour). |
| `SquireLetter` | The errand of carrying a letter (or a threat) to another lord. |
| `SquireFeast` | The errand of attending a feast of the realm in your lord's name. |
| `SquireBand` | The errand of destroying a company of sellswords sent against your lord's lands. |
| `SquireTaxes` | The game's own "Revenue Farming" quest, given by your lord. |
| `SquireGarrison` | The game's own "Lord Needs Garrison Troops" quest, given by your lord. |
| `SquireTraining` | The errand of drilling a day with your lord's men at one of their fortresses. |
| `SquireHideout` | The errand of clearing a bandit hideout near your lord's lands. |
| `SquireArmyCall` | You are called to every army your lord raises or joins. |
| `SquireRescue` | Your lord's house asks you to free them when they are captured. |
| `SquireBattleSide` | In battle your lord is outlined in gold, and you start at their side. |
| `SquireStayOn` | When your lord sends for you after your errands, you may stay on as their squire instead of kneeling for your spurs. |
| `SquireMarkLord` | Your lord carries the game's map arrow while you serve. |
| `SquireMarchCall` | Word when your lord's own party rides out to raid or besiege. |
| `SquireMarchDefend` | The same when they ride out to relieve a place of their realm. |
| `SquireMarchPatrol` | The same when they take their ships to harry an enemy coast (War Sails). |
| `SquireBattleAlarm` | A quick notice when your lord goes into battle without you. |
| `SquireArmyLearn` | Riding in the same army as your lord, you learn a little of their best skills each day. |

### Lords who remember you, captives and companions with a story

| Switch | What it does | Page |
|---|---|---|
| `NobleMemoryEnabled` | Lords remember what you did to them and theirs, and bring it up when you talk. | [Lords who remember you](features/memories.md) |
| `CaptiveDealsEnabled` | When you take a lord prisoner, their house may act (bargains, sellswords, knives in the streets). | [Captives](features/captives.md) |
| `CaptiveDealOffer` | The "name your price" bargains, from the house's messenger or from the captive. | [Captives](features/captives.md) |
| `CaptiveMarriageOffer` | A marriage into their house can be among the offers. | [Captives](features/captives.md) |
| `CaptiveCaravanTip` | Word of a rich caravan can be among the offers. | [Captives](features/captives.md) |
| `CaptiveRescueParty` | The house can hire sellswords to hunt your party and free the captive. | [Captives](features/captives.md) |
| `CaptiveTownThugs` | The house can send cut-throats to the town where you keep the captive. | [Captives](features/captives.md) |
| `CaptiveTalksEnabled` | Noble prisoners in your party speak to you, and how you keep them matters. | [Captives](features/captives.md) |
| `CaptiveTalkNews` | You can ask captives about their realm. | [Captives](features/captives.md) |
| `CaptiveGrudges` | Captives leave grateful or bitter, and a bitter one can become your rival. | [Captives](features/captives.md) |
| `CaptiveTalkWorldNews` | Captives speak of what happened to their kin, house and realm since they last spoke. | [Captives](features/captives.md) |
| `CaptiveTalkRansom` | A well-treated captive can name their own ransom. | [Captives](features/captives.md) |
| `CaptiveTalkParole` | You can free a well-treated captive on their word not to fight you again in this war. | [Captives](features/captives.md) |
| `StoryCompanionsEnabled` | Companions with a story of their own can appear. | [Alayen](features/alayen.md) |
| `AlayenEnabled` | Alayen can appear. | [Alayen](features/alayen.md) |
| `AlayenQuestEnabled` | His quest, "The Grey Wolf". | [Alayen](features/alayen.md) |
| `AlayenErrandsEnabled` | His requests for leave and men to settle matters of his own. | [Alayen](features/alayen.md) |

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
| `AiPeaceTrainingEnabled` | Once their kingdom has been at peace for 10 days, AI troops get only a quarter of their free daily training. |
| `GearPricesEnabled` | Fairer prices of weapons and armour for the player. |
| `ApplyToWeapons` | Weapons get cheaper too. Off = only armour. |

### Logs
`EventLogEnabled`, `DiplomacyLogEnabled`, `CourtMeasureLogEnabled`, `RivalLogEnabled`, `MercContractLogEnabled`, `SquireLogEnabled`, `NobleMemoryLogEnabled`, `CaptiveLogEnabled`, `StoryLogEnabled`, `FixRealmLogEnabled` and `CompanyLogEnabled` write detailed lines to the game's log, useful only when I ask you for a log to track a bug. Off by default.
