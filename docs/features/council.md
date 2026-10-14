# Win the council over

Talk the clan leaders of your own kingdom, the ruler included, into backing or opposing a war or a peace. You argue it out with the game's own persuasion, and a lord you win over votes your way on that matter for a month.

![Raising a matter of war and peace with the king](../assets/council-persuasion.jpg)

## Starting the conversation

Talk to the leader of any other clan of your kingdom and choose **"There is something I'd like to discuss."**, then **"There is a matter of war and peace I would raise with you."**

It works whether you are a vassal or the ruler. Neither you nor the lord can be a mercenary. A lord whose relation with you is below -30 refuses: *"I do not discuss the affairs of the realm with you."*

Choose what you want:

- **"We should go to war."** / **"There is a war we should keep out of."** Lists the kingdoms your kingdom could declare war on right now (not during a truce or while they pay you tribute, see [War and peace](war-and-peace.md)).
- **"We should make peace."** / **"There is a war we should not end yet."** Lists the kingdoms you are at war with.

Then pick the kingdom.

## Where the lord stands

The lord first tells you what they think and why, for example *"The Vlandians are stronger than we are. I see more to lose than to gain."* Then one of these:

- **They already agree:** *"You need not waste words on me. I am of the same mind."* Nothing to do.
- **They can be argued with:** their view ends with *"But say your piece; I will hear it."* The persuasion starts.
- **Their mind is made up:** *"My mind is made up, and nothing you say will change it."* They are too far from your view to be moved.
- **Peace is not possible yet:** *"There can be no peace with them yet, whatever you or I may think of it."* The rules of peace (see [War and peace](war-and-peace.md)) do not allow it yet, so a promise would be worth nothing.
- **You already tried and failed recently,** or they **already gave you their word** on this.

## The arguments

You get four arguments. Three depend on the matter, and the fourth is always a personal favour (*"Do this for me, as a friend. I will not forget it."*). Each argument uses one of your skills (Leadership, Tactics or Charm) and appeals to one trait.

An argument is easier when:

- it is **true** as things stand: *"The Sturgians are already at war elsewhere. We will not get a better chance."* lands better when they really are, and *"(town) is ours by right"* when the other kingdom really holds a town or castle of your kingdom's culture;
- it suits the lord's **character**: a valorous lord likes talk of glory, a merciful one listens to the suffering of the people, a calculating one to counting the spears, an honourable one to right and wrong, a generous one to a favour between friends;
- you get on well with the lord (for the favour).

Most lords need **2 arguments** to land; the hardest ones need **3**. An argument that lands very well counts double, and one that goes very badly takes one away.

You can stop with *"I have nothing more to say on it."* Leaving before making any argument costs nothing.

## Your chances

How hard a lord is depends on how far they are from your view, your relation with them, and whether they are the ruler. Rough odds with a typical mix of arguments (not counting perks):

| How far the lord is from your view | Relation 0 to 14 | Friend (15 to 49) | Close friend (50+) | The ruler (relation 0 to 14) |
|---|---|---|---|---|
| Almost agrees | 85% | 90% | almost certain | 60% |
| Has doubts | 75% | 85% | almost certain | 40% |
| Against it | 60% | 75% | 95% | 35% |
| Strongly against it | 40% | 60% | 90% | 5% |
| Very strongly against it | 35% | 40% | 75% | almost none |
| Mind made up | cannot be moved | cannot be moved | cannot be moved | cannot be moved |

- A close friend (relation 50 or more) also starts one argument ahead.
- A lord you are on bad terms with is harder: one step down the table below 0 relation, two steps below -15.
- The ruler is two steps harder than any other lord.

!!! tip
    **Feasts make it easier.** At a [feast](feasts.md) of your kingdom, a lord who is there with you is one step easier to persuade. With the whole council in one hall, a feast is the best time to win votes.

## What you get

**Success:** the lord votes your way on that matter, with a firm vote, for **30 days**. You see a message such as *"(clan) will back a war with the Vlandians for the next 30 days."* A ruler you win over votes the same way and will not overrule the council on it.

Winning lords over changes their vote, not what they propose. Someone still has to put the war or peace to the council, and that can be you. A promise for peace only counts while the rules allow that peace.

You also gain the skill experience the base game gives for the arguments that landed, at most once per clan every 30 days.

**Failure:** the lord will not discuss that matter with you again for **45 days**. If an argument went very badly they get angry (*"You overstep. I will not hear another word of this."*): **60 days** and **-4 relation**.

If you later ask a lord for the opposite of what they promised you, and they already agree with it on their own, the old promise is cancelled and you get a message.

A promise ends if the lord's clan leaves the kingdom, and all promises end if you leave it.

!!! note
    A family member or companion sent as an [envoy](envoys.md) can win a lord over the same way, with the same promises and waiting times.

## Turn it off

In the [settings file](../settings.md), set `CouncilPersuasionEnabled` to `false`. The conversation is no longer offered.
