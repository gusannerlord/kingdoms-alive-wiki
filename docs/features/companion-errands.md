# Companion errands

Now and then a companion riding with you speaks up: word has reached them of something they must see to, and they ask for leave and a few men. Let them go and they come back days later with experience, sometimes gold or recruits, and the men who survived. Refuse and they will remember it.

## How often

- About **once every 80 to 120 days**, counted from the last errand's return or the last refusal.
- The first request comes **20 to 120 days** after you start using the mod.
- Only one companion is away at a time.

## Who asks, and when

The companion must be riding in your own party, unhurt, not pregnant and not busy with a quest. A companion who is your champion in a pending duel does not ask.

They only speak up while you are travelling on the map: not in a town, at sea, in a battle or siege, or in the middle of another conversation or event window.

Your party must have enough healthy troops to spare: what they ask for **plus 10 more**. Heroes and troops lent to you by a quest do not count.

## The conversation

The companion opens a conversation and explains the matter, how many days they need and how many men. You answer:

- *"Go, and take the {N} men you need."* They leave with everything they asked for.
- *"Go, but I can spare you only {N} men."* They leave with **half** the men. The errand is more likely to go wrong (see below).
- *"Then I am coming with you."* They thank you but say no: this is theirs to see to. You answer again.
- *"No. I need you here."* They stay and lose relation with you.

If the conversation is cut short before you answer, they ask again about 5 days later.

While they are away, the companion and their men are gone from your party.

## The six errands

The men asked for are a share of your healthy troops, with a minimum, and **never more than 40**. The men are picked at random from your troops, elites included.

| Errand | Days | Men asked | Can go wrong | Losses (if it goes well) | Skill trained | Relation: let go / refused |
|---|---|---|---|---|---|---|
| A dying father | 6–9 | 5% (at least 4) | Never | None | Charm, 900 xp | +6 / -6 |
| Outlaws above their village | 7–10 | 15% (at least 8) | 15% | 10–30% | Tactics, 1,600 xp | +5 / -5 |
| An old comrade's debt | 8–12 | 10% (at least 6) | 10% | 5–20% | Leadership, 1,400 xp | +5 / -5 |
| A merchant selling out | 10–14 | 8% (at least 5) | 20% | Up to 5% | Trade, 1,500 xp | +3 / -2 |
| A buried hoard | 7–10 | 12% (at least 6) | 25% | 10–30% | Scouting, 1,500 xp | +4 / -3 |
| A kidnapped nephew | 8–12 | 18% (at least 10) | 20% | 15–35% | Roguery, 1,800 xp | +7 / -7 |

**Extra rewards when it goes well:**

- **A merchant selling out:** your share is **4,000 to 12,000 denars**.
- **A buried hoard:** your half is **3,000 to 9,000 denars**.
- Both gold rewards grow with your clan tier (**+30% per tier**: at tier 3 the hoard pays 5,700 to 17,100).
- **An old comrade's debt:** **4 times in 10**, **3 to 6 veteran soldiers** of the companion's culture come back to join you. They are high-tier noble troops, such as Vlandian Knights or Khuzait Torguud.

## When it goes wrong

The chance in the table is for when you give all the men asked for. With half the men, it is **doubled**, and losses are **1.5 times** as heavy.

When an errand goes wrong:

- No gold and no veterans.
- The companion gets **half** the experience.
- In every errand except the merchant deal, there was a fight: the companion comes back **badly wounded** (never killed) and losses are **doubled**.
- The merchant deal that goes wrong just means empty saddlebags. Nobody is hurt.
- No errand ever costs more than 80% of the men sent.

## Coming back

When the days are up, the companion and the surviving men rejoin your party with a message telling what happened.

- **If you are a prisoner, in a battle or at sea**, they wait and rejoin once you are free, out of the fight or back on land (or in a port).
- If the companion dies of old age while away, or is no longer one of your companions, the men come back without them and a message tells you why.

!!! warning
    Do not start a War Sails story quest while a companion is away on an errand. If the errand ends during it, the men can be lost and the companion left without a party.

## Turn it off

In the settings file (see [Settings](../settings.md)), set `CompanionErrandsEnabled` to `false`. Nobody asks again, but a companion already away still comes back.
