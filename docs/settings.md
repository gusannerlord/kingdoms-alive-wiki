# Settings

Every feature has an on/off switch. You do not need to touch anything: the defaults are what the mod is designed and tested with.

## In the game's options (Mod Configuration Menu)
If you use [Mod Configuration Menu](https://www.nexusmods.com/mountandblade2bannerlord/mods/612) **5.13 or later**, every switch below (and a few numbers: truce days, peace rules, siege preparations, children's culture) is also under **Options > Mod Options > Kingdoms Alive**, grouped as on this page. MCM is not required: without it, everything works as before through the file.

Changes made there are written to the same settings file and apply the next time you start the game. Settings you put in the file by hand are kept, and the menu shows them.

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
| `SuccessionLawsEnabled` | Each realm follows its own law of succession when its ruler dies. Off: the base game's vote everywhere. | [The crown and its claim](features/succession.md) |
| `RightToRuleEnabled` | Every lord has a claim to the crown, and the ruler's claim has the effects below. | [The crown and its claim](features/succession.md#what-makes-a-claim) |
| `RightToRulePlotsEnabled` | A weak claim breeds plots, even in a kingdom that is not too large. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleOathEnabled` | The new ruler's claim weighs in every house's oath. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleWarEnabled` | The claim weighs in war and peace. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleCouncilEnabled` | The claim weighs in the council's support for the ruler's proposals. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleNotifyPlayer` | A line in your messages whenever a crown passes anywhere in Calradia. | [The crown and its claim](features/succession.md) |
| `FactionsEnabled` | Factions: charters, reckonings, the demand to step down, grievances. Off: the plots and civil wars of before, alone. | [Factions and grievances](features/factions.md) |
| `FactionGrievancesEnabled` | Every house remembers what the crown did to it. | [Factions and grievances](features/factions.md#lords-remember) |
| `FactionCharterEnabled` | The Charter: lords who would bind the ruler's hands. | [Factions and grievances](features/factions.md#the-charter) |
| `FactionReckoningEnabled` | The Reckoning: lords who would bring down an overmighty house. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `FactionAbdicationEnabled` | A strong plot asks the ruler to step down before it rises. | [Factions and grievances](features/factions.md#asking-a-ruler-to-step-down) |
| `FactionConfidantsEnabled` | Friends tell you what is afoot in their realm, and write when it comes to a head. | [Factions and grievances](features/factions.md#you-and-the-factions) |
| `FactionsInAiRealms` | Factions in the AI kingdoms too, not only in yours. | [Factions and grievances](features/factions.md) |
| `FactionAiInternalWarLimit` | Only one civil war at a time among the AI kingdoms, and not too soon after another. | [Factions and grievances](features/factions.md#not-too-many-civil-wars) |
| `FactionFeudsEnabled` | A reckoning the ruler refused may take up arms: a feud between two houses of the realm over the fief. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionStripRebelsEnabled` | A house that loses a fief to a reckoning's vote may refuse it and break with the realm. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `FactionGrievanceRelationsEnabled` | A wrong between two AI houses sours their heads at once. | [Factions and grievances](features/factions.md#lords-remember) |
| `FiefRightsEnabled` | Rights to fiefs: old rights to lost fiefs, rights by blood, by leading the siege, old claims of a line. Off: rights count for nothing. | [Rights to fiefs](features/fief-rights.md) |
| `FiefRightsVotesEnabled` | Rights weigh when a fief is shared out and in a reckoning's vote. | [Rights to fiefs](features/fief-rights.md#in-the-council) |
| `FiefRightsVoicesEnabled` | Win a weak right to a fief with a forged grant its people swear to. | [Rights to fiefs](features/fief-rights.md#a-forged-claim) |
| `FiefRightsForgerEnabled` | The grant must first be forged by a gang leader of the town (of the nearest town for a castle). | [Rights to fiefs](features/fief-rights.md#the-forger) |
| `FiefRightsEnvoyEnabled` | Send an envoy with the forged grant to find witnesses for you. | [Rights to fiefs](features/fief-rights.md#sending-an-envoy) |
| `FiefRightsReckoningNeedsRight` | A reckoning can only be raised over a fief one of its houses has a right to. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `FiefRightsNativeRevokeNeedsRight` | Only the ruler may put any house's fief to the council; a vassal needs a right (their own or their reckoning's). | [Rights to fiefs](features/fief-rights.md#in-the-council) |
| `FiefRightsAncestralEnabled` | Many AI houses start with an old claim to a fief of another house. | [Rights to fiefs](features/fief-rights.md#old-claims-of-a-line) |
| `FiefRightsAiVoicesEnabled` | AI houses forge claims to fiefs they covet; you hear of it when the fief is yours. | [Rights to fiefs](features/fief-rights.md#when-others-court-your-people) |
| `FiefRightsFeudHonourEnabled` | Honourable houses with no ties to either side may stand with the holder in a feud over a weaker right. | [Rights to fiefs](features/fief-rights.md#in-the-council) |
| `FiefRightsEncyclopediaEnabled` | Rights in the encyclopedia pages of houses and fiefs. | [Rights to fiefs](features/fief-rights.md#where-to-see-it) |
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

### Faiths
See [The faiths of Calradia](features/faiths.md).

| Switch | What it does |
|---|---|
| `FaithEnabled` | Every people keeps a faith: priests, festivals, the sacred months, pilgrimages and blessings. Off: none of it. |
| `FaithPriestsEnabled` | A priest of the town's faith in every town, who gives their recruits only to a pillar of their faith. |
| `FaithPietyEnabled` | The lords of your faith think better of you the more devoutly you keep it, the most devout think less of you if you do not, and your towns of your faith hold more loyally to you. |
| `FaithTroopsWageEnabled` | The warriors of the faiths ask far less pay than other soldiers. |
| `FaithTroopsEnabled` | A priest's recruits are his faith's own warriors, a line of three for each faith. |
| `FaithFestivalsEnabled` | Each faith's great festival, once a year in its holy town. |
| `FaithSacredMonthsEnabled` | Every autumn the Aserai realms go to no war and raid nothing, and whoever attacks them then is cursed. |
| `FaithMissionsEnabled` | Priests ask the faithful for help, as the townsfolk do. Each mission has its own switch: `FaithMissionPilgrimsEnabled`, `FaithMissionGrainEnabled`, `FaithMissionRelicEnabled`, `FaithMissionHereticEnabled`, `FaithMissionShrineEnabled`. Off: no new ones are offered; those under way can still be finished. |
| `FaithPilgrimageEnabled` | You can ask a priest of your faith to send you on pilgrimage, to keep a vigil at its holy place. |
| `FaithVirtuesEnabled` | Each faith holds two virtues of character dear; the way you live raises you among its faithful, or lowers you. |
| `FaithDeedsEnabled` | Clearing bandits from the lands of your faith, defending its villages and winning back its holy town raise you among the faithful; executing its lords does not. |
| `FaithBlessingsEnabled` | Festivals and pilgrimages leave a blessing on your company: morale, march or healing. |
| `FaithConversionEnabled` | You can take up another faith with one of its priests. |
| `FaithRelationsEnabled` | Lords of the same faith quarrel less, and marry across faiths less often. |

### The faith and ways of a fief
See [The faith and ways of a fief](features/faith-and-ways.md).

| Switch | What it does |
|---|---|
| `FiefWaysEnabled` | A town or castle slowly takes up the faith and the culture of its realm; until then its people are restless. Off: nothing more changes (fiefs already changed stay so). |
| `FiefWaysTempleEnabled` | Who takes a town of another faith by siege decides what becomes of its temple. |
| `FiefWaysOldPriestEnabled` | The old faith's priest can be left in peace, banished or won over. |
| `FiefWaysMissionsEnabled` | A priest of the realm's faith, paid, sends preachers to a fief. |
| `FiefWaysAlmsEnabled` | Alms for the people of a fief in hard times. |
| `FiefWaysOldLawsEnabled` | A fief's old laws, granted and revoked through its governor. |
| `FiefWaysUnrestEnabled` | Now and then trouble in a fief of another faith or culture. |
| `FiefWaysRebellionEnabled` | A town of another faith and culture rises sooner. |
| `FiefWaysLogEnabled` | Lines `Ways:` in the log (with the diplomacy log on). |

### The Marshal and the realm's command
See [Command your armies](features/command-your-armies.md).

| Switch | What it does |
|---|---|
| `PrudenceRealmEnabled` | The whole realm's command: orders as ruler or as Marshal, orders to one army, riders, and your liege's words. Off = none of it. |
| `PrudenceOfficeEnabled` | The Marshal leads the realm's armies: you give orders through your Marshal, or take your liege's as Marshal. Off = no orders, no orders to one army and no riders. |
| `PrudenceArmyOrdersEnabled` | Order one army of the realm to besiege a place, stand guard over one of yours, or come home. |
| `PrudenceRiderEnabled` | Send riders with your word from any town or castle of your realm (needed for riders from your party too). |
| `PrudenceFieldRiderEnabled` | A companion or family member riding with you finds you a rider, wherever you are. |
| `PrudenceMarshalEnabled` | Your liege tells you how the war goes, and the leader of the army you ride in tells you why it acts. |

### Your realm and household

| Switch | What it does |
|---|---|
| `RealmAffairsEnabled` | [Affairs of your kingdom](features/realm-affairs.md), brought to you by a messenger on the road. Each affair also has its own switch: `RealmAffairFreeCompany`, `RealmAffairPeasantRevolt`, `RealmAffairFamine`, `RealmAffairClanFeud`, `RealmAffairRealmWorks`, `RealmAffairEnemies` (the enemies of the crown, for vassals; see [The Blackhand's knives](features/lords-enemies.md)). |
| `RealmRescueRuler` | While you are a vassal, the ruler's house asks you to free the ruler when they are taken and held in an enemy town or castle. No blame of any kind. See [The crown in chains](features/realm-affairs.md#the-crown-in-chains). |
| `RealmAffairQuestLogEnabled` | Each affair of your kingdom has its own quest log entry for as long as it lasts, with its places and rebel bands marked on the map. |
| `AffairDelegationEnabled` | The messenger's answers *"One of my companions or kin will see to it."* and, if you rule, *"My vassals will see to it."*: send someone of yours with men you pick, or hand the affair to a house of your realm. Off = you deal with affairs yourself. See [Affairs of your kingdom](features/realm-affairs.md). |
| `CompanionErrandsEnabled` | [Companion errands](features/companion-errands.md). |
| `AwayQuestLogEnabled` | A quest log entry, with the days until they are back, for everyone you send away: on an affair of your kingdom, or a companion on an errand. It closes by itself when they return. |
| `TaskQuestLogEnabled` | A quest log entry, with its places marked on the map, for the mod's other tasks: feasts and hunts you are bound to, envoys and meetings, council promises, plots and civil war, petitions, promised fiefs, the oath to a new ruler, a vassal's call for help and your overlord's wars, and the like. |

### Mercenary contracts and the Unsworn
See [Mercenary contracts](features/mercenary-contracts.md).

| Switch | What it does |
|---|---|
| `MercContractsEnabled` | While you serve a realm as a mercenary, its ruler sends you tasks by messenger and summons you to the realm's armies. Off = none of that, and none of the company's career below; a task under way ends as usual. |
| `MercContractRaid` | The task of raiding an enemy village (the game's own "Raid an Enemy Territory" quest). |
| `MercContractProtect` | The tasks of escorting a caravan of the realm and guarding a border village. |
| `MercContractCapture` | The task of taking a lord of an enemy realm captive and handing them over to the crown. |
| `MercContractRescue` | The task of freeing a lord of the realm from an enemy town's dungeon. |
| `MercContractRescueRuler` | When the ruler is held in an enemy town, their house asks you to bring them home. Off = no task while the ruler is a prisoner. |
| `MercContractArmy` | When a lord of the realm raises an army, the ruler may summon your company to ride in it, for pay. |
| `MercContractUnswornHideout` | The task of clearing a hideout of the Unsworn. Only offered to a mercenary when the King's Writ contracts are off (`WritEnabled` or `WritContractsEnabled`); otherwise it is a contract of the writ. |
| `MercContractUnswornSweep` | The task of beating three bands of the Unsworn that roam the realm's villages. The same rule as above. |
| `MercInfluencePayEnabled` | The game's own mercenary pay: the influence you earn is paid in silver. Off = no silver for influence while you serve as a mercenary; your pay is the contract's advance, the tasks and the armies. AI mercenaries are not affected. |
| `MercCareerEnabled` | The company's career: a record of service with every crown, your company's name, and the switches below. Off = only the tasks and summons. |
| `MercFamePayEnabled` | Your company's name raises its pay. |
| `MercTermsEnabled` | Contracts of 30, 60 or 100 days with an advance. Off = you serve and leave as in the base game, with no leave in peacetime, offers from other rulers or enemy purse on the road. |
| `MercPeaceReleaseEnabled` | When the realm has been at peace for a week, its ruler sends word that you may go with the crown's thanks. |
| `MercBidsEnabled` | Rulers at war send for a company with a name. |
| `MercGearRewardsEnabled` | Serve one crown long enough and its ruler gives you the harness of a noble warrior of the realm, in person. |
| `MercTurncoatEnabled` | An enemy ruler's messenger may offer a renowned company a purse to change sides. |
| `MercSiegeBribeEnabled` | At a siege, the defenders may try to buy your company the night before the assault. |
| `MercTurncoatBloodFeud` | Changing sides brings a blood feud with the betrayed ruler's house (not on game version 1.4.8). |
| `UnswornTroopsEnabled` | Taverns sometimes offer Unsworn sellswords for hire. Off = they are no longer offered, and there are no Unsworn tasks or contracts. |
| `FixMercHideoutMenEnabled` | The hideouts of the Unsworn and of your rival hold 35 to 40 men. Off = only as many as the game's own hideouts. |

### The King's Writ
See [The King's Writ](features/kings-writ.md).

| Switch | What it does |
|---|---|
| `WritEnabled` | The whole feature: a free hunter can ask a ruler for their writ. Off = no writ can be asked for, and one you carry is laid aside quietly (what the crown owes you is paid). |
| `WritRewardsEnabled` | The crown pays for outlaw bands, dens and prisoners in its lands, collected from the sheriff. |
| `WritNativeQuestBonusEnabled` | The game's own outlaw quests done in the king's lands bring a bonus from the crown. |
| `WritOutsideNoticeEnabled` | A word when a fight that would have paid was out of the king's lands. |
| `WritSheriffEnabled` | A king's sheriff, a notable you talk to, in every town: he pays you, takes your prisoners and keeps the manhunters' yard. Off = no new sheriffs; a "Sheriff's House" in the town menu does their work. |
| `WritSheriffNativeCompensation` | The sheriff takes no place from the town's own merchants, artisans and gang leaders. |
| `WritContractsEnabled` | The king's contracts: the Unsworn's den and bands, deserters after a peace, a prisoner taken to trial, a raid in a town. Off = the two Unsworn tasks go back to the mercenary contracts. |
| `WritCastleBuildingsEnabled` | The Hunters' Lodge, Gaol Tower and Watchtower of the Master's castle. |
| `WritHordeEnabled` | The outlaws' host that comes for the Master's castle. |
| `WritRaidEnabled` | The raid on a gang hiding inside one of the realm's towns, fought in its streets. |
| `WritRaidTownsfolkEnabled` | Townsfolk walk the raid's streets and run when the fight starts. Off = the curfew bell rings and the streets are empty. |
| `WritWantedEnabled` | Outlaw chiefs with a name and a price, who grow and raid while nobody hunts them. |
| `WritTrialEnabled` | A captured chief is judged in the lord's hall before the king's justiciar. Off = the verdict comes in a window. |
| `WritGallowsEnabled` | A chief sentenced to the rope may draw his gang to the town: walk him to the gallows yourself, and ride after them if they carry him off. |
| `WritFameEnabled` | Fame among the outlaws: small bands keep away, and weaker ones may yield in the king's name. |
| `WritAssassinsEnabled` | With great fame, the outlaws put a price on your head and send hired blades. |
| `WritBribesEnabled` | With fame, a wanted chief may try to buy you off. |
| `WritCompanyRulesEnabled` | Every soldier in your company must be a sworn manhunter, or the crown pays nothing (not for the Master of the King's Hunt). Off = anyone may ride with you. |
| `WritCompanyLimitEnabled` | Off by default. On = the writ also limits the size of your company by rank, with a bar in the journal (`WritCompanyBarEnabled`). |
| `WritBandVanillaScaling` | The writ's bands and dens are sized the way the game sizes the outlaws of its own quests: small early in a campaign, bigger later. Off = they are sized against the strength of your company. |
| `WritRanksEnabled` | The ranks of the writ: King's Hunter, Hunter of the March, High Justice of the Roads, with more pay and rights. |
| `WritRankBarEnabled` | A bar in the writ's journal entry shows your progress toward the next rank (the king's summons has its own bars, `WritSummonsBarsEnabled`). |
| `WritSummonsBarsEnabled` | The writ's journal entry shows bars for what the king wants before he sends for you: his trust, the days in his service, contracts, named chiefs and dens. |
| `WritTroopsEnabled` | The manhunters' troop tree (mounted, on foot and crossbow), hired from the sheriff or freed from the outlaws. |
| `WritWageAsRegular` | Manhunters cost the wages of regular soldiers of their tier. Off = they cost what hired swords cost. |
| `WritGearGiftsEnabled` | The sheriffs' master-at-arms gives you a manhunter's kit with the writ, and better ones as your work for the crown adds up. |
| `WritArmouryEnabled` | The crown's armoury: every piece of the manhunters' gear for sale at any sheriff of the realm. |
| `WritArmouryWeapons` | The armoury sells their weapons and shields too. Off = armour only. |
| `WritOutlawKingEnabled` | After four chiefs taken in a realm, its outlaws crown a king of their own. |
| `WritVassalOfferEnabled` | At the end of a long service, the ruler sends for you and offers a castle, vassalage and the title of Master of the King's Hunt. |
| `WritCaptainsEnabled` | Companions and kin leading your clan's parties can hunt as your captains: one from High Justice of the Roads, up to three as Master of the King's Hunt. |

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
| `CompanySeaPassageEnabled` | With War Sails, a company takes ship to reach you across the sea (you pay the passage). |

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
| `SquireHorses` | The game's own "Lord Needs Horses" quest, given by your lord when their men lack mounts. |
| `SquireTraining` | The errand of facing a garrison's men one after another in a castle yard or a town arena. |
| `SquireDrillVeterans` | The men of that drill fight as veterans, each better than the last, the sergeant hardest. Off = as well as the game would make them. |
| `SquireDrillInView` | The men of that drill wait in a row by the wall in plain sight, the sergeant last. Off = each steps in when called. |
| `SquireHideout` | The errand of clearing a bandit hideout near your lord's lands. |
| `SquirePatrol` | The errand of walking the rounds with the watch of a town, where Skolderbroda lie in wait. |
| `SquirePatrolCastles` | Off by default. On = those rounds can also be walked in castles. |
| `SquireEnemies` | The errand of stopping Blackhand killers paid by your lord's enemies. See [The Blackhand's knives](features/lords-enemies.md). |
| `EnemiesHall`, `EnemiesAlley`, `EnemiesChampion`, `EnemiesVillage`, `EnemiesTavern` | Each of the five ways of the Blackhand's jobs (the hall, the lanes, the arena, the village, the tavern), for your lord's errand and for the enemies of the crown alike. |
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
| `SquireFireEnabled` | Talks with your lord by the fire, in their host, every few evenings. |
| `SquireJudgeEnabled` | After a battle at their side your lord tells you how you fought, and calls on you to stand over them when they fall. |
| `SquireBannerEnabled` | Now and then your lord gives you their colours to carry in a field battle. |
| `SquireYardEnabled` | Practice bouts with your lord (or one of their house) when you are both in a castle. |
| `SquireYardInTowns` | The same on the sand of a town's arena. |
| `SquireYardPeaceOnly` | Bouts only in peacetime. Off = bouts by chance in wartime too (invitations are always peace-only). |
| `SquireYardArrivalNotice` | The word that your lord is in the castle or town also comes as a big notice with their portrait. |
| `SquireYardInvites` | In peacetime your lord sends for you to come for a bout, and waits for you. |

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
| `CourtOfficesEnabled` | The five offices of the court (Marshal, Steward, Master of Works, Chancellor, Warden of the King's Peace) and what they give. |
| `CourtAiAppointEnabled` | AI rulers name their own court and may offer you an office. |
| `CourtChargeEnabled` | When you hold an office for an AI ruler, the affairs of that office come to you as the ruler's charge, with greater rewards. |
| `AudiencesEnabled` | Petitioners come to you with requests, and **Hold court** in your own towns and castles calls them in and hears them, then the notables of the place with tasks for you. |
| `OathEnabled` | When a kingdom gets a new ruler, every house swears to them, asks for something or refuses. |
| `FiefRevocationEnabled` | Proposing to take a fief from a vassal worries your other vassals, and the holder may break away with its fiefs. |
| `FiefPlotEnabled` | As ruler, win lords over to vote for taking a fief from another house. |
| `FiefClaimFourCandidates` | Four candidates when a fief is shared out; right after a conquest, the house that led it always stands. See [Council](features/council.md#who-gets-a-fief). |
| `FiefClaimEnabled` | Ask a lord for their voice for your house when the next fief is shared out. |
| `FiefClaimFriendshipEnabled` | Every lord's vote for your house rises a little with how much they like you. |

### Smarter warlords (off by default)
See [Smarter warlords](features/command-your-armies.md#smarter-warlords-off-by-default). The pieces below do nothing while `PrudenceEnabled` is off.

| Switch | What it does |
|---|---|
| `PrudenceEnabled` | AI lords and armies see as you do and wage war more wisely. **Off by default** = the AI decides as in the base game. |
| `PrudenceNoticesEnabled` | A line on screen when a siege is lifted for fear of a relief and your realm is on either side. |
| `PrudenceSiegeRetreatEnabled` | A besieger lifts a siege it sees lost. Off = the next three do nothing either. |
| `PrudenceWithdrawEnabled` | A siege camp losing a battle at the walls breaks off and leaves. |
| `PrudenceStartSeenEnabled` | No siege begun where the danger already in sight would lift it at once. |
| `PrudenceRememberDefendersEnabled` | A lord remembers an enemy lord seen riding into the place he means to besiege. |
| `PrudenceRefugeEnabled` | A lord fleeing a stronger host takes refuge in the nearest friendly fortress. Off = the next two do nothing either. |
| `PrudenceEarlyWarningEnabled` | He sees a stronger host coming from as far as he can see, and stays inside while it is in sight. |
| `PrudenceWaitOutThreatEnabled` | After taking refuge, he lays no siege the host he fled could reach until it is far, weaker or gone. |
| `PrudenceHuntEnabled` | An AI army rides at an enemy army it sees and can beat and catch. |
| `PrudenceHuntPlayerArmy` | Your army is prey too, if you lead one. |
| `PrudenceHuntGatheringEnabled` | Armies still gathering are prey. |
| `PrudenceHuntBesiegersEnabled` | Armies besieging a third realm are prey. |
| `PrudenceReliefWaitEnabled` | A relief gathers a few hours from the besiegers' camp until it is strong enough (game version 1.5.5 only). |
| `PrudenceRallyEnabled` | An AI army too weak for its siege or relief calls more lords. |

### Running from you (on by default)
See [Running from you](features/command-your-armies.md#running-from-you-on-by-default). These work whether `PrudenceEnabled` is on or off.

| Switch | What it does |
|---|---|
| `FleeRouteEnabled` | A party running from you that is no faster than you, or any bandit party, takes the open way that leaves it farthest from you instead of turning about in a dead end. |
| `FleeRefugeEnabled` | A party running from you makes for a place it reaches before you: bandits a hideout of their own kind, villagers their village, others a town or castle not at war with them. |

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
`EventLogEnabled`, `DiplomacyLogEnabled`, `CourtMeasureLogEnabled`, `RivalLogEnabled`, `MercContractLogEnabled`, `SquireLogEnabled`, `NobleMemoryLogEnabled`, `CaptiveLogEnabled`, `StoryLogEnabled`, `FixRealmLogEnabled`, `CompanyLogEnabled`, `PrudenceLogEnabled` (AI armies, the realm's Marshals and their orders) and `FaithLogEnabled` (faiths) write detailed lines to the game's log, useful only when I ask you for a log to track a bug. Off by default.
