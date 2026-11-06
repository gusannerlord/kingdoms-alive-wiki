# Sparring with nobles (very soon in 2.0.0)

In peacetime the nobles of your realm take up the blunted practice blades together. A lord who likes you may invite you to a bout in the castle yard or on the sand of a town's arena, and you can ask any noble of your realm who is there. You learn, you make friends, and sometimes a purse changes hands.

## When and where
- Only in peace: while your realm is at war with another kingdom, nobody spars. Nor does anyone whose house is at feud, who rides with an army, is bound for a hunt or has a feast of their own to see to, is wounded, too old or with child.
- Only nobles of the same realm, in the same castle (its courtyard) or town (its arena). Not while a tournament holds the arena, not at night, not with an enemy at the walls.
- At most one bout a day for you, and one every 30 days with the same noble, whoever asked.

## Being invited
Each morning you spend in the same place as a lord of your realm, that lord may invite you: about 1 in 4 if they like you (relation 10 or more), far less if they only tolerate you, hardly ever if they dislike you. Brave lords ask more often. A lord sends at most one invitation every 30 days, to you or anyone else. The invitation comes in a window with their words ("Onto the sand" / "Into the yard" or "Not today"), and stays in the town or castle menu for the rest of the day as "Answer ...'s invitation to the arena" or "... to the yard".

## Asking
- From the castle or arena menu: **Look for a sparring partner (Practice blades)**. You see every noble of your realm who is there; those who cannot spar now are greyed out with the reason.
- In conversation: "Would you take up the practice blades with me? (Practice blades)". The line is hidden when the rules do not allow a bout.

The lord answers in their own voice. Good regard and Valor make a yes likelier, a calculating nature less likely; a request from the ruler is almost never refused. A yes in conversation leaves an option in the menu that day to go to the yard or the arena.

## The bout
- On foot, blunted steel, the best of three falls. A side falls when its leader is brought low; nobody leaves the bout with a wound on the map.
- Only weapons for both hands, from the game's practice rack: Sparring Twohander, Sparring Two Handed Axe, Sparring Billhook, Sparring Glaive and Sparring Menavlion. You choose yours (the window shows your skill for each).
- The lord takes their own, by their better skill and their people: a two-handed sword (an axe in Sturgia and the north, either in Battania), or for a polearm fighter the Billhook in Vlandia, the Menavlion in the Empire and the Glaive elsewhere.
- Two against two, about 1 time in 3, when both sides have a second: for you, a companion or family member with you (you choose); for the lord, one of their house or one of their landed knights, an adult no older than 45 who knows Two Handed or Polearm.
- Walking off before the end ("Yield the bout") counts as yielding, and everyone will hear of it.

## What it gives
- **Weapon experience**, as the game gives for knocking that opponent down once in a tournament: the full amount for the winner, three quarters for the loser (half of that if you yield after blows, nothing if you yield at once), half of it for each second. Up to half again more against an opponent much more skilled than you.
- **Relation +2** between you, but never above 30 from sparring. Nothing if you yield, or if the bout was won with too many kicks against an honourable opponent.
- **A memory**: the lord brings up the bout for a while afterwards (see [Lords who remember you](memories.md)).
- The noble with the most wins in a realm (at least 4, and two of every three bouts won) becomes known as the court's good blade. If that is you, brave lords invite you more often, and the invitations say so.

## Wagers
A bout may carry a wager, paid to the winner: 1,000 denars with a lord of modest means, 2,000 with a rich one, 3,000 with a very rich one. You can offer one when you ask, and a brave or proud lord sometimes proposes one. A lord only takes or offers a wager when they like their chances; a shrewd one needs better odds. Yielding hands the wager to your opponent.

## The AI spars too
Lords of the AI spar among themselves under the same rules, with no scene: the winner is decided by skill and level. They spar less often than with you (each lord waits 60 days between bouts, the same two 120 days), and less often still when one of them is a woman. Their bouts give them the same experience, relation, wagers and memories.

## Turn it off
In the settings file (see [Settings](../settings.md)):
- `NobleSparringEnabled` to `false`: no sparring at all.
- `NobleSparringAiEnabled` to `false`: AI lords no longer spar among themselves.
- `NobleSparringWagersEnabled` to `false`: no wagers.
