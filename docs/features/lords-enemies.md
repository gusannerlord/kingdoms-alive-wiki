# The Blackhand's knives

Somebody has paid the Blackhand Company to hurt the one you serve. Killers wait in a hall, an alley, an arena, a village or a tavern, and you are sent to deal with them. Each job is a short fight in a real scene of the game, on foot, against some of the hardest men for hire in Calradia.

## Who sends you

Two people can give you this work:

- **Your lord, while you are their [squire](squire.md):** one of their errands, *"the lord's enemies"*. The killers are paid by a noble house whose head your lord hates (a house of a kingdom at war with theirs counts as more hateful still). Your lord must have a real enemy for this errand to come up.
- **Your ruler, while you are their vassal:** one of the [affairs of your kingdom](realm-affairs.md#the-enemies-of-the-crown), *"The enemies of the crown"*. The killers are paid by a rival crown: a kingdom whose ruler is on bad terms with yours, or one that made peace with your realm in the last 120 days. Here the "lord" in everything below is your ruler, and the hall is a hall of the ruler's own house.

Only one Blackhand job runs at a time. Each one is a journal entry with where to go and how many days you have. The place, and anyone you must find, are marked on your map.

## The killers

They are men of the [Blackhand Company](free-companies.md), the axemen who hire out as a whole company in the taverns: Blackhand Reavers and Headsmen with great axes, Blackhand Ironwalls with axe and shield. Their champions are captains with names of their own (Hrolf Nine-Fingers, Grimar Widowmaker, Arnulf Stonejaw...).

## The five ways

The job takes one of five shapes, picked at random among those that fit where you are.

### Knives in the hall

*"Knives in the hall of {place}"*. Your lord will not hide behind their walls: they ride to one of their castles or towns and sit in the hall to wait for the killers. **Only in peacetime.**

- Your lord's arrow shows the way. When they get there you are told: *"{lord} has reached {place} and sits in her/his hall. Go to the lord's hall when you get there."*
- Your lord **stays there** until it is done (as long as the ride plus 5 days, at most 12). They are let go with no blame on you if war breaks out, they are called to a host, their men run short of food, they are taken, or the place changes hands.
- Enter the town or castle and go to the **lord's hall**. The servants are no servants: **3 or 4 killers** draw axes from under their aprons. You fight beside your lord and **3 of their guards**, with up to **2 of your companions** if they walk in with you. If you came unarmed, you find a sword in your hand.
- **If your lord is cut down**, they are carried off wounded. There is a small chance (**1 in 20**) that they die of it. If they die after you won, the job still counts as done.

### A letter or a purse

*"A letter for {notable}"* or *"A purse for {notable}"*. Carry it to a merchant or craftsman of a nearby town and hand it over yourself: **"I come from {lord}, with {what} for you."**

- At the gate of the town, a ragged boy or a beggar warns you that Blackhand men wait in the lanes. You choose:
    - **"Through the lanes"**: a street fight with **2 or 3 of your best men** against **3 or 4** Blackhand men. Win, then find the notable.
    - **"The long way round"**: no fight, but your lord hears that the Blackhand still swagger in those lanes. Done the lesser way.
    - **"Another day"**: come back later (or once you have healed: you cannot fight wounded).
- Lose the fight and the letter or the purse is gone with them: the job fails.

### The champion

*"The Blackhand's champion at {town}"*. A Blackhand captain, bought to call your lord a coward from the arena, waits on the sand.

- In the town menu, choose **"Meet {champion} on the sand"**. One against one, on foot, with real steel, until one of you is knocked senseless. Nobody dies. He is tougher than an ordinary man.
- Not at night, not while a tournament holds the arena, not in disguise and not while you are wounded.
- **Win** and his crew leaves your lord's lands. **Lose** and it still counts as done, the lesser way: he had his fight and moves on.

### Blackhand men in a village

*"Blackhand men at {village}"*. A crew squeezes one of your lord's villages for coin and grain.

- Ride there, choose to take a walk in the village and find their leader among his men. He offers you a deal. Your answers:
    - **"Here is 1000. Take it, and be gone from these lands."** They leave. Done the lesser way.
    - **"Look at my men, and count your own. Leave now, while you still can."** A threat. The odds rest on the better of your **Roguery** and **Leadership**: about 15% with no skill, 50% at 100, 65% at 150, never more than 85%. If he backs down, they leave and it counts in full. If not, he draws.
    - **"Enough talk."** A fight.
- In a fight you have **5 of your best men** (and companions walking with you) against **5 or 6** of theirs. Lose and the crew goes on squeezing the village: the job fails.
- If raiders burn the village first, or it changes hands, the job lapses with no blame.

### A name for sale

*"A name for sale at {town}"*. A stranger in a town's tavern says he will sell the name of the house that pays the Blackhand, to you and nobody else. Here the house that pays is hidden until the end.

- Go to the tavern and find him: **"I am listening. Who pays the Blackhand?"** It is a trap: **3 or 4** men at the next tables draw on you. Up to **2 of your companions** walking with you in the town fight at your side.
- **Win** and the stranger, found shaking under a table, gives up the name. Your lord learns which house it was and thinks a good deal worse of its head (**−10**).
- Lose and the stranger is gone, and the name with him: the job fails.

## Time, rewards and blame

You have the ride there plus half of it again, plus **4 days**. The hall lasts as long as your lord waits there.

| | For your lord (squire) | For your ruler (vassal) |
|---|---|---|
| Done | **2,500** denars (a quarter more from a generous lord, a quarter less from a closefisted one), **+3** relation, a little renown | **4,000** denars, **+5** relation, **3 renown**, **10 influence** |
| Done the lesser way | half the gold, **+1** relation, half the renown | half the gold, renown and influence, no relation |
| Failed, or out of time | **−3** relation | **−3** relation |
| Refused | **−2** relation | **−2** relation |

**The lesser way** is buying the village crew off, taking the long way round, or losing to the champion.

For your lord, the job counts towards the **10 errands** of your squire service, whichever way it is done. It **lapses with no blame** when it can no longer be done through no fault of yours: you were a prisoner when time ran out, the place is under siege or at war with you, the notable is gone, a tournament outlasted the champion, your lord or ruler died, or (for your ruler) you are no longer their vassal.

## Turn it off

In the settings file (see [Settings](../settings.md)):

- `SquireEnemies`: your lord never sends you after the Blackhand.
- `RealmAffairEnemies`: your ruler never does.
- `EnemiesHall`, `EnemiesAlley`, `EnemiesChampion`, `EnemiesVillage`, `EnemiesTavern`: each of the five ways, for both.
