# The faith and ways of a fief

A town or castle that changes hands does not change its people. Its notables keep their old ways, and its people pray as they always have. Slowly, over the years, a fief takes up the faith and the ways of the realm it belongs to. Until it does, its people are restless, and its lord has choices to make.

Needs [the faiths](faiths.md) on for everything about faith; the ways (culture) change either way.

## What a fief takes up

- **The faith** of the realm: the faith of its ruling house. A fief keeps its own until enough of its people have come round, and then it keeps the realm's: its priest is the realm's, its festivals and pilgrims are the realm's.
- **The ways** of the realm: its culture. This goes notable by notable, in the town and in its villages. Each takes up the new ways on their own, sooner the more they like the fief's lord. When half of them have, so has the fief and its villages: its townsfolk, its militia and the recruits of its notables. The rest follow sooner after that.

A house with no realm brings its own faith and ways. A fief that passes to another realm starts over toward the new one; a fief that goes back to a realm of its own faith and ways is at peace again.

With nothing to help or hinder it, the faith takes about **300 days** and the ways about **400 days** (a related faith comes round about a third faster). What its lord does can make the faith come sooner, but never quickly: a lord who does everything in his power still waits about **200 days**. A lord who leaves the old temple and its priest to its people waits more than twice as long.

In a campaign started before this version, fiefs already held by a realm of another faith are taken to have come half way already.

Once a fief has taken up a realm's ways, that realm's old enemies no longer count it as *their* land to win back.

## Restless people

While a fief keeps another faith or other ways than its realm's:

- **Loyalty.** The game already takes loyalty from a fief of another culture than its lord's. A fief of another faith loses some more each day (less for a related faith), easing as the new faith takes hold. It shows in the fief's loyalty breakdown as *Of another faith*.
- **Risings.** A town of another faith **and** other ways rises at a higher loyalty than the game's (35 instead of 25), one with only one of them at 30, and higher still for a while after its temple is destroyed or its old laws are revoked. The rebels are its own people, of its old ways.
- **Trouble.** Now and then: a preacher of the old faith has the crowd in the square (loyalty), a brawl in the market between old families and newcomers (security), or a fire at the new faith's altar (the new faith loses ground). If the fief is yours, you hear of it.

## The old temple

When a town of another faith is taken by siege, whoever took it decides, once, what becomes of its temple:

| Choice | What follows |
|---|---|
| **Leave it to them** | The people rest easier, and the new faith takes a long time to take hold. |
| **Give it to the realm's priests** | A priest of the realm's faith takes it that same day. The faith takes hold faster; the people resent it for a while. |
| **Destroy it** | The realm's priest preaches in the open. The old faith will not last long, but the town's loyalty falls at once, it is readier to rise for a while, and every head of a house of the old faith thinks less of whoever gave the order. |

AI lords choose by their character: merciful ones leave it, calculating ones give it to their priests, and only cruel lords who care little for honour destroy it.

Castles have no temple of their own, and no choice to make.

## The old priest

While a town of yours keeps the old faith, its priest is still there. Speak with them (at the temple, or *"Seek out..."* in the town menu if their temple is no longer theirs):

- **Leave them in peace.** They keep their people from foolishness: less trouble, but the new faith comes a little slower.
- **Banish them** (only if you gave the temple to your priests or destroyed it). They go to preach in one of the town's villages for a couple of months, and there is more trouble while they do. Ride to that village and you can **seize** them: the preaching ends, and the town is angry for a while.
- **Win them over**, with the game's persuasion. It is easier the further the new faith has come, with a related faith, and if they like you; harder with an honourable priest or a destroyed temple. If they agree, they keep the realm's faith from then on and the town comes some way round at once. If they refuse, they will not hear it again for a while; if it goes badly, they think much less of you and the people hear of it.

AI lords do the same by their character and their Charm.

## Helping it along, and calming the people

- **A mission.** Ask a priest of your realm's faith: *"Some of my lands do not yet keep our faith. Would you send preachers there?"*. Choose the fief and the purse; for a month or so the faith takes hold faster there. Where the people are angry, the preachers may be stoned in the street and flee, and no one will go back there for a month. A town whose temple you left to its people gets its first priest of your faith this way.
- **Alms.** In hard times (the town is starving, or was besieged or its village raided lately) a new option in the town or castle menu: *Give alms to the people*. Two purses. Loyalty rises, and where a new faith is taking hold, the people listen a little more. Once a month.
- **The old laws.** Through the fief's governor (*Speak with ... about the old laws*): grant the fief its old laws by charter, for some influence. While the charter stands, the people do not feel the game's loss of loyalty for a lord of another culture, there is less trouble, but the fief keeps its ways about five times as long. Revoking the charter costs loyalty at once, the notables think less of you, the town is readier to rise for a while, and no new charter is believed for some months. Without a governor there is no one to keep the laws in your name.
- **The governor.** A governor of the fief's own ways calms its people; one of the realm's faith helps the faith along.
- **Festivals.** The game's daily project *Festival and Games* gives twice the loyalty in a fief that is changing. A lord who left the old temple to its people gains some loyalty there while the old faith's great festival is under way.

The AI does all of this too: it grants the old laws when a fief is near rising, pays for missions and alms when it has silver to spare, and now and then a calculating lord revokes a charter once the fief is quiet.

## Where to see it

- **The encyclopedia.** A fief's page says how far the new faith has come and whether its notables still keep the old ways, what became of its temple, and whether it keeps its old laws.
- **The loyalty breakdown** of the fief: *Of another faith*, *Their temple given over*, *Their temple torn down*, *Their old laws kept*, *Their old festival honoured*.

## Turn it off

In the [settings file](../settings.md), set to `false`:

- `FiefWaysEnabled`: all of it (fiefs already changed stay as they are);
- `FiefWaysTempleEnabled`: the choice over the old temple;
- `FiefWaysOldPriestEnabled`: leaving, banishing or winning over the old priest;
- `FiefWaysMissionsEnabled`: missions;
- `FiefWaysAlmsEnabled`: alms;
- `FiefWaysOldLawsEnabled`: the old laws;
- `FiefWaysUnrestEnabled`: trouble in the streets;
- `FiefWaysRebellionEnabled`: towns rising sooner.
