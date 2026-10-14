# Duels

Make enough enemies and one of them will send you a glove. A duel is to the death: face them yourself in the arena, send someone of your house in your place, or refuse and let the realm talk.

## Who challenges you, and how often
- A clan whose leader stands at **-30 or worse** with you, and whose realm is not at war with you, can challenge you.
- The clan sends its **best or second best fighter**, chosen by melee skill, Athletics, armour and health.
- Never a king or queen, never your own blood (parents, children, brothers and sisters, spouse), and never someone who personally likes you.
- After a challenge, no other comes for **60 to 90 days**. Once that wait is over, there is a 1 in 20 chance each day while such a clan exists. Expect roughly one challenge every 100 to 200 days if you have bitter enemies, none if you have none. The first one cannot come before 10 days.

## The challenge
A window titled **"A challenge"** opens on the map: the challenger has *"sent you a glove and a message"*, names the arena, and warns that *"Whoever falls does not get up again."* You have three answers:

| Answer | What happens |
|---|---|
| **"Name the day. I will be there."** | You fight in person. The hint shows your rough chance to win. |
| **"Someone of my house will answer for me."** | You pick a champion in a second window, **"Who answers for you?"**, each with their chance to win. |
| **"I do not cross swords with the likes of you."** | You lose **75 renown** and **100 influence**. |

## Where and when
The duel is held in the arena of the challenger's ruler: their most prosperous town with an arena. If the ruling clan has none, the realm's most prosperous town; failing that, the town nearest you. Never a town at war with you.

If you fight in person, the arena town is marked on your map and you have **10 days** to get there. Once inside the town, the menu shows **"Go to the arena to meet {challenger}"**.

!!! warning
    Not turning up counts as refusing: the same 75 renown and 100 influence, and the challenger tells everyone who will listen.

## Fighting in person
- You fight **on foot**, each in your own battle gear, with **150 hit points** each, in the arena scene, the same kind of fight as the base game's "The Spy Party" quest.
- **If you win**, the challenger dies.
- **If you lose**, you wake up badly wounded (*"{challenger} spared you, which is somehow worse."*). You do not die.

### When you cannot fight
Every hour you could not fight moves the day back by an hour. That covers: the challenger is in a battle or a siege, the arena town is under siege, you are wounded, or you are a prisoner. While you are wounded or the challenger is in the field, the arena option is greyed out with the reason.

After **10 days** of such delays, or if you are a prisoner when the day comes, the duel is called off with no penalty: *"The duel with {challenger} will not take place."* It is also called off if the challenger dies, is captured, becomes a ruler, or your realms go to war.

## Sending a champion
- Any **companion or family member** who can fight: adult, not wounded, not a prisoner, not pregnant, not tied up in a quest.
- The duel is fought without you **3 to 5 days later**, settled by the two fighters' skill, armour and health. Equal fighters have even odds; one about 60 points "better" wins about 3 times in 4.
- **Whoever loses dies, your champion too**, even if they are family.
- If either of them is in a battle or a siege that day, the duel waits. If one of them cannot come at all, it does not take place.
- A champion cannot leave as an [envoy](envoys.md) until the duel is over.

## What winning and losing give

| Outcome | The loser | The loser's house | The winner's house | Between the two clan leaders |
|---|---|---|---|---|
| You or your champion win | Challenger dies | -50 renown, -50 influence | +100 renown | -15 relation |
| Your champion loses | Champion dies | -50 renown, -50 influence (yours) | +100 renown | -15 relation |
| You lose in person | You are badly wounded | -50 renown, -50 influence (yours) | +100 renown | no change |
| You refuse or do not come | — | -75 renown, -100 influence (yours) | — | no change |

Deaths in duels appear in the game's notifications and the encyclopedia as *"{name} died in a duel with {killer}."*

## Duels between AI lords
AI lords fight duels too:

- Between two clans of realms that are not at war with each other, whose leaders stand at **-50 or worse**.
- Each clan sends its best or second best fighter; **rulers never fight** (the next best fighter of their clan goes instead).
- A 1 in 100 chance each day for the whole map, and no more than one duel every 60 to 90 days. That is roughly 5 deaths every 1,000 days.
- The loser dies, with the same renown, influence and relation changes as above. The death shows up as news like any lord's, saying it was a duel.

## Turn it off
In the settings file, set the switch to `false`. See [Settings](../settings.md).

- `DuelsEnabled`: all duels, yours and the AI's.
- `AiDuelsEnabled`: only the duels between AI lords.

Two related switches are off by default: `DuelRulersCanChallengePlayer` (set to `true` to let kings and queens challenge you) and `AiDuelsCanKillRulers` (set to `true` to let rulers fight in AI duels).
