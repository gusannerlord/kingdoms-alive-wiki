# Events between clans

The clans of a kingdom do not just sit side by side. Now and then two of them share a hunt, lend each other silver, quarrel over a boundary or insult each other at table, and their leaders come to like or dislike each other a little more. Over time this decides who stands with whom when a [plot](civil-war.md) begins.

## How often

- In **every kingdom**, one event every **15 to 25 days**.
- In a kingdom with fewer than 8 clans the wait is longer, so that each pair of clans sees events about as often as in a kingdom of 8. With 4 clans, for example, it is roughly 70 to 120 days. The wait is never more than 6 times the usual one.

## Who is involved

Any two vassal clans of the kingdom can be picked (mercenaries are not), including yours and the ruler's.

- Clans whose home settlements are within about **1.5 days' ride** of each other are **twice as likely** to be picked. Neighbours help each other and quarrel more.
- Pairs that include the **ruler's clan** are **half as likely**.

## Good or bad

About **55%** of events are bad. The chance shifts with the two clan leaders:

- each level of **Generosity**, **Mercy** or **Honor** in either leader makes a bad event 5% less likely;
- each level of **Calculating** makes it 5% more likely;
- leaders who already like each other have up to 10% fewer bad events, and leaders who dislike each other up to 10% more. Friends tend to stay friends, and enemies stay enemies.

Whatever the traits, the chance of a bad event stays between 20% and 80%.

## How big

| Kind | Usual change | Larger change |
|---|---|---|
| Good | +2 to +4 (85% of the time) | +6 to +10 (15%) |
| Bad | −2 to −5 (80% of the time) | −8 to −12 (20%) |

Good turns bring two houses a little closer. Quarrels are a little more frequent and hurt a little more, so over many events relations drift slowly downward unless something mends them.

**Cap:** an event never takes a relation above **+60** or below **−60**. A good event between leaders already at +60 or more changes nothing, and so does a bad one between leaders at −60 or less. Your Charm does not make these changes any larger or smaller.

## The twelve events

The window title is the event's name. Larger changes usually come with the more serious stories.

| Event | Kind |
|---|---|
| A hunt in the hills | good |
| A loan in a lean year | good |
| A ward taken in | good, larger |
| Help against brigands | good |
| A gift of horses | good, larger |
| A word in council | good |
| A boundary stone moved | bad |
| A caravan plundered | bad, larger |
| An insult at table | bad, larger |
| A share of the spoils | bad |
| A debt unpaid | bad |
| Whispers at court | bad |

## What you see

**Between two other clans of your kingdom:** a short message, for example *"In {Kingdom}: A debt unpaid. The {clan} and the {clan} think worse of each other."*

**When your clan is one of the two:** the game's event window opens, with the story and *"Your relation with {leader} of the {clan} has gone −5 and now stands at 12."* The change has already happened; your choice can move it further. Hovering over each choice shows what your relation will be afterwards.

The window waits until you are free (not in a battle, a conversation or captivity). If it cannot open within 2 days, you just get a message with the change.

### After a bad event

| Choice | Cost | Effect |
|---|---|---|
| *"Make amends: send X denars to {leader}."* | **2,000 denars × the other clan's tier**, paid to their leader. If you cannot afford it: **20 influence** instead (*"Make amends: spend 20 influence at court on it."*). With neither, the choice reads *"Make amends... but you have neither the gold nor the influence for it."* and does nothing. | Gets back **half** of what you lost (rounded up). |
| *"Let it be. Words would only make it worse."* | Nothing | The relation stays where the event left it. |
| *"Answer in kind, and make sure the whole realm hears of it."* | Nothing | You lose **another half** of the loss, and the other clan loses **10 renown**. |

Example: an insult at table costs you −12 with a tier 4 clan. Making amends costs 8,000 denars and brings you back 6 points, to −6 overall. Answering back takes you to −18, and they lose 10 renown.

### After a good event

| Choice | Cost | Effect |
|---|---|---|
| *"Take it in the spirit it was meant."* | Nothing | The relation stays where the event left it. |
| *"Return the kindness with a gift of X denars."* | **1,000 denars × the other clan's tier**, paid to their leader. If you do not have it, the choice reads *"Return the kindness... but you cannot spare X denars."* and does nothing. | Adds **another half** of the gain (rounded up). |

The +60 / −60 cap only limits the event itself, not your answer.

## Tips

- Your neighbours matter most: they are picked twice as often, for better or worse.
- Making amends with a powerful clan costs more (higher tier), but a lord with Clan Strength of 1,000 or more and a grudge against the ruler is exactly the kind who starts plots. Keep them sweet if you rule, and keep them close if you plan to plot.
- Answering back is free and hurts their renown, but it makes the quarrel half as bad again.

## Turn it off

In the settings file, set `ClanEventsEnabled` to `false`: no more events between clans. See [Settings](../settings.md).
