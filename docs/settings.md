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
| `WarSpoilsWeight` (a number, 0.7) | How much what a kingdom simply stands to win counts when it weighs a new war (1 = base game). Wars under way, peace and allies joining a war are not affected. |
| `WarSharedSpoilsEnabled` | A kingdom already at war promises less to one more attacker (less piling on). |
| `WarRulerRelationEnabled` | The relation between rulers counts much more; friendship holds a war back more than hatred pushes one. Numbers you can change: `WarRelationWeight` (10) and `WarRelationMaxPoints` (150000) for a good relation, `WarHateWeight` (6) and `WarHateMaxPoints` (100000) for a bad one (a war needs roughly 230,000 to 370,000). |
| `WarRelationIgnoresStrength` | That relation counts the same whatever the kingdoms' strengths. |
| `WarGoodRelationCounts` | Good relations count against war as much as bad ones count for it. |
| `WarReconquestEnabled` | Kingdoms want back lost towns and castles of their own culture. |
| `WarOpportunityEnabled` | "The right moment": a kingdom strikes to retake land while its holder is busy elsewhere. |
| `WarOpportunityStrengthCountsTargetEnemies` | That moment also counts who else is already fighting the holder. |
| `WarWearinessEnabled` | Losses make a kingdom want peace. |
| `WarNoCausePenaltyEnabled` | A war with no cause needs clearly better odds. |
| `WarAmbitionEnabled` | Restlessness after a long peace. |
| `WarDuringFeudPenaltyEnabled` | A kingdom with feuds running between its houses is slower to declare a new war, the more so the greater the share of its strength caught up in them (the AI and your council alike). Numbers you can change: `WarDuringFeudMaxPoints` (450000, taken off the wish for war when the whole realm is at feud), `WarDuringFeudMinPoints` (150000 more while a feud is fought in arms). |
| `WarWaitsForFeudsEnabled` | While a kingdom has a feud fought or waiting, the restlessness of a long peace does not push it to war; once the last feud is over, it counts again at the level the days of peace give. |
| `NegotiatedPeaceEnabled`, `NegotiatedPeaceAiEnabled` | Terms of peace on the Terms of Peace screen, from the Diplomacy tab (for influence, AI kingdoms too) or in person (free): tribute, towns and castles, fealty, voted at once by the council of the realm that gives most, house by house, your own council included; AI kingdoms clearly losing offer terms, clearly winning ones demand them. Numbers you can change: `NegotiatedPeaceInfluenceCost` (200, what Negotiate terms costs, and what an AI kingdom pays to put terms), `NegotiatedVassalVoteDays` (3, how long your council waits for your vote when you are not its ruler), `NegotiatedPeaceMinWarDays` (40), `NegotiatedFiefMinGap` (150), `NegotiatedFiefMinNetTaken` (1), `NegotiatedMaxFiefs` (2), `NegotiatedKeepFiefs` (2), `NegotiatedPairCooldownDays` (15), `NegotiatedTributeDays` (100), `NegotiatedTributeWeight` (1), `NegotiatedTributeTrust` (0.5), `NegotiatedFiefWeight` (1), `NegotiatedVassalWeight` (1), `NegotiatedOwnerGrievance` (30), `NegotiatedFiefDeepWeight` (0.5), `NegotiatedFiefCultureWeight` (0.25), `NegotiatedFiefTownWeight` (0.25), `NegotiatedFiefSeatWeight` (0.5), `NegotiatedFiefCutWeight` (0.75), `NegotiatedDemandStrengthRatio` (1.5), `NegotiatedAiCedeCastleShare` (0.25), `NegotiatedAiCedeCastleMinNet` (2), `NegotiatedAiCedeTownShare` (0.4), `NegotiatedAiCedeTownMinNet` (3), `NegotiatedAiMaxTownsPerPeace` (1); how the houses of a council weigh terms: `NegotiatedCouncilLandWeight` (600, land lost), `NegotiatedCouncilGainWeight` (400, land won), `NegotiatedCouncilKneelShare` (0.3), `NegotiatedCouncilVassalShare` (0.15), `NegotiatedCouncilKinWeight` (0.5), `NegotiatedCouncilNeighbourWeight` (0.5), `NegotiatedCouncilNeighbourDistance` (60), `NegotiatedCouncilCandidateWeight` (0.5), `NegotiatedCouncilDangerWeight` (250, how much the course of the war sways them), `NegotiatedCouncilTwoWarsDanger` (0.1), `NegotiatedCouncilRealmDanger` (0.25), `NegotiatedCouncilSiegeDanger` (0.3), `NegotiatedCouncilFrontDanger` (0.1). `NegotiatedPeaceMinWarDays` binds only the AI's own terms. See [War and peace](features/war-and-peace.md#terms-of-peace). |
| `WarAfterLongPeaceEnabled` | After a long peace, abroad and within, the ruler of an AI kingdom puts the war he would most gladly fight to his council when it is worth it. Numbers you can change: `WarAfterLongPeaceDays` (50), `WarAfterLongPeaceCouncilAt` (0.5, how strongly the council must lean towards the war before he puts it). |
| `DominanceEnabled` | Neighbours fear and gang up on a kingdom grown too large. |
| `DominanceLiftsSharedSpoils` | Piling on a dominant kingdom is not discouraged. |
| `DominanceRemovesSizeDiscount` | A dominant kingdom's lands keep their full value as a war prize (the base game counts a large kingdom's lands at half value). |
| `DominanceCountsDestroyedKingdoms` | Destroyed kingdoms still count when judging who is too large. Turn off for world scenarios that remove kingdoms at the start. |
| `ExpansionResentmentEnabled` | Neighbours grow wary of a kingdom that keeps growing. |
| `WarHolyCityEnabled` | A kingdom wants back the holy city of its ruler's faith from a kingdom of another faith, more than a town of its faith or of its duchies. Needs the faiths. |
| `WarFaithLandEnabled` | A kingdom wants the towns and castles whose people keep its ruler's faith from a kingdom whose ruler keeps another. Needs the faiths. |
| `WarRulersFaithEnabled` | Rulers of different faiths are a little readier for war with each other, rulers of one faith a little slower to it. Needs the faiths. |
| `WarTitlesEnabled` | A kingdom of dukes and counts wants back the towns of its duchies and the castles of its counties it lost to another kingdom. Needs the titles. |
| `WarTitleVotesEnabled` | In the vote on a war, dukes and counts whose lands border the enemy, or lost a place to it, are for the war more; those far from it a little less. Needs the titles. |
| `TruceEnabled` | 45 days of truce after a peace (`TruceDaysAfterPeace`, 45). |
| `WarTributeWeightEnabled` | A kingdom weighing a war on one that pays it tribute counts what the war would throw away: the tribute still owed, and the shame of breaking a peace whose price is still being paid. Both fade as the tribute runs out; it weighs, it does not forbid the war. Numbers you can change: `WarTributeOwedWeight` (1.5, times the tribute still owed), `WarTributeHonourPoints` (50000, the shame at the start of the tribute). |
| `PeaceNeedsOtherSideConsent` | Peace needs both sides, unless the war is decided or has lasted 80 days. Numbers you can change: `PeaceConsentShareOfThreshold` (0.75, how close the other side must be to wanting the peace itself), `PeaceWithoutConsentWarScoreGap` (375, the war score gap that decides a war). |
| `DiplomacyRulesApplyToPlayerKingdom` | The truce and peace rules also bind your own kingdom. |
| `CallerPeaceCoversCalledAllies` | When a kingdom that called an ally makes peace, the ally makes peace too. |
| `CallerStaysWhileAlliesAreBound` | A kingdom that called an ally cannot walk out of that war early. |
| `HeirRelationEnabled` | An heir inherits 10% to 70% of each relation, at random, instead of 70%. |
| `WarSupportExplained` | The kingdom screen explains why your lords back or oppose a war, or a peace. |
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
| `FeastsEnabled` | Feasts, and the tournaments of the feasts held in towns. | [Feasts](features/feasts.md) |
| `GrandTournamentEnabled` | A ruler's feast in a town is always the grand tournament of the realm, in every kingdom: high-tier gear of the realm's culture, a richer purse, renown and influence for the champion. Numbers you can change: `GrandTournamentPurse` (50000, the most a ruler puts up; an AI ruler what he can spare of it), `GrandTournamentPrizeMinTier` (5), `GrandTournamentRenown` (50), `GrandTournamentInfluence` (30), `GrandTournamentAiPrizeGoldCap` (100000, the most a champion away from you is paid in gold for the prize of any feast's tournament; 0 = as the game pays it). | [Feasts](features/feasts.md#the-grand-tournament-of-the-realm) |
| `FeastTournamentsEnabled` | Every other host's feast in a town has a tournament too, with the game's usual prize and a purse the host puts up. Numbers you can change: `FeastTournamentPurse` (5000, the most he puts up). | [Feasts](features/feasts.md#the-tournament-of-a-feast) |
| `FeastHallTalkEnabled` | At a feast, go into the lord's hall and have a word over the wine: a toast, what is said at the tables, a match between your houses, a matter of war and peace. Numbers you can change: `FeastToastRelation` (1, relation a toast brings, never above the feasts' 40). | [Feasts](features/feasts.md#a-word-over-the-wine) |
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
| `RealmDiscontentEnabled` | Discontent in kingdoms grown too large (off by default since 1.27.1). | [Civil war](features/civil-war.md) |
| `ConspiracyEnabled` | Plots and civil wars. | [Civil war](features/civil-war.md) |
| `RealmSizeAmbitionEnabled` | The larger a kingdom grows beyond its fair share, the more its lords resent the crown's wrongs, the sooner they plot or band together and the more readily they join. Numbers you can change: `RealmSizeFullAtTimesShare` (2), `RealmSizeGrievanceBoost` (1), `RealmSizePlotRelationBoost` (10), `RealmSizeJoinBoost` (10), `RealmSizeReckoningGrudgeCut` (0.3). | [Civil war](features/civil-war.md#great-realms-restless-lords) |
| `PlotsOnlyInLargeRealms` | Off by default. On: the old way, where the AI plots only in a kingdom grown too large or under a weak ruler, and a plot ends once its kingdom shrinks. | [Civil war](features/civil-war.md#too-large) |
| `ThroneClaimsEnabled` | Claims to the throne: every plot names from the start the house it would crown, a house with a claim (blood, marriage, a crown once worn or the law of the realm). Any discontented house may start a plot; the pretender needs the strength. Numbers you can change: `PlotMinStrength` (500, the Clan Strength a pretender needs), `PlotPretenderRelation` (10, the best relation with the ruler a pretender may have), `PlotPretenderBonus` (10, what being the one crowned adds to a pretender's wish to join) and `PlotClaimElectiveTop` (3, how many of the best claims to rule count as claims to the throne under an elective law), `PlotClaimBloodTop` (2, the same under a hereditary law or the founder's blood). Off: the house that starts a plot is its pretender and needs `PlotMinStrength`, and the ruler's close kin never plot. | [Civil war](features/civil-war.md#how-a-plot-starts) |
| `CivilWarOutsideRestraintEnabled` | Other kingdoms hold back from attacking either side of a civil war. | [Civil war](features/civil-war.md) |
| `CivilWarReunionEnabled` | A negotiated peace in a civil war brings the realm back together on terms that follow the war (the king steps down, the pretender's house inherits or is pledged the votes, amnesty, or the crown's terms); two kingdoms only when the leading house is of another culture or faith. Numbers you can change: `CivilWarReunionAbdicateFiefShare` (0.35), `CivilWarReunionHeirFiefShare` (0.15), `CivilWarReunionCrownFiefShare` (0.15), `CivilWarReunionAbdicateRatio` (1.5), `CivilWarReunionHeirRatio` (1.1), `CivilWarReunionAmnestyRatio` (0.9), `CivilWarPledgeMerit` (10), `CivilWarPledgeBrokenRelation` (20), `CivilWarPledgeBrokenGrievance` (20). Also a win by fiefs taken: `CivilWarWinFiefShare` (0.4; 0 turns it off), `CivilWarWinFiefMin` (2). | [Civil war](features/civil-war.md#the-outcomes) |
| `CivilWarNotifyPlayer` | A notice in the middle of the screen when any kingdom falls into civil war. | [Civil war](features/civil-war.md) |
| `IndependencePlotEnabled` | Plots to break away: houses with towns and castles on bad terms with the ruler, whose lands touch, may plot to leave the realm with their lands and stand as a realm of their own. Nobody is talked into it or out of it; it rises at 30% of the realm's strength with another house beside its leader. Numbers you can change: `IndependenceRelation` (-30, the relation with the ruler every house needs, or worse), `IndependenceLargeRealmRelation` (-20, the same in a kingdom of twice its fair share), `IndependenceRisesAt` (0.3), `IndependenceRisesSureAt` (0.5, from it an AI plot always rises), `IndependenceStartChance` (0.02 a week), `IndependenceStartPerCalculating` (0.01), `IndependenceStartPerHonor` (0.01), `IndependenceLargeRealmStartFactor` (1: up to twice as likely in a kingdom of twice its fair share), `IndependenceDukeFactor` (1.5), `IndependenceJoinAt` (30), `IndependenceCultureBonus` (10), `IndependenceLargeRealmPull` (10), `IndependenceNeighbourFiefs` (4), `IndependenceFizzleShare` (0.15), `IndependenceGiveUpDays` (180), `IndependenceLeaveMargin` (5), `IndependenceMaxPerRealm` (1). | [Civil war](features/civil-war.md#plots-to-break-away) |
| `CivilWarBriefingEnabled` | When your realm falls into civil war and your house stays with the crown as a vassal, a window tells you once what it is about, who rose and how it can end. | [Civil war](features/civil-war.md#when-your-realm-falls-into-civil-war) |
| `PlotStripRisingEnabled` | A fief taken from a house of a plot (by vote or decree) makes a plot with 40% or more of the realm rise at once, even in a war with another kingdom, after the other houses weigh joining it; a weaker plot may rise, or the house break away alone, or yield, by its head's character. Numbers you can change: `PlotStripRiseAt` (0.4), `PlotStripRiseBase` (0.6), `PlotStripRisePerValor` (0.2), `PlotStripRisePerCalculating` (0.15), `PlotStripJoinBonus` (15), `PlotStripJoinKinBonus` (10), `PlotStripJoinGrievanceBonus` (10). | [Civil war](features/civil-war.md) |
| `CrownWinsExecutesLeaderEnabled` | When the crown wins a civil war, the head of the house that led the rising is put to death (you choose as ruler; the same awaits you if you led it). Numbers you can change: `TraitorAiSpareChancePerMercy` (0.15, the chance an AI ruler spares him for each level of Mercy). Off: his house comes back like the others. | [Traitors and the houses of a realm](features/realm-houses.md) |
| `TraitorsEnabled` | The rebel houses that come back are marked as traitors: the ruler may pardon them, rebuke them before the court, take their towns and castles or banish them by decree, no vote and no influence; an AI ruler judges one at a time, hardest on the house that led the rising. A beaten house rarely defies the judgment, and one that loses land may leave the realm with nothing instead. Numbers you can change: `TraitorMarkDays` (60), `TraitorRefuseFactorOne` (0.5), `TraitorRefuseFactorAll` (1), `TraitorRefuseFactorBanish` (1.25, times the odds a house breaks away when a fief is taken), `TraitorKinRelation` (5, lost with the ruler by each house of kin or friends), `TraitorBanishRulerRelation` (10, lost between the ruler and the head of a banished house; a vote to expel costs 20 with every lord who backed it), `TraitorPardonRelation` (10), `TraitorAiPardonBase` (0.3, the house that led the rising), `TraitorAiPardonPerMercy` (0.2), `TraitorAiBanishChance` (0.25), `TraitorAiBanishMinHouses` (10); defying the judgment: `TraitorDefyFactor` (0.1, times the odds above), `TraitorDefyMax` (0.1); exile when land is taken: `TraitorExileBase` (0.1), `TraitorExilePerValor` (0.1, per point of Valor), `TraitorExilePerRelation` (0.003, per point of ill will toward the ruler), `TraitorExileMax` (0.4); an AI ruler's pace: `TraitorJudgeEveryDays` (4, days between two houses of the same realm); the houses that followed the leader: `TraitorFollowerPardonBase` (0.5, plus `TraitorAiPardonPerMercy`), `TraitorFollowerStripChance` (0.3, to take one town or castle), `TraitorFollowerStripPerPunished` (0.1, less for each house already stripped or banished in the same judgment), `TraitorFollowerMinLanded` (5, houses with a town or castle at or below which none is taken); a rebuke: `TraitorRebukeRelation` (10, lost with the ruler by the house's head), `TraitorRebukeGrievance` (15, weight of the grievance); a costly judgment: `TraitorAiCostlyPardon` (0.15, more to pardon) and `TraitorAiCostlyStrip` (0.1, less to take from a follower) for each house that defied or went into exile. | [Traitors and the houses of a realm](features/realm-houses.md) |
| `RealmJoinNeedsLandEnabled` | An AI kingdom takes in a noble house only with land for it. Numbers you can change: `RealmJoinMinFiefsPerHouse` (1.2). | [Traitors and the houses of a realm](features/realm-houses.md) |
| `RealmNewHousesEnabled` | An AI kingdom with many more towns and castles than houses raises a new house with its next fief to share out. Numbers you can change: `RealmNewHouseFiefsPerHouse` (2.2), `RealmNewHouseFromHouses` (11), `RealmNewHouseStepPerHouse` (0.3), `RealmNewHouseMinHouses` (5), `RealmNewHouseEveryDays` (30), `RealmNewHouseTier` (3), `RealmNewHouseGold` (50000). | [Traitors and the houses of a realm](features/realm-houses.md) |
| `HouseKnightsEnabled` | A rich AI house with land and too few lords for its parties takes knights into its service; they never inherit nor wed. Numbers you can change: `HouseKnightMinGold` (40000), `HouseKnightCost` (15000), `HouseKnightEveryDays` (30), `HouseKnightMax` (3). | [Traitors and the houses of a realm](features/realm-houses.md) |
| `LandedKnightsEnabled` | Landed knights, one for each castle a house holds (you too; in the Empire only the crown swears them, see the Empire's own ways below): houses of one knight holding the villages of one castle of its lord, with no vote, castle or army of their own, who rise to full houses when the kingdom has land to spare. A lord with a knight in every castle who takes you as his knight dismisses his weakest one (only for you). An AI lord raises a knight only with a full purse and lets one go once his house has been short of silver for a month (not you: your house needs no purse to raise or keep one, and you let yours go yourself, in person or by an envoy). Knights wear the noble gear of their culture and ride with their lord in a feud. From the House tab you may grant land to a worthy knight yourself, now and then. Numbers you can change: `LandedKnightCreateMinGold` (100000, an AI house's gold to raise a new knight, or to take you as its knight), `LandedKnightKeepMinGold` (30000, an AI house's gold to keep its knights or take on a landless one), `LandedKnightKeepPoorDays` (30, days in a row below it before it lets one go), `LandedKnightPlayerGrantDays` (20, days between two knights you raise with the House tab's button), `LandedKnightDismissRelationLoss` (5, regard a knight let go without a quarrel loses for his lord), `LandedKnightLordSpread` (0.4, how much less likely a lord is to make another knight for each he has), `LandedKnightStartTier` (1), `LandedKnightReadyTier` (2), `LandedKnightAscendLords` (2), `LandedKnightDailyChance` (0.05, a day in each kingdom), `LandedKnightGift` (10000), `LandedKnightMaxRealmAid` (200), `LandedKnightMaxVillages` (2), `LandedKnightLordMinVillages` (1, villages with no knight a lord must hold to grant a knight his castle's second one), `LandedKnightMoreRelation` (30), `LandedKnightMoreDailyChance` (0.01), `LandedKnightMoreAskAgainDays` (24, before you ask the same lord again for another village after he said no), `LandedKnightPlayerMaxTier` (1), `LandedKnightAskRelation` (10), `LandedKnightRevokeRelation` (-30), `LandedKnightRevokeDailyChance` (0.02), `LandedKnightRevokeRelationLoss` (20, with a grudge, when his land is taken from one his lord despises), `LandedKnightLandlessDays` (24, before a landless knight's house comes to an end), `LandedKnightOfferDailyChance` (0.1), `LandedKnightPagesDays` (48, before a knight's house that ended, and its people, leave the encyclopedia). | [Landed knights](features/landed-knights.md) |
| `LordErrandsEnabled` | As a landed knight, your lord sends you errands by a rider, one at a time; only you, not the AI's knights. One switch per kind: `LordErrandWorkEnabled`, `LordErrandRentsEnabled`, `LordErrandRoadEnabled`, `LordErrandGarrisonEnabled`, `LordErrandMessageEnabled`, `LordErrandJudgeEnabled`, `LordErrandRecruitsEnabled`, `LordErrandDebtEnabled`. Numbers you can change: `LordErrandHoldMaxDays` (20, days in all an errand may wait while its lord or place cannot be reached: at sea, besieged, in a battle; past that it is set aside without blame), `LordErrandEveryDaysMin` (20), `LordErrandEveryDaysMax` (30), `LordErrandMessengerWaitDays` (5), `LordErrandRelation` (5), `LordErrandRefuseRelation` (2), `LordErrandFailRelation` (6), `LordErrandRenown` (2), `LordErrandGenerosityGold` (0.2 more or less gold for each step of the lord's generosity), `LordErrandWorkEveryDays` (120), `LordErrandWorkPayShare` (0.85), `LordErrandWorkExtraDays` (20), `LordErrandRentsGold` (750), `LordErrandRentsSetOutDistance` (5), `LordErrandRentsCarters` (8), `LordErrandRentsAmbushChance` (0.6), `LordErrandRentsRaidersShare` (0.6), `LordErrandRentsRaidersMax` (30), `LordErrandRoadGold` (1500), `LordErrandRoadMenMin` (20), `LordErrandRoadMenMax` (30), `LordErrandRoadDays` (10), `LordErrandGarrisonGold` (1500), `LordErrandGarrisonMenMin` (8), `LordErrandGarrisonMenMax` (15), `LordErrandGarrisonMinTier` (3), `LordErrandGarrisonThinShare` (0.6), `LordErrandGarrisonStayDays` (2), `LordErrandGarrisonStayGold` (600), `LordErrandMessageGold` (1000), `LordErrandMessageLordRelation` (8), `LordErrandMessagePlayerRelation` (3), `LordErrandJudgeGold` (1000), `LordErrandJudgeWalkHours` (4), `LordErrandJudgeFairWinRelation` (10), `LordErrandJudgeLoserRelation` (6), `LordErrandJudgeCaughtRelation` (2), `LordErrandJudgeFairSplitRelation` (5), `LordErrandJudgeWrongedRelation` (10), `LordErrandJudgeUnfairWinRelation` (3), `LordErrandJudgeWinPower` (20), `LordErrandJudgeMend` (5), `LordErrandJudgeFairLordRelation` (3, on top of `LordErrandRelation`), `LordErrandJudgeUnfairLordRelation` (4 lost), `LordErrandJudgeUnfairPayShare` (0.5), `LordErrandJudgeQuarrelProduction` (0.2 less goods and food), `LordErrandJudgeQuarrelDays` (20), `LordErrandRecruitsGold` (400), `LordErrandRecruitsMin` (10), `LordErrandRecruitsMax` (20), `LordErrandRecruitsMaxTier` (2), `LordErrandDebtMin` (2000), `LordErrandDebtMax` (6000), `LordErrandDebtShare` (0.15), `LordErrandDebtCharmBase` (0.2), `LordErrandDebtCharmPerPoint` (0.002), `LordErrandDebtCharmMax` (0.85), `LordErrandDebtPressRelation` (10), `LordErrandDebtPressSecurity` (5), `LordErrandDebtPaidRelation` (3). | [Landed knights](features/landed-knights.md#errands-from-your-lord) |
| `KnightIssuesEnabled` | A notable of your fief with a trouble a companion could solve may hand it to one of your landed knights instead (*"My knight will see to it."*): the knight rides there with their own men, the trouble comes before any host, and the reward is yours. Numbers you can change: `KnightIssueRelation` (5), `KnightIssueRefuseRelation` (2), `KnightIssueFailRelation` (6), `KnightIssueRenown` (2), `KnightIssueRefuseFrom` (-9) and `KnightIssueRefuseAlways` (-30) (the relation from which a knight may refuse, and surely does), `KnightIssueSpareDays` (3), `KnightIssueSeaWaitDays` (3, days your rider waits for a knight at sea). | [Landed knights](features/landed-knights.md#troubles-of-your-fiefs) |
| `KnightIssuesPlayerAutoEnabled` | Your landed knights also take up troubles of your lands of their own accord, at no cost and no reward to you. Numbers you can change: `KnightIssueAiDailyChance` (0.015, a day for each knight, also for the AI's). | [Landed knights](features/landed-knights.md#troubles-of-your-fiefs) |
| `KnightIssuesAiEnabled` | AI lords send their landed knights to the troubles of their own lands in peacetime. | [Landed knights](features/landed-knights.md#troubles-of-your-fiefs) |
| `VillageWorksEnabled` | Whoever holds a village (its landed knight, else the lord of its castle or town; you and the AI alike) may raise a few small works there, one at a time; a raid stops the one under way and ruins one already raised. Numbers you can change: `VillageWorkWellCost` (5000), `VillageWorkWellDays` (10), `VillageWorkWellHearth` (0.15 hearths a day), `VillageWorkPalisadeCost` (6500), `VillageWorkPalisadeDays` (15), `VillageWorkPalisadeMilitia` (0.5 a day), `VillageWorkPalisadeRaidSlower` (0.2), `VillageWorkMillCost` (8000), `VillageWorkMillDays` (20), `VillageWorkMillProduction` (0.05), `VillageWorkStorehouseCost` (4000), `VillageWorkStorehouseDays` (10), `VillageWorkStorehouseRecovery` (0.03 a day), `VillageWorksAiReserve` (80000), `VillageWorksAiDailyChance` (0.002). | [Works in a village](features/village-works.md) |
| `TitlesEnabled` | Counties, duchies and the chain of lords and vassals in Vlandia, Sturgia, Battania, the Aserai and Nordvyg (and the themes and ulus below, which need it too): dues to its one lord (by its chief seat, kept while held; a duke's, the crown), titles kept without their land and taken only in a feud for the title, vacant duchies granted by the ruler, vassals following their lord in the realm's quarrels, a grievance against a lord who does not defend his vassal, a duke's grievance against a crown that keeps a town of his duchy for itself, and against a house of the realm that holds land in his duchy of another lord. Numbers you can change: `TitleRentShare` (0.025, the share of what a house's towns and castles yield a day that it pays its lord), `TitleDuchyVacantDays` (96, how long a duke or noyan keeps his title holding no town or castle anywhere, and a strategos a theme where he holds none), `TitleClaimGrantWeight` (60, what a firm claim to a vacant title adds when an AI ruler weighs a house for it; half for a weak one), `TitleUsurpedGrievance` (40, the grievance of a house whose title was won from it in a feud), `TitleGrantPerTown` (20), `TitleIsleDistance` (170), `TitleRoyalTownGrievance` (10, the grievance of a duke with a town of the ruler's in his duchy), `TitleForeignTownGrievance` (10) and `TitleForeignCastleGrievance` (5) (a duke's grievance against a house for each county, by its town, and each castle counted on its own that it holds in his duchy of another lord; 0 for none), `TitleLiegePull` (30), `TitlePlotLiegePull` (20, following one's lord into a plot against the crown), `TitleLiegeStayPull` (8), `TitleLiegeHateRelation` (-30), `TitleLiegeGrudgeFull` (20), `TitleFeudLiegeChance` (0.5), `TitleFeudLordBackChance` (0.5), `TitleFeudLordBackPerValor` (0.1), `TitleLordFailedGrievance` (12), `TitleLordFailedRelation` (8), `TitleLordAbsentGrievance` (6). | [Dukes, counts and castellans](features/titles.md) |
| `TitleLordDemandEnabled` | With `TitlesEnabled` and `FiefRevocationEnabled`: a duke or count may put the taking of a fief a vassal of lesser title holds of him before the council: if it passes, the fief is his; if the vassal refuses (with `RevokeAnyProposerEnabled`), a feud between them, and a vassal that holds out holds of the crown alone. | [Dukes, counts and castellans](features/titles.md#a-lord-takes-back-a-vassals-fief) |
| `TitleDuchyRightsEnabled` | With `TitlesEnabled` and `FiefRightsEnabled`: a duke or noyan holds a weak right to each county (by its town) or castle of his duchy held by a house of the realm that does not answer to him, while it lasts; a town won by it takes with it the castles of its county the losing house held. | [Dukes, counts and castellans](features/titles.md#rights-of-a-duchy-and-of-a-county) |
| `TitleCountyRightsEnabled` | With `TitlesEnabled` and `FiefRightsEnabled`: a count holds a weak right to each castle of his county held by a house of the realm that does not answer to him, and resents that house, while it lasts. Number you can change: `TitleCountyCastleGrievance` (5; 0 for none). | [Dukes, counts and castellans](features/titles.md#rights-of-a-duchy-and-of-a-county) |
| `FelonyJusticeEnabled` | A house that rides against its own lord in a feud and loses has its head sentenced to death by that lord (a merciful lord may spare him); off, it only loses its land in the lord's lands. In every feud each head calls his vassals, who choose a side. Numbers you can change: `TitleVassalTurnLean` (40, how far an AI vassal must lean to the other side to ride against his lord, before the fear of felony), `TitleFelonyRiskLean` (40, how much the fear of felony adds), `TitleFelonyHateLean` (50, how far hatred of his lord drives him), `TitleFelonyLeanSpread` (80, how wide the lean runs from never to always), `TitleFelonyOddsRatio` (1.5, the other side "clearly the stronger"), `TitleFelonyDeclareStrength` (1, the strength an AI house wants to declare a feud against its own lord, more against a cruel lord), `TitleVassalRoseGrievance` (15, a lord's grievance against a vassal who rode against him), `TitleTruceBreakLean` (20, how readily the other head of a feud paused for a lord's breaks the truce). | [Factions and grievances](features/factions.md#felony) |
| `ImperialThemesEnabled` | In a campaign begun with it on: themes in the three empires, each under a strategos the emperor names and relieves, not inherited. Numbers you can change: `ThemeGrantPerCastle` (10) and `ThemeGrantPerTier` (5), how an AI emperor weighs a house besides his relation with its head and `TitleGrantPerTown`; `ThemeDisgraceRelation` (-10, a strategos whose head is this or worse with an AI emperor is relieved); `ThemeIncumbentBonus` (20, how much better another house must be for a new emperor to replace the strategos); `ThemeRelievedGrievance` (12, the grievance of a house relieved). | [Dukes, counts and castellans](features/titles.md#themes-of-the-empires) |
| `KhuzaitUlusEnabled` | In a campaign begun with it on: the ulus of the Khuzaits, held and inherited by a house, given first to the khan's blood; vassals who owe the khan before their noyan; an ulus taken back for treason. Numbers you can change: `UlusBloodBonus` (30, how much a house of the khan's blood is favoured for a vacant ulus), `UlusWithdrawnGrievance` (30, the grievance of a house whose ulus is taken back with no land in it). | [Dukes, counts and castellans](features/titles.md#the-ulus-of-the-khuzaits) |
| `TitlesOathsEnabled`, `TitlesGreetingsEnabled`, `TitlesReliefEnabled`, `TitlesServiceEnabled`, `TitlesVassalCallEnabled` | Oaths, greetings, relief, the call to the banner, and the cheaper call of one's vassals to a host, between lords and vassals (with `TitlesEnabled`). Numbers you can change: `TitlesOathWarmRelation` (3), `TitlesOathColdRelation` (2), `TitlesGreetWarmRelation` (20), `TitlesGreetColdRelation` (-10), `TitlesGreetGrudge` (3), `TitlesRiderSpeedFactor` (1.5), `TitlesRiderMinHours` (2), `TitlesReliefScoreFactor` (2), `TitlesReliefRefuseRelation` (4), `TitleFeudReliefChance` (0.5, the odds an AI lord rides to a feud when his vassal sends for aid, before his honour, valour and regard for each side), `TitlesReliefKeptRelation` (4), `TitlesReliefBrokenRelation` (8), `TitlesReliefBrokenGrievance` (6), `TitlesServiceMaxRideDays` (2.5), `TitlesServiceRestDays` (7), `TitlesServiceJoinDays` (4), `TitlesServiceJoinRelation` (2), `TitlesServiceFailRelation` (8), `TitlesVassalCallCostFactor` (0.5). | [Dukes, counts and castellans](features/titles.md#oaths-and-duties) |
| `RealmShedHousesEnabled` | An AI kingdom with many houses and too little land lets a landless one go. Numbers you can change: `RealmShedMinHouses` (12), `RealmShedFiefsPerHouse` (1), `RealmShedEveryDays` (30). | [Traitors and the houses of a realm](features/realm-houses.md) |
| `ExpelRefuseEnabled` | A house the council votes out of a kingdom may refuse and break with it, holding its towns and castles. Number you can change: `ExpelRefuseFactor` (1.25, times the odds a house breaks away when a fief is taken). | [Traitors and the houses of a realm](features/realm-houses.md) |
| `SuccessionLawsEnabled` | Each realm follows its own law of succession when its ruler dies. Off: the base game's vote everywhere. | [The crown and its claim](features/succession.md) |
| `RightToRuleEnabled` | Every lord has a claim to the crown, and the ruler's claim has the effects below. | [The crown and its claim](features/succession.md#what-makes-a-claim) |
| `RightToRulePlotsEnabled` | A weak claim breeds plots: a lord with a better claim than the ruler starts one with less bad blood. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleOathEnabled` | The new ruler's claim weighs in every house's oath. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleWarEnabled` | The claim weighs in war and peace. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleCouncilEnabled` | The claim weighs in the council's support for the ruler's proposals. | [The crown and its claim](features/succession.md#what-a-claim-does) |
| `RightToRuleNotifyPlayer` | A line in your messages whenever a crown passes anywhere in Calradia. | [The crown and its claim](features/succession.md) |
| `FactionsEnabled` | Factions: charters, reckonings, the demand to step down, grievances. Off: the plots and civil wars of before, alone. | [Factions and grievances](features/factions.md) |
| `FactionGrievancesEnabled` | Every house remembers what the crown did to it. | [Factions and grievances](features/factions.md#lords-remember) |
| `FactionCharterEnabled` | The Charter: lords who would bind the ruler's hands. | [Factions and grievances](features/factions.md#the-charter) |
| `FactionReckoningEnabled` | The Reckoning: lords who would bring down an overmighty house. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `ReckoningSmallRealmEnabled` | In a realm below its fair share of towns and castles, AI houses back a reckoning's vote to take a fief less strongly. Numbers you can change: `ReckoningSmallRealmVoteCut` (0.5, the most their votes are cut), `ReckoningSmallRealmFullAt` (0.5, the size against its fair share at or below which the cut is whole; nothing at its fair share or above). | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `FactionAbdicationEnabled` | A strong plot asks the ruler to step down before it rises. | [Factions and grievances](features/factions.md#asking-a-ruler-to-step-down) |
| `FactionConfidantsEnabled` | Friends tell you what is afoot in their realm, and write when it comes to a head. | [Factions and grievances](features/factions.md#you-and-the-factions) |
| `FactionsInAiRealms` | Factions in the AI kingdoms too, not only in yours. | [Factions and grievances](features/factions.md) |
| `FactionFeudsEnabled` | A reckoning the ruler refused may take up arms: a feud between two houses of the realm over the fief. Numbers you can change: `FactionFeudKingLetWeight` (6: how readily a ruler of the AI lets the two houses settle it rather than forbid it or take a side), `FactionFeudKingClaimantsWeight` (2.5: how much more readily he stands with the claimants when he takes a side), `FactionFeudDays` (72, how long a feud over a fief lasts), `FactionFeudMaxPerRealm` (5, feuds at once in a realm), `FactionFeudTraitorDays` (7, the days of grace in the field after a house refuses the crown's call to arms against a foe at the walls). |
| `FactionFeudBlindEyeEnabled` | When the days of grace of a house that would not answer the crown's call to arms run out, the ruler may turn a blind eye instead of naming it traitor (an AI ruler by the house's strength, his character, his regard for its head and how the war goes; you choose): it costs the ruler's regard, and the ruler and the houses that obeyed hold it against them. Numbers you can change: `FactionFeudBlindEyeBase` (0.4), `FactionFeudBlindEyeRelation` (10), `FactionFeudBlindEyeKingGrievance` (15), `FactionFeudBlindEyeObeyedGrievance` (10). |
| `FeudSummonsEnabled` | Once the realm declares a war, the crown asks the two heads of each feud fought in arms to set it aside and ride in its host. Either may refuse; the feud waits for that war only if both heed. You are asked too. Numbers you can change: `FeudSummonHeedChance` (0.3, before a head's honour, cunning, regard for the ruler and grudge), `FeudSummonRefuseRelation` (5, lost with the ruler by a head who refuses). |
| `KingsPeaceEnabled` | In peacetime a ruler may proclaim the King's peace on a feud: both sides must lay down their arms. If one refuses, the feud goes on and after 7 days both choose again; a side that still refuses is judged by the crown. The AI does it rarely. Numbers you can change: `KingsPeaceInfluenceCost` (300), `KingsPeaceRelationLoss` (5, with each head), `KingsPeaceRefuseRelation` (10, lost by the houses of a side that refuses), `KingsPeaceHeedChance` (0.4). |
| `InternalWarWeaknessEnabled` | Plots, charters, reckonings and feuds no longer wait for peace: they may rise or take up arms while the realm fights another kingdom. A weak realm is less prone to it: while at war, a realm losing its wars, or much smaller than the others, starts them far less often (a large, dominant realm that is losing is not held back; a strategos' coup never is). Numbers you can change: `InternalWarWhileLosingFactor` (0.3, times the AI's chance in a weak realm at war), `InternalWarWhileAtWarFactor` (1, the same in any realm at war), `InternalWarSmallRealmBelow` (0.5, towns and castles under this share of the average realm count as weak), `InternalWarPrepRetryDays` (10, how often a feud made ready without weighing that weakness tries again to declare). Off: no weakness counts. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudKingHeedsRightEnabled` | The crown respects a firm right: against claimants with a firm right to the fief (or the title), the ruler, AI or you, may only let the houses settle it or give it to them by decree, never forbid the feud or stand with the holder. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudDefyCouncilEnabled` | An AI reckoning the council turns down may take up arms all the same. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudPressRightEnabled` | A house with a right to a fief another house of its realm holds may press it by the sword, with no reckoning: the AI's, and yours in person, by an envoy or from the Factions tab. A claim to a duke's title is pressed the same way, in a feud for the title. Numbers you can change: `FactionFeudPressRightDailyChance` (0.14, how readily an AI house presses a right), `FactionFeudTitleDays` (120, how long a feud for a title lasts), `TitleFeudTownPoints` (2) and `TitleFeudCastlePoints` (1, what each town and castle of the duchy counts), `TitleFeudWinShare` (0.6, the share of the land the two sides hold that a side must hold for `FactionFeudHoldDays` (10) days to win), `TitleFeudConquerStrength` (1, how strong an AI side must be against the duke's, unless it already holds the share). | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudPartyLimitEnabled` | While a noble house of the AI is out of its realm for a feud it may lead as many companies as a minor faction (or your house) of its clan tier; back home, the companies raised for it disband. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudPlayerJoinEnabled` | Kin and friends of either side of a feud ask your help when it breaks out, and you may offer your sword (or hire out your company as a mercenary) to either house at any time, in person or by an envoy. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudMusterEnabled` | When a feud breaks out, the lords of both sides whose companies are thin make recruiting their first care for some days: they ride to towns and villages with volunteers for them and recruit there as always. Their garrisons are left as they are. Numbers you can change: `FactionFeudMusterDays` (10), `FactionFeudMusterUntilRatio` (0.9 of what a company is filled to: its size, or less when its house cannot pay more wages), `FactionFeudMusterPriority` (3), `FactionFeudMusterReachDays` (2, how far from its lands a house is reckoned to find men when it weighs a feud). | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudHireMercenariesEnabled` | Each side of a feud hires free companies of sellswords, paid once by its richest house. Numbers you can change: `FactionFeudSellswordsMax` (4, counting the companies for hire below), `FactionFeudSellswordFeePerMan` (25), `FactionFeudSellswordFeeMin` (1000), `FactionFeudSellswordGoldShare` (0.3 of the payer's gold at most). | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudHireCompaniesEnabled` | Once a feud is declared, the lords of both sides (taking turns) may also hire the [companies for hire](features/free-companies.md), as any lord at war does, if their purses can bear it; never so many that fewer than `CompanyFeudLeaveFree` (2) stay free, and never with fewer than `FactionFeudCompanyMinDaysLeft` (15) days of the feud left or once the claimants hold the fief. Needs `FactionFeudHireMercenariesEnabled`, `CompanyHireEnabled` and `CompanyAiHireEnabled`. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudArmyRulesEnabled` | The lords of a feud's host can gather an army with lighter companies than a realm asks. Numbers you can change: `FactionFeudArmySizeRatio` (0.3 of a company's size; the game asks 0.6), `FactionFeudArmyMinStrength` (0; the game asks 1000). | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudPrepareEnabled` | A house of the AI that means to take up arms first gathers its men in silence and declares only when its lords' companies are nearly full and it can reach the walls; it lets the quarrel be if it cannot in time. Numbers you can change: `FactionFeudPrepareRatio` (0.75 of what the companies are filled to, wounded men counted), `FactionFeudPrepareDays` (30, not counted while a foe stands at the realm's walls), `FactionFeudPrepMaxDays` (90, the most a feud's preparations last in all). | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudFeasibleOnlyEnabled` | A house of the AI does not take up arms over a fief its side could never besiege. Numbers you can change: `FactionFeudFeasibleMargin` (0.65: a side that could bring about two thirds of what the siege asks, the sellswords it could hire included, may take up arms; it keeps recruiting and hiring while the feud lasts), `FactionFeudSiegeFactor` (1: how many times the strength within its walls a host brings before it lays siege to the fief in dispute, and what a house weighs when it decides; the game asks 2 for any siege, and this changes no other siege). | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionFeudGiveBackEnabled` | When a feud ends, fiefs taken that were not the one in dispute go back to their houses, unless the taker refuses. | [Factions and grievances](features/factions.md#when-a-reckoning-takes-up-arms-feuds-between-houses) |
| `FactionStripRebelsEnabled` | A house that loses a fief to a reckoning's vote may refuse it and break with the realm. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `RevokeFeudEnabled` | A house that loses a fief to a reckoning's vote but will not break with the realm may hold it by force; the reckoning then takes up arms in a feud the ruler lets them settle. Needs `FiefRevocationEnabled`, `FactionStripRebelsEnabled` and `FactionFeudsEnabled`. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `FactionGrievanceRelationsEnabled` | A wrong between two AI houses sours their heads at once. | [Factions and grievances](features/factions.md#lords-remember) |
| `FactionGrievanceRelationsWithPlayer` | The same against your house: an AI house you wrong thinks less of you. | [Factions and grievances](features/factions.md#lords-remember) |
| `FactionAbandonedGrievanceEnabled` | A house whose fief falls to a siege blames each army of the realm that lingered within `FactionAbandonedRideDays` (1 day) for `FactionAbandonedMinHours` (12) hours while free to come (not besieging elsewhere, not in a battle, not holding or relieving another besieged fief, not gathering, not marching to the fief) and never fought for it, you included; against the crown if it was the ruler's army. An army marching on the fief counts as coming however far off it is. The crown alone is blamed only when no army marched to the fief or lingered near it and no lord fought or stood within its walls, and never for a fief that fell within `FactionUndefendedMinSiegeHours` (24) hours of the siege beginning. Numbers you can change: `FactionGrievanceAbandoned` (10), `FactionAbandonedRelation` (5), `FactionAbandonedComingMinHours` (3, hours on its way for an army to count as coming). Off: the rule of before (any lord within `FactionUndefendedRideDays`, 1.5 days, spares the crown). | [Factions and grievances](features/factions.md#lords-remember) |
| `FactionMarshalBlameEnabled` | A fief that falls with no army near and no lord fighting for it is held against the realm's Marshal too. Number you can change: `FactionMarshalBlameShare` (0.5 of the crown's grievance and of the goodwill the ruler loses). | [The royal court](features/royal-court.md#the-marshals-burden) |
| `PleaToRelieveEnabled` | When you lead an army, a lord in it whose house has a fief besieged nearby asks you to relieve it. Numbers you can change: `PleaMaxRideDays` (3), `PleaRefuseRelation` (3), `PleaBrokenRelation` (6), `PleaKeptRelation` (5), `PleaUnaskedHelpRelation` (3). | [Factions and grievances](features/factions.md#lords-remember) |
| `FactionCrownGrievanceRelationsEnabled` | A wrong against the crown costs a little of the house head's goodwill toward the ruler (AI or you). Numbers you can change: `FactionCrownGrievanceRelationShare` (0.35 of the grievance), `FactionUndefendedRelationTown` (5) and `FactionUndefendedRelationCastle` (3) for a fief lost with no help sent. | [Factions and grievances](features/factions.md#lords-remember) |
| `FiefRightsEnabled` | Rights to fiefs: old rights to lost fiefs, rights by blood, by marriage, by leading the siege, old claims of a line, forged claims. Off: rights count for nothing. | [Rights to fiefs](features/fief-rights.md) |
| `FiefRightsVotesEnabled` | Rights weigh when a fief is shared out and in a reckoning's vote. | [Rights to fiefs](features/fief-rights.md#in-the-council) |
| `FiefRightsForgeEnabled` | Someone of your house left in a town or castle of another house (the game's "+") can forge a weak claim to it there. Numbers you can change: `FiefRightForgeCharmPoints` and `FiefRightForgeDailyChances` (the daily chance by Charm). At a duke's seat, a claim to his title: `TitleForgeSlowness` (2, how many times as long it takes). | [Rights to fiefs](features/fief-rights.md#a-claim-forged-at-a-foreign-court) |
| `FiefRightsMarriageEnabled` | When the head of a house, its heir or you marry into another noble house, a weak claim to the fiefs of the spouse's house of birth, for the spouse's life. Numbers you can change: `FiefRightMarriageReckoningRelation` (-20, how bad the heads' relation must be for an AI house to press such a claim; you press yours at any time), `FiefRightMarriageNearest` (2, how many fiefs of the spouse's house it reaches, the nearest to the house's lands; 0 = all). | [Rights to fiefs](features/fief-rights.md#a-claim-by-marriage) |
| `FiefRightsReckoningNeedsRight` | A reckoning can only be raised over a fief one of its houses has a right to. | [Factions and grievances](features/factions.md#the-reckoning-of-a-house) |
| `FiefRightsNativeRevokeNeedsRight` | Only the ruler may put any house's fief to the council; a vassal needs a right (their own or their reckoning's), or to be the lord the fief is held of. | [Rights to fiefs](features/fief-rights.md#in-the-council) |
| `FiefRightsAncestralEnabled` | Four or five AI houses in each kingdom start with an old claim to a fief of another house. Numbers you can change: `FiefRightAncestralPerRealmMin` and `FiefRightAncestralPerRealmMax` (4 and 5), `FiefRightAncestralNearest` (4, among the fiefs nearest the house's lands). | [Rights to fiefs](features/fief-rights.md#old-claims-of-a-line) |
| `FiefRightsAiForgeEnabled` | AI houses quietly forge claims to fiefs near their own; you hear of it when the fief is yours. Numbers you can change: `FiefRightAiForgeDailyChance`, `FiefRightAiForgePerRealm` (2), `FiefRightAiForgeNearest` (4), `TitleAiForgeShare` (0.25, how often an AI house seeks a claim to a nearby duke's title instead). | [Rights to fiefs](features/fief-rights.md#when-others-forge-claims-to-your-fiefs) |
| `FiefRightsFeudHonourEnabled` | Honourable houses with no ties to either side may stand with the holder in a feud over a weaker right. | [Rights to fiefs](features/fief-rights.md#in-the-council) |
| `FiefRightsEncyclopediaEnabled` | Rights in the encyclopedia pages of houses and fiefs. | [Rights to fiefs](features/fief-rights.md#where-to-see-it) |
| `EnvoysEnabled` | Envoys (all errands). | [Envoys](features/envoys.md) |
| `EnvoyMeetingEnabled`, `EnvoySoundEnabled`, `EnvoyGiftEnabled`, `EnvoyMarriageEnabled`, `EnvoyRecruitEnabled`, `EnvoyCouncilEnabled`, `EnvoyPlotJoinEnabled`, `EnvoyPlotLoyalEnabled`, `EnvoyFiefClaimEnabled`, `EnvoyFiefPlotEnabled`, `EnvoyFactionWinEnabled`, `EnvoyPactEnabled`, `EnvoyCallToWarEnabled`, `EnvoyHireEnabled`, `EnvoyPeaceTermsEnabled`, `EnvoyDemandFealtyEnabled` | Each envoy errand on its own. Numbers you can change: `EnvoyCaptureChance` (0.05, on each half of the road near an enemy), `EnvoyMaxChaseDays` (3), `EnvoyRetryDays` (30), `EnvoySoundBaseAccuracy` (0.8), `EnvoySoundMemoryDays` (60), `EnvoyMeetingMinDays` (2), `EnvoyMeetingMaxDays` (6), `EnvoyMeetingNoShowRelationLoss` (3), `EnvoyGiftSmall` (1000), `EnvoyGiftMedium` (5000), `EnvoyGiftLarge` (20000). | [Envoys](features/envoys.md) |
| `SpeakerKinEnabled` | Whoever speaks to a lord of their own blood, you in person or an envoy, lands each argument a little more often in the talks an envoy can also carry (the council, plots, fiefs, winning a house to your realm, demanding fealty). Numbers you can change: `SpeakerKinArgumentShift` (0.25). | [Envoys](features/envoys.md#how-the-envoys-speech-counts) |
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
| `RivalCallOutEnabled` | Face to face, you can call your rival out to the arena at once (needs `RivalDuelEnabled`). | [Your rival](features/rival.md) |
| `RivalAmendsEnabled` | Face to face, you can ask your rival what would end the feud: an apology (costs `RivalApologyRenown`, 15 renown), the blood price, or a refusal, by their character. | [Your rival](features/rival.md) |

### The Empire's own ways {#the-empires-own-ways}
See [The Empire's own ways](features/empire.md). In the three realms of the Empire there are no reckonings, no feuds between houses and no vassal's Annex; these have no switch. The rest:

| Switch | What it does |
|---|---|
| `ImperialPetitionEnabled` | A house with a right to a fief another house of the realm holds lays it before the emperor, who grants or refuses it; you in person, by an envoy or from the Factions tab. Numbers you can change: `ImperialPetitionDailyChance` (0.007, a day in each realm of the Empire, for the AI), `ImperialPetitionHearingDays` (5, before the emperor answers), `ImperialPetitionAgainDays` (60, before a refused house asks again). A house may refuse a weak emperor's grant: see `ImperialPetitionDefyEnabled`. |
| `ImperialPetitionDefyEnabled` | A house a petition takes a fief from may refuse a weak emperor (newly crowned, a doubted claim, or losing a war he does not dominate): it breaks with the realm with its fiefs, or its plot rises over the fief; the fief does not pass. Rarer than defying a king's decree; you are asked in a window, and before a strong emperor you, like the AI, give it up. Numbers you can change: `ImperialPetitionDefyFactor` (0.5, times the odds of defying a decree), `ImperialPetitionDefyClaimBelow` (60, a claim to the throne under this is doubted), `ImperialPetitionDefyNewRulerYears` (1, years an emperor counts as newly crowned). | [The Empire's own ways](features/empire.md#when-the-holder-will-not-give-it-up) |
| `ImperialPetitionDefySmallEnabled` | A small Empire (under half the realms' even share of towns and castles, `InternalWarSmallRealmBelow`) also counts as weak: a house that refuses keeps the fief and stays in the realm, and the emperor backs down. Number you can change: `ImperialBackDownRefuserRelation` (20, lost with the emperor by the head of the house that refused). | [The Empire's own ways](features/empire.md#when-the-holder-will-not-give-it-up) |
| `ImperialBackDownHumbleEnabled` | An emperor who backs down is humbled: for a while plots against the crown draw more lords, a strategos's coup gains pressure, and his claim to the throne bears the shame for the rest of his reign. Numbers you can change: `ImperialBackDownDays` (48), `ImperialBackDownMaxStack` (3, back-downs counted at once), `ImperialBackDownPlotBonus` (8), `ImperialBackDownCoupPressure` (0.25), `ImperialBackDownRecordPoints` (4, off the claim each time). | [The Empire's own ways](features/empire.md#when-the-holder-will-not-give-it-up) |
| `PronoiaEnabled` | Only the crown swears landed knights in the Empire: a pronoia, the rents of a village of any castle of the realm, whoever holds the castle (that house loses the rents while it lasts, with no grievance). A pronoia is the throne's and passes to a new emperor. |
| `StrategosCoupsEnabled` | When the Empire loses its wars or its emperor is weak, the strategos of a theme may plot to seize the throne: a blow at the palace, or, if the coup is strong and the emperor will not yield, a rising in arms that never splits the Empire. The emperor may come to suspect him and relieve him. Needs the themes (`ImperialThemesEnabled`). Numbers you can change: `StrategosCoupStartChance` (0.04, a week, times the pressure), `StrategosCoupStrikeWeeklyChance` (0.15), `StrategosCoupSuspicionChance` (0.08, a week), `StrategosCoupCooldownDays` (150, with no coup after one in that realm), `StrategosCoupSuccessCalmDays` (300, after one that crowned its strategos). |
| `WarImperialClaimEnabled` | Between two realms of the Empire, the claim to the whole Empire is a cause for war. Number you can change: `WarImperialClaimPoints` (80000). |
| `ImperialUnionEnabled` | In terms of peace between two realms of the Empire, a clearly beaten emperor may yield the purple: his realm ends and his lords go over to the other emperor with their lands. Needs `NegotiatedPeaceEnabled` and `VassalageEnabled`. Numbers you can change: `ImperialUnionLossShare` (0.3, of his towns and castles lost to that rival), `ImperialUnionMinNet` (4), `ImperialUnionGlobalGapDays` (300, days between two unions anywhere on the map). |
| `ImperialDefectionEnabled` | A house of the Empire on bad terms with its own emperor and better with another goes over to that emperor's realm more readily (the game's own defection). Numbers you can change: `ImperialDefectionPoints` (20000), `ImperialDefectionShare` (0.3). |

### The kingdom assembly {#the-kingdom-assembly}
See [The kingdom assembly](features/assembly.md).

| Switch | What it does |
|---|---|
| `AssemblyEnabled` | Once in each long peace the ruler summons the houses of the realm to his hall, in the form of its culture (the thing, the kurultai, the majlis, the oenach, the curia of the peers, the Senate), and the crown hears the cases the realm really has; you can summon one as ruler from a town or castle of your own. Numbers you can change: `AssemblyPeaceDays` (30), `AssemblyAiDailyChance` (0.3, an AI ruler's chance a day once it may be called), `AssemblyAiHonorChance` (0.1 more for each point of Honor), `AssemblyNoticeDays` (4), `AssemblyDays` (5), `AssemblyMaxTravelDays` (5), `AssemblyTravelScore` (10), `AssemblyMaxCases` (3), `AssemblyMissedRelation` (5, lost with the ruler by a house that stays away), `AssemblyMissedMemoryDays` (120), `AssemblyAccuseMaxDays` (120), `AssemblyAccuseMaxRelation` (0, an AI house accuses only at this relation or worse); how an AI ruler judges: `AssemblyRulingBase` (0.5), `AssemblyRelationWeight` (0.01), `AssemblyKinWeight` (0.15), `AssemblyCalculatingWeight` (0.08), `AssemblyHonorWeight` (0.1), `AssemblyBackWeight` (0.04), `AssemblyBackRelationGap` (20), `AssemblySpeechWeight` (0.08), `AssemblySpeechFullCharm` (200), `AssemblyServiceWeight` (0.08), `AssemblyRulingMin` (0.05), `AssemblyRulingMax` (0.95), `AssemblyExecutedWeight` (0.15); a petition for a fief of the crown: `AssemblyPetitionBase` (0.3), `AssemblyFirmRightWeight` (0.2), `AssemblyGenerosityWeight` (0.1), `AssemblyCrownKeepsFiefs` (3), `AssemblyPetitionRegardMax` (0.35), `AssemblyPetitionSpeechWeight` (0.15), `AssemblyPetitionTownLoss` (0.2), `AssemblyPetitionCastleLoss` (0.05), `AssemblyPetitionIncomeLossWeight` (0.5); sentences: `AssemblyFine` (3000), `AssemblyBloodPrice` (5000), `AssemblyStripChance` (0.3), `AssemblyStripMinFiefs` (2); the peers' and senators' vote: `AssemblyVoteRelationWeight` (0.02), `AssemblyVoteTraitWeight` (0.15), `AssemblySenateOverrideChance` (0.3), `AssemblySenateOverrideRelation` (5); the majlis: `AssemblyMajlisConsultWeight` (0.15), `AssemblyMajlisRelation` (3); the kurultai: `AssemblyKurultaiVoiceRelation` (-10), `AssemblyKurultaiKhanRelation` (2), `AssemblyKurultaiVoices` (2), `AssemblyKurultaiJoinBonus` (8), `AssemblyKurultaiPullDays` (60); defiance: `AssemblyDefyMaxRelation` (-10), `AssemblyDefyMinStrength` (0.5), `AssemblyDefyBase` (0.3), `AssemblyDefyPerValor` (0.1), `AssemblyDefyPerCalculating` (0.1), `AssemblyDefyPerRelation` (0.005), `AssemblyDefyMax` (0.7), `AssemblyDefySafeConductDays` (4), `AssemblyDefyArmyGraceDays` (2), `AssemblyDefySeizeRelation` (5); the Senate: `AssemblyAccountMinVillages` (1), `AssemblyPlotAccuseMaxRelation` (10), `AssemblyAccountBase` (0.3), `AssemblyAccountPerVillage` (0.1); interruptions: `AssemblyThreatDays` (1), `AssemblyThreatMinMen` (80), `AssemblyKingAwayDays` (2); the thing: `AssemblyTrialMinOdds` (0.45), `AssemblyTrialBoldOdds` (0.3). |
| `AssemblyKingStaysEnabled` | The ruler who presides goes to his hall and stays there until the assembly rises, unless his own land is attacked. |
| `AssemblyPlaintiffPullEnabled` | A house with a case to bring rides to the assembly from any distance, and more eagerly. Number you can change: `AssemblyPlaintiffScoreFactor` (3). |
| `AssemblyWarWrongsEnabled` | A house may accuse another of a wrong of the last war (deserting, going over to the foe, leaving a fief to fall, an ally or liege who failed it, a broken pledge). Numbers you can change: `AssemblyGrievanceCaseMin` (3, how heavy the grievance must still be; also for redress), `AssemblyWrongAccuseMaxRelation` (10), `AssemblyGrievanceGrowth` (1.5, how much a grievance dismissed or refused grows). |
| `AssemblyRedressEnabled` | A house may ask the crown to make good a wrong the crown did it: an office, a fief of the crown or gold. Numbers you can change: `AssemblyRedressBase` (0.35), `AssemblyRedressGold` (3000). |
| `AssemblyRewardEnabled` | The crown answers the service of the house that served it best in the late war. |
| `AssemblyHallTalkEnabled` | Between hearings, talk to the heads of the houses in the lord's hall about tomorrow's case: ask them to stand with your side, to stand aside, or sound them out, for nothing, for gold or for a favour, by their character; the AI's sides canvass the same way. Numbers you can change: `AssemblyHallAskerWeight` (0.5), `AssemblyHallKingWeight` (0.5), `AssemblyHallKinWeight` (40), `AssemblyHallAllyWeight` (20), `AssemblyHallGrudgeWeight` (0.5), `AssemblyHallRightWeight` (15), `AssemblyHallStrengthWeight` (10), `AssemblyHallMercyWeight` (5), `AssemblyHallStake` (10), `AssemblyHallGraveStake` (20), `AssemblyHallWithdrawEase` (15), `AssemblyHallFriendRelation` (30), `AssemblyHallHateRelation` (-20), `AssemblyHallAgreeLean` (30), `AssemblyHallHopelessLean` (-30), `AssemblyHallGoldPrice` (2000; 0 for no gold, only a favour), `AssemblyHallCriticalRelation` (2), `AssemblyHallAiAsks` (6, the houses each side of a case may ask), `AssemblyHallFavourDays` (120), `AssemblyHallFavourBrokenRelation` (10). |
| `AssemblyHallKingEnabled` | When your case comes up under an AI ruler, he waits for you in the lord's hall to hear you, rule and hear your answer in person, and you can ask him why he ruled as he did. Number you can change: `AssemblyHallKingWaitHours` (8). |

### Sparring with nobles {#sparring-with-nobles}
See [Sparring with nobles](features/sparring.md).

| Switch | What it does |
|---|---|
| `NobleSparringEnabled` | In peace, nobles of your realm in the same castle or town invite you to practise with blunted weapons, and you can ask them: the best of three falls, each fought until a side's leader goes down, in its own scene, sometimes two against two. Weapon experience and a little goodwill. Numbers you can change: `NobleSparringInviteDailyChance` (0.25, each morning, by his regard for you), `NobleSparringPlayerPairCooldownDays` (30, between two bouts with the same noble), `NobleSparringPlayerInviteGapDays` (5, days after an invitation or a bout of yours before another lord invites you), `NobleSparringPairChance` (0.35, two against two), `NobleSparringRelationGain` (2) and `NobleSparringRelationCeiling` (30, it never raises a relation above this). |
| `NobleSparringAiEnabled` | AI lords spar among themselves too, with no scene. Number you can change: `NobleSparringAiDailyChance` (0.05). |
| `NobleSparringWagersEnabled` | A bout may carry a wager of 1,000 to 3,000 denars, by the lord's wealth. |

### Faiths
See [The faiths of Calradia](features/faiths.md).

| Switch | What it does |
|---|---|
| `FaithEnabled` | Every people keeps a faith: priests, festivals, the sacred months and blessings. Off: none of it. |
| `FaithPriestsEnabled` | A priest of the town's faith in every town, who gives their recruits only to a pillar of their faith. |
| `FaithPietyEnabled` | The lords of your faith think better of you the more devoutly you keep it, the most devout think less of you if you do not, and your towns of your faith hold more loyally to you. |
| `FaithTroopsWageEnabled` | The warriors of the faiths ask far less pay than other soldiers. |
| `FaithTroopsEnabled` | A priest's recruits are his faith's own warriors, a line of three for each faith. |
| `FaithFestivalsEnabled` | Each faith's great festival, once a year in its holy town (every second year in fast mode). |
| `FaithSacredMonthsEnabled` | Every autumn the Aserai realms go to no war and raid nothing, and whoever attacks them then is cursed. |
| `FaithMissionsEnabled` | Priests ask the faithful for help, as the townsfolk do. Each mission has its own switch: `FaithMissionPilgrimsEnabled`, `FaithMissionGrainEnabled`, `FaithMissionRelicEnabled`, `FaithMissionHereticEnabled`, `FaithMissionShrineEnabled`. Off: no new ones are offered; those under way can still be finished. |
| `FaithVirtuesEnabled` | Each faith holds two virtues of character dear; the way you live raises you among its faithful, or lowers you. |
| `FaithDeedsEnabled` | Clearing bandits from the lands of your faith, defending its villages and winning back its holy town raise you among the faithful; executing its lords does not. |
| `FaithBlessingsEnabled` | Festivals leave a blessing on your company: morale, march or healing. |
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
| `FiefWaysScreensEnabled` | The town's Manage screen and the clan's Fiefs tab show the fief's faith and culture, and how far it has come to its realm's. |
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
| `CompanyHireEnabled` | The sellsword companies can be hired. Off = nobody hires them any more; a contract under way runs to its end. |
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
| `SquireLetter` | The errand of carrying a letter (or a threat) to another lord. Number you can change: `SquireHoldMaxDays` (20, days in all an errand or a call to your lord's host may wait while the one you must reach cannot be reached; past that it lapses without blame). |
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
| `SquirePupil`, `SquirePupilKeepsGear`, `SquirePupilFire`, `SquirePupilBattle`, `SquirePupilYard`, `SquirePupilYardPeaceOnly` | A squire of your own once you are a knight: offered at all; he keeps his own gear (off = you can take it in the inventory); he comes to your fire; he is outlined in battle and starts at your side; bouts with him; those bouts only in peacetime. See [Squire service](features/squire.md). |

### Lords who remember you, captives and companions with a story

| Switch | What it does | Page |
|---|---|---|
| `NobleMemoryEnabled` | Lords remember what you did to them and theirs, and bring it up when you talk. | [Lords who remember you](features/memories.md) |
| `LordMemoriesEnabled` | Lords remember what other lords did to them and theirs, and it moves the relation between their houses while it is remembered (between AI lords only; yours moves as in the game). Numbers you can change: `MemoryTourneyRelation` (-1), `LordMemoryTourneyDays` (30), `MemoryBattleWithRelation` (1), `MemoryAidRelation` (3), `MemoryCapturedRelation` (-3), `MemoryRescuedRelation` (5), `MemoryKinKilledRelation` (-10), `MemoryKinExecutedRelation` (-20), `LordMemoryMaxPerLord` (20), `LordMemoryMaxRecords` (10000). | [Lords who remember you](features/memories.md#lords-remember-each-other) |
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
| `CourtOfficesEnabled` | The five offices of the court (Marshal, Steward, Master of Works, Chancellor, Warden of the King's Peace) and what they give. Number you can change: `CourtChancellorMaxGrievanceCut` (0.5, the most of the goodwill lost over the crown's wrongs a chancellor spares the ruler, reached only at `CourtChancellorGrievanceFullSkill` Charm, 300; below it the cut falls off with `CourtChancellorGrievanceCurve`, 2, so Charm 240 spares about 30%; up to 0.9). |
| `CourtAiAppointEnabled` | AI rulers name their own court and may offer you an office. Numbers you can change: `CourtVacancyFillMinDays` (4) and `CourtVacancyFillMaxDays` (8; 0 = off), how soon an empty office is filled. |
| `CourtChargeEnabled` | When you hold an office for an AI ruler, the affairs of that office come to you as the ruler's charge, with greater rewards. |
| `AudiencesEnabled` | Petitioners come to you with requests, and **Hold court** in your own towns and castles calls them in and hears them, then the notables of the place with tasks for you. |
| `AudienceClaimEnabled` | As ruler, in peace, the head of a house of your realm with a right to one of your towns or castles may come to ask for it. Numbers you can change: `AudienceClaimGrantRelation` (15), `AudienceClaimDelayFail` (3), `AudienceClaimRefuseRelation` (6), `FactionGrievanceClaimDenied` (8), `AudienceClaimRestDays` (120), `AudienceClaimWeight` (1.5, how often it comes up against the other requests, 1 each). See [The royal court](features/royal-court.md#the-requests). |
| `CorruptionEnabled` | A house with two or more towns and castles loses part of their taxes to corruption, more with each one; its governor's Steward cuts it. See [Other changes](features/other-changes.md#corruption-in-a-wide-demesne). |
| `LandHoardEnabled` | Too much land in one hand: the lords resent a house with more towns and castles than its tier less one (at least 1; the crown 2 more) that are also more than 20% of the realm (the crown 30%): a grudge that grows while it lasts, and 5 less goodwill with the head of each begrudging house for each town or castle beyond, given back once the house holds less. Numbers you can change: `HoardMinFreeFiefs` (1), `HoardRulerExtraFiefs` (2), `HoardRulerMinShare` (0.3), `HoardVassalMinShare` (0.2), `HoardEveryDays` (30), `HoardGrievancePerFief` (2), `HoardRelationPerFief` (5). See [Factions and grievances](features/factions.md#lords-remember). |
| `WorldNewsEnabled` | Ask any lord for the news of any realm of Calradia. Number you can change: `WorldNewsMinRelation` (-10, below it he will not tell). See [Factions and grievances](features/factions.md#you-and-the-factions). |
| `RealmAffairsTalkEnabled` | Ask any lord of a realm what is happening in it: civil war, traitors, feuds, causes, talk of plots, vacant titles, wars. Uses `WorldNewsMinRelation` too. See [Factions and grievances](features/factions.md#asking-how-things-stand). |
| `HouseTalkEnabled` | Ask a lord about his house: its lands, titles, rights, claim to the throne, allies and foes, and where it stands with the crown. See [Factions and grievances](features/factions.md#asking-how-things-stand). |
| `HouseAlliancesEnabled` | Alliances between houses of a realm, by marriage (if their heads were on good terms) and by a sworn pact between friends; allies are called to arms in a feud. Numbers you can change: `AlliancePactMinRelation` (30), `AlliancePactChance` (0.01 every `AlliancePactEveryDays`, 30), `AllianceBreakRelation` (0), `AllianceRefuseRestDays` (60), `AllianceRefuseRelation` (10), `AllianceRefuseGrievance` (8). See [Factions and grievances](features/factions.md#alliances-between-houses). |
| `AlliesInCausesEnabled` | A house leans more to join a plot, charter or reckoning an ally leads, and far less to join one against an ally. Numbers you can change: `AllyLeadsCauseJoinBonus` (15), `AllyOfTargetPenalty` (30). |
| `MarriageOtherRealmEnabled` | Weddings across realms are rarer than within one. Number you can change: `MarriageOtherRealmFactor` (0.25 of a wedding within the realm; the base game, 0.5). |
| `FeudAllyCallEnabled` | Allies called to arms when a feud breaks out. Numbers you can change: `FeudAllyCallBase` (0.8), `FeudAllyCallPerHonor` (0.1), `FeudAllyCallMin`/`FeudAllyCallMax` (0.2/0.98). |
| `FeudCourtEnabled` | The heads of a feud's sides court other houses that have a cause of their own, and pay those who come a compensation for their men; you can too, in person or by an envoy. Numbers you can change: `FeudCourtEveryDays` (3), `FeudCourtRetryDays` (15), `FeudCourtMax` (0.7), `FeudCourtFriendRelation` (20), `FeudCourtFoeRelation` (-10), `FeudCourtMinGrudge` (5), `FeudCourtCompensationShare` (0.5 of their wages for the days left), `FeudCourtCompensationReserve` (20000). |
| `FeudAiDefiesBanEnabled` | A house of the AI may defy the crown's ban on its feud, as you may. Numbers you can change: `FeudAiDefyBase` (0.05), `FeudAiDefyMax` (0.4). |
| `FeudPartySizeEnabled` | Lords' companies of houses riding in a feud hold more men. Number you can change: `FeudPartySizeBonus` (0.2). |
| `FeudAssaultWaitEnabled` | An AI army besieging the fief in dispute of a feud does not storm it until the walls are down, at most `FeudAssaultWaitMaxDays` (8) after the siege began. |
| `FeudStrengthCountsHiresEnabled` | When a house of the AI weighs a feud, what its purse could hire counts in its strength. |
| `FeudReachCountsCourtingEnabled` | When a house of the AI weighs whether its side could take the walls, the houses with a cause to join it count too, as likely as they are to come. |
| `OathEnabled` | When a kingdom gets a new ruler, every house swears to them, asks for something or refuses. |
| `FiefRevocationEnabled` | Proposing to take a fief from a vassal worries your other vassals, and the holder may break away with its fiefs. |
| `RevokeAnyProposerEnabled` | Whoever proposes to take a fief, the house that loses it may refuse and break away (with `FiefRevocationEnabled`); when its own lord asked, it bars the gates and fights a feud with him instead. |
| `RevokeRulerKeepsFiefEnabled` | A fief the ruler takes by the council's vote passes to the ruler, with no share-out (with `FiefRevocationEnabled`). |
| `BreakawayPeaceRulesEnabled` | A house that broke away over a fief makes peace with its old kingdom only on the terms between kingdoms (the crown willing, the war decided, or 80 days of war). |
| `FiefPlotEnabled` | As ruler, win lords over to vote for taking a fief from another house. |
| `FiefClaimFourCandidates` | Four candidates when a fief is shared out; right after a conquest, the house that led it always stands. See [Council](features/council.md#who-gets-a-fief). |
| `FiefClaimRulerStands` | One more candidate when a fief is shared out: the ruler's house always stands for a fief not its own, unless the realm's charter gives fiefs to the realm. See [Council](features/council.md#who-gets-a-fief). |
| `FiefClaimEnabled` | Ask a lord for their voice for your house when the next fief is shared out. |
| `FiefClaimFriendshipEnabled` | Every lord's vote for a house, yours or the AI's, rises a little with how much they like its head. |

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
| `PrudenceReliefWaitEnabled` | A relief gathers a few hours from the besiegers' camp until it is strong enough (game version 1.5.6 only). |
| `PrudenceRallyEnabled` | An AI army too weak for its siege or relief calls more lords. |

### Realms on the back foot (on by default) {#realms-on-the-back-foot-on-by-default}
See [Realms on the back foot](features/command-your-armies.md#realms-on-the-back-foot-on-by-default). These work whether `PrudenceEnabled` is on or off.

| Switch | What it does |
|---|---|
| `DefensiveStanceEnabled` | An AI realm much weaker than its enemies and behind in one of its wars fights as the game's defensive stance makes your lords fight: against every realm at war with it, fewer sieges and raids, quicker reliefs, and quicker to ride at enemy parties. Never the realm you rule. Numbers you can change: `DefensiveMinNetFiefs` (1, towns and castles lost, net, to an enemy in this war to count as behind in it), `DefensiveMinScoreGap` (100, or how far behind in the war's score), `DefensiveSiegeFactor` (0.65, the weight of a siege or raid against those enemies; the game's own), `DefensiveDefendFactor` (1.1, of relieving one of its places), `DefensiveEngageFactor` (1.2, of riding at their parties). |

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
| `FastModeMarriageRelationEnabled` | In fast mode a wedding gives exactly +20 relation between the two houses instead of +50 or more. See [Fast mode families](features/fast-mode.md). |
| `FastModeChildrenEnabled` | More AI children in fast mode. |
| `ChildCultureEnabled` | A child of two AI characters takes the father's culture 9 times out of 10. |
| `SiegePreparationEnabled` | Siege preparations take 1.5 times as long. See [Other changes](features/other-changes.md). |
| `SiegePatienceIgnoresAddedPreparationTime` | The AI besieger is not made impatient by that extra time. |
| `AiPeaceTrainingEnabled` | Once their kingdom has been at peace for 10 days, AI troops get only a quarter of their free daily training. |
| `GearPricesEnabled` | Fairer prices of weapons and armour for the player. |
| `ApplyToWeapons` | Weapons get cheaper too. Off = only armour. |

### Logs
`EventLogEnabled`, `DiplomacyLogEnabled`, `CourtMeasureLogEnabled`, `RivalLogEnabled`, `MercContractLogEnabled`, `SquireLogEnabled`, `NobleMemoryLogEnabled`, `CaptiveLogEnabled`, `StoryLogEnabled`, `FixRealmLogEnabled`, `CompanyLogEnabled`, `PrudenceLogEnabled` (AI armies, the realm's Marshals and their orders), `FaithLogEnabled` (faiths), `NobleSparringLogEnabled` (sparring) and `AssemblyLogEnabled` (the assembly) write detailed lines to the game's log, useful only when I ask you for a log to track a bug. Off by default.
