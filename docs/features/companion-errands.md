# Companion errands

Now and then a companion riding with you speaks up: word has reached them of something they must see to, and they ask for leave and a few men. Let them go and they come back days later with experience, sometimes gold or recruits, and the men who survived. Refuse and they will remember it.

## How often

- About **once every 80 to 120 days**, counted from the last errand's return or the last refusal.
- The first request comes **20 to 120 days** after you start using the mod.
- Only one companion is away at a time.

## Who asks, and when

The companion must be riding in your own party, unhurt and not busy with a quest. A companion who is your champion in a pending duel does not ask.

They only speak up while you are travelling on the map: not inside a town, castle or village, at sea, in a battle or siege, or in the middle of another conversation or event window.

Only healthy soldiers of **tier 2 or higher** count, and only they can go. Heroes, recruits of tier 1 and troops lent to you by a quest are left out. A companion never asks for more than **a third** of those soldiers, and always leaves you at least **10** of them. A small company early in the campaign is asked for a handful of men, or not asked at all: the smallest errand needs about 14 such soldiers in your party, the largest about 31.

## The conversation

The companion opens a conversation and explains the matter, how many days they need and how many men. You answer:

- *"Go. Pick the men you need from my company."* The game's troop screen for quests opens, as when you send a companion to settle a quest. Move the men who go: healthy soldiers of tier 2 or higher, no more than they asked for (*"{Companion} asked for {N} men, no more."*). As with the game's own quests, the men's wages for those days are paid when they leave.
    - All the men they asked for: they thank you and leave.
    - Fewer: *"Fewer than I would like. It will have to do, and I thank you for it."* They leave, but the errand is more likely to go wrong (see below).
    - Nobody: *"Without men I cannot go. What do you say?"* and you answer again.
- *"Then I am coming with you."* They thank you but say no: this is theirs to see to. You answer again.
- *"No. I need you here."* They stay and lose relation with you.

If the conversation is cut short before you answer, the men you picked go back to your party and the companion asks again about 5 days later.

While they are away, the companion and their men are gone from your party.

## In your quest log

When a companion leaves, the quest log gets an entry with the errand's name (for example *"Outlaws above {Companion}'s village"* or *"Buried plunder"*), who went, with how many men, and a **Return Days** bar that fills up until their return. It closes by itself when they come back, with the same news as the message.

## The six errands

The men asked for are a share of your healthy soldiers of tier 2 or higher, with a minimum, **never more than 40** and never more than a third of them. You choose which men go.

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

The chance in the table is for when you give all the men asked for. The fewer you give, the likelier it goes wrong and the heavier the losses: with half the men the chance is **doubled** and losses are **1.5 times** as heavy; with only a man or two, close to **three times** as likely, with losses close to **twice** as heavy.

When an errand goes wrong:

- No gold and no veterans.
- The companion gets **half** the experience.
- In every errand except the merchant deal, there was a fight: the companion comes back **badly wounded** (never killed) and losses are **doubled**.
- The merchant deal that goes wrong just means empty saddlebags: the companion comes back unhurt, and losses are no heavier than usual (up to 5% of the men).
- No errand ever costs more than 80% of the men sent.

## Coming back

When the days are up, the companion and the surviving men rejoin your party with a message telling what happened.

- **If you are a prisoner, in a battle or at sea**, they wait and rejoin once you are free, out of the fight or back on land (or in a port).
- If the companion dies of old age while away, the men come back without them and a message tells you.

!!! warning
    Do not start a War Sails story quest while a companion is away on an errand. If the errand ends during it, the men can be lost and the companion left without a party.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `CompanionErrandsEnabled` to `false`: nobody asks again, but a companion already away still comes back.
- `AwayQuestLogEnabled` to `false`: no new quest log entries for those you send away (this also covers affairs of your kingdom you hand to someone). Entries already open still close.
