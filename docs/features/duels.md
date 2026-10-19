# Duels

A duel is to the death: face your enemy yourself in the arena, send someone of your house in your place, or refuse and let the realm talk. AI lords who loathe each other settle their quarrels the same way.

## Who challenges you
Only **[your rival](rival.md)**. A duel in the arena is always the last step of a rivalry, and your rival always fights it in person. The rival page explains when it comes and what winning or losing it means.

Houses that hate you **no longer challenge you on their own**. That is off by default; you can turn it back on with `DuelPlayerChallengesEnabled` (see [Challenges from houses that hate you](#challenges-from-houses-that-hate-you) below).

## The challenge
A window titled **"A challenge"** opens on the map. It names the arena and tells you what is at stake. You have three answers:

| Answer | What happens |
|---|---|
| **"Name the day. I will be there."** | You fight in person. The hint shows your rough chance to win. |
| **"Someone of my house will answer for me."** | You pick a champion in a second window, **"Who answers for you?"**, each with their chance to win. |
| **"I do not cross swords with the likes of you."** | You refuse. Your rival's price: **25 renown**, no influence, and they challenge you again 30 days later. |

## Where and when
The duel is held in the arena of the challenger's ruler: their most prosperous town with an arena. If the ruling clan has none, the realm's most prosperous town; failing that, the town nearest you. Never a town at war with you.

If you fight in person, the arena town is marked on your map and you have **10 days** to get there. Once inside the town, the menu shows **"Go to the arena to meet {challenger}"**.

Once you agree to fight, in person or by a champion, the duel has its own entry in your quest log: *"A duel with {challenger} at {town}"*, or *"The reckoning with {challenger} at {town}"* for your rival's. It names the arena town. If that arena can no longer be used because its lords go to war with you, the duel is not called off: it **moves to another arena**, chosen the same way, and the entry tells you where. A siege of the town only holds the duel back, as below.

!!! warning
    Not turning up counts as refusing, and the challenger tells everyone who will listen.

## Fighting in person
- You fight **on foot**, each in your own battle gear, with **150 hit points** each, in the arena scene, the same kind of fight as the base game's "The Spy Party" quest.
- **If you win**, the challenger dies.
- **If you lose**, you wake up badly wounded (*"{challenger} spared you, which is somehow worse."*). You do not die.

### When you cannot fight
Every hour you could not fight moves the day back by an hour. That covers: the challenger is in a battle or a siege, the arena town is under siege, you are wounded, or you are a prisoner. While you are wounded or the challenger is in the field, the arena option is greyed out with the reason.

After **10 days** of such delays, or if you are a prisoner when the day comes, the duel is called off with no penalty: *"The duel with {challenger} will not take place."* If your realms go to war with each other, it is called off. Your rival does not give up: they challenge you again later, once there is peace.

## Sending a champion
- Any adult **companion or family member**, wherever they are, as long as they are not a prisoner, not away (as an envoy, on an errand or solving a quest), not tied up in a quest, and not pregnant (for women of your family). Being wounded does not stop them.
- The duel is fought without you **3 to 5 days later**, settled by the two fighters' best melee skill, Athletics, armour and health. Equal fighters have even odds; the choice window shows each candidate's chance against the challenger.
- **Whoever loses dies, your champion too**, even if they are family.
- If either of them is in a battle or a siege that day, the duel waits. If one of them cannot come at all, it does not take place.
- A champion cannot leave as an [envoy](envoys.md) until the duel is over.

Deaths in duels appear in the game's notifications and the encyclopedia as *"{name} died in a duel with {killer}."*

## Duels between AI lords
AI lords fight duels among themselves:

- Between two clans of realms that are not at war with each other, whose leaders stand at **-50 or worse**.
- Each clan sends its best or second best fighter, chosen by melee skill, Athletics, armour and health; **rulers never fight** (the next best fighter of their clan goes instead). Nor do a lord who is pregnant, anyone of your blood, or a lord riding in your army.
- A 1 in 100 chance each day for the whole map. If the two clans drawn have nobody free to fight (everyone is in a battle or a siege), another feuding pair is tried. After a duel, none for 60 to 90 days. That is roughly 5 deaths every 1,000 days.
- The loser dies. The loser's house loses **50 renown** and **50 influence**, the winner's gains **100 renown**, and the two clan leaders lose **15** relation with each other. The death shows up as news like any lord's, saying it was a duel.

## Challenges from houses that hate you
Off by default. If you set `DuelPlayerChallengesEnabled` to `true`, houses that hate you challenge you on their own, besides your rival:

- A clan whose leader stands at **-30 or worse** with you, and whose realm is not at war with you, can challenge you. Not your rival's house: your rival has their own duel.
- The clan sends its best or second best fighter. Never a king or queen, never your own blood (parents, children, brothers and sisters), never someone who personally likes you, never a lord who is pregnant, and never a lord riding in your army.
- After a challenge, no other comes for **60 to 90 days**. Once that wait is over, there is a 1 in 20 chance each day while such a clan exists: roughly one challenge every 80 to 110 days if you have bitter enemies. The first one cannot come before 10 days.
- The window reads *"{challenger} of the {clan} has sent you a glove and a message"* and warns that *"Whoever falls does not get up again."* Everything else (arena, champions, delays) works as above.

What these duels give:

| Outcome | The loser | The loser's house | The winner's house | Between the two clan leaders |
|---|---|---|---|---|
| You or your champion win | Challenger dies | -50 renown, -50 influence | +100 renown | -15 relation |
| Your champion loses | Champion dies | -50 renown, -50 influence (yours) | +100 renown | -15 relation |
| You lose in person | You are badly wounded | -50 renown, -50 influence (yours) | +100 renown | no change |
| You refuse or do not come | — | -75 renown, -100 influence (yours) | — | no change |

## Turn it off
In the settings file, set the switch to `false`. See [Settings](../settings.md).

- `DuelsEnabled`: the duels between AI lords, and the challenges from houses that hate you (if you turned those on). Your rival's duel has its own switch, `RivalDuelEnabled` (see [Your rival](rival.md)).
- `AiDuelsEnabled`: only the duels between AI lords.
- `DuelQuestLogEnabled`: no quest log entry for your duels, and a duel whose arena turns hostile is called off instead of moved.

Three related switches are off by default: `DuelPlayerChallengesEnabled` (set to `true` to let houses that hate you challenge you), `DuelRulersCanChallengePlayer` (set to `true` to let kings and queens challenge you) and `AiDuelsCanKillRulers` (set to `true` to let rulers fight in AI duels).
