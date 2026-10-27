# Command your armies

Your realm now has someone at the head of its armies: the **Marshal** of the [royal court](royal-court.md). As ruler, you give your war aims to your Marshal and they carry them to the lords. As a vassal, you can be that Marshal yourself, take your liege's orders and see them done. Orders go by word of mouth or by riders who find the lords wherever they are, and every lord answers in their own voice.

A second part, **Smarter warlords**, changes how AI lords wage war. It is **off by default**: see [below](#smarter-warlords-off-by-default).

## One Marshal

- The Marshal of the court is the one who leads the realm's armies. The Court tab says so: *"The Marshal leads the realm's armies in the field. The ruler's orders for the war go to the Marshal, who carries them to the lords and sees them done..."*
- A Marshal who is a captive, in hiding or away on another duty keeps the office but gives no orders until they are back.
- Orders exist only in your own realm: when you rule it, or when you are its Marshal. Elsewhere, the armies wage war as the AI decides.
- Mercenaries cannot be Marshal.
- Any lord of your realm can ask the ruler *"Who leads the realm's armies, and to what end?"*, and hear who the Marshal is and what they have been sent to do.

!!! note "With the court's offices switched off"
    If `CourtOfficesEnabled` is off, the realm has a Marshal of its own instead, always the head of a house. AI rulers name one and look again once a year, keeping the one they have unless another is clearly better. As ruler, you name yours by saying *"I would have you serve as Marshal of the realm."* (they accept unless they dislike you) or by rider.

## As ruler

### Orders for the Marshal

Talk to your Marshal and say *"Marshal, I have orders for you."* (a Marshal of your own family or a companion hears it the same way). The window **Orders for the Marshal** offers:

- **Take a fortress of the enemy.** Only enemy towns and castles on your border are listed, nearest to the Marshal first.
- **Hold one of our fortresses.**
- **No orders: act as you judge best.** Ends the current order.
- **Orders for one of the realm's armies, through the Marshal.** See [below](#orders-to-one-army).

There is one aim for the whole realm at a time. A new order replaces the old one.

- **Take:** the Marshal's army and every army of the realm make the place their first aim. It is a strong pull, not a leash: they still march where the war lets them.
- **Hold, while no enemy is near it:** the Marshal keeps watch. Their army takes no new siege far from the place (more than about a day and a half's march) and patrols it and its villages, and so do the lords riding alone near it.
- **Hold, when the enemy comes:** *"My liege, the enemy has come against {PLACE}. I bid the realm's armies to its relief, all but those you have sent elsewhere."* If the enemy host is stronger than the Marshal's army, the Marshal says so and waits for more lords to come up.

An order ends when the place is taken, holds, falls, is lost some other way, or after **10 days**. The Marshal reports each step: the siege begun, the place taken, the place lost (*"My liege, {PLACE} has fallen. We could not save it. I am sorry."*).

**When the Marshal holds back**, they tell you why, and only the real reason: the enemy hosts around the place are stronger than anything they can gather (*"My liege, {PLACE} is too well covered..."*), or simply that other needs came first. A Marshal who is taken captive or away leaves your order waiting; you are told, and a new Marshal takes it up.

### Orders to one army

Through your Marshal, pick any army of the realm in the field (*"{LEADER}'s army, {MEN} strong, near {PLACE}"*) and tell it what to do. Your Marshal sends a rider with your word. The orders are:

| Order | What the army does |
|---|---|
| **Besiege a fortress of the enemy** | Makes for it and lays siege. Only places on your border that it can reach; a leader asked for one deep in enemy lands says *"{PLACE} lies beyond our reach, deep in their lands..."* |
| **Stand guard over one of our fortresses** | Goes to it and stands at its gate. Lays no sieges and relieves no other place, rides to defend its villages when they are raided (unless the raiders are stronger), and does not chase enemy armies far from it. An army with less than about 6 days of food goes for food first. |
| **Break off and ride back to our lands** | Leaves any siege and rides to the nearest of your towns and castles. |

A new order replaces any the army holds. Your own orders are always taken up.

**Ignoring an order.** A leader who takes up an order and then goes their own way loses **5** relation with you: an army that never marches on the place it was to besiege within 10 days, one that leaves the place it guards for more than a day, one that is not home in good time. Hours spent fighting, fleeing or facing a stronger host do not count against them. A leader who judges the road too dangerous says so and is not blamed: *"{LEADER} judged the road to {PLACE} too dangerous for her/his army, and held back. There is no shame in that."*

## As a vassal: the Marshal

### Becoming Marshal

- An AI ruler may offer you the office like any other, with the letter **"An office at court"** (see [The royal court](royal-court.md#ai-rulers-and-their-courts)). Once named, the ruler tells you in their own voice, for example *"You are Marshal of {REALM}. My orders will come to you, and you will pass them to the lords."*
- Or ask for it. Talk to your ruler: *"My liege, let me lead the realm's armies as your Marshal."* They grant it if there is no Marshal, if the Marshal is a captive, or if you stand higher than the one who holds it. Your house's tier counts most, then how your ruler likes you, then your record as Marshal (orders carried out count for you, orders failed against you). If they say no, they say why: *"The great houses would not follow a lesser one..."*, *"... has my trust, and you have yet to earn as much."* or *"... Show me what you can do in the field, and we will speak again."* You cannot ask while you hold another office, or soon after being dismissed from one.
- Once you are Marshal, your ruler does not replace you with someone better suited. You lose the office only if you cannot serve (a captive, or away) for about a month, or if you leave the realm.

### The ruler's orders

When no order stands, your ruler gives you one, at most every 3 days: relieve the nearest of the realm's besieged fortresses or, if none is besieged, take the least defended of the enemy fortresses on the border near you (*"Marshal, our next aim is {PLACE}. Speak to the lords and lead them there."*, or, for a hard one, *"... It will not fall easily: gather enough lords before you march on it."*). The place is marked on your map.

Pass it on:

- **To a lord in person**, any lord of the realm leading their own party: *"As Marshal, I bring the king's command: {PLACE} is to be taken. Make for it with your men."* They take it up unless they dislike you (relation below −10): *"Marshal or not, I will not march at your word. Find someone else to run your errands."*
- **By rider** to several lords at once (see [Riders](#riders)).
- **By ordering an army.** As Marshal you can talk to any army's leader: *"As Marshal, I have orders for your army."* The same three orders as above. They take your own orders unless they dislike you (relation below −10); a leader who takes one up and ignores it loses 5 relation with you.

How your ruler judges it, after up to 10 days:

| Outcome | What it gives |
|---|---|
| Done, and you had a hand in it (you fought or marched there, passed the order to lords, or sent an army) | **+3** relation with your ruler, **+10** influence |
| Done by others alone | Nothing; *"Next time, lead."* |
| Lost, or nothing came of it, and you did nothing for it | **−3** relation with your ruler |

You are never blamed if you were a captive, if you rode in your ruler's own army, if you strove for it, or if the place fell before anyone could reach it.

## Riders

You do not have to chase lords across the map. Riders go **twice as fast as a lord's party** and find the lord wherever the road has taken them. The answer is the one you would hear face to face, and you hear it when the rider arrives. If the lord has died, been captured or left the realm, the rider comes back and tells you.

- **From a town or castle of your realm**: choose **"Send a rider with the realm's word"** in its menu. Not while the place is under siege.
- **From your own party, anywhere**: talk to a companion or family member riding with you and say *"Find me a rider. The realm's word must reach our lords."* The rider sets out from where you stand. Not at sea, and not from inside a besieged place.

The window **The realm's riders** offers, as ruler: *"Offer a lord the office of Marshal"* and *"Send orders to your Marshal"*. As Marshal: *"Carry the king's order for {PLACE} to the lords"* (pick as many lords as you like, nearest to the place first) and *"Send your orders to one of the realm's armies"*.

## Your liege explains the war

While you serve a realm you do not rule, as a vassal or a mercenary, your liege tells you how the war goes, in their own voice and with their portrait: when the realm is losing and turns to the defence, when it is all but beaten, when it takes heart again or presses a beaten enemy. The leader of an army you ride in tells you when they turn to relieve one of your places. Each kind of news comes at most twice a day.

You can also ask your liege in person: *"My liege, what is our plan for this war?"*

## Smarter warlords (off by default)

This part changes how every AI lord and army wages war. It plays by the same rules as you: what a lord does depends on what they can see.

- **They see as you do.** In the base game a lord reacts only to what is within a short fixed distance, shorter than what you see by day, and scouting never helps. Now each lord sees what your party would see in their place: less at night and in forests, more with a good scout. An army sees with the eyes of every party riding in it, yours included.
- **They lift sieges they cannot win.** A besieger who sees a relief coming, or defenders too strong for them, lifts the siege instead of dying at the walls: once the danger outweighs the camp by about a tenth. A siege all but won (the garrison down to a fifth) is kept unless the danger is twice the camp. A camp that sees itself losing a battle at the walls breaks off and leaves; if you ride in an AI lord's army, you go with it. They do not start a siege they would lift at once, and they remember an enemy lord they saw ride into the place while that lord stays nearby.
- **They take refuge.** A lord fleeing a stronger host (they stand their ground from about 95% of its strength, a little less for a brave lord, a little more for a cautious one) rides into the nearest fortress of a friendly realm they can reach first, instead of running across the map. They stay inside while the host is in sight, and lay no siege it could reach until it is far, weaker or gone. Not your clan, and not lords riding in an army.
- **They hunt armies they can catch.** An AI army may ride at an enemy army it sees, when it is at least as strong and no more than twice as strong (stronger than that and the enemy would only run), and only if it can catch it within about 12 hours. Your army is fair game if you lead one, and so are armies still gathering and armies besieging a third realm.
- **A relief waits out of reach.** Lords riding to relieve a place gather about 4 hours' march from the besiegers' camp until they are strong enough, instead of right beside it. (Only on game version 1.5.5.)
- **They call more lords.** An AI army set on a siege or on relieving one of its places, but too weak for it, calls free lords within a day's ride, a few a day, paying the influence as you would. It never calls when its own men are below 70% of full strength (50% for a relief waiting out of reach).
- **The army leader tells you why.** Riding in an AI army, you hear from its leader why they lift a siege, break off a battle, ride at an enemy army or let one go. A line on screen tells you when a siege is lifted for fear of a relief and your realm is on either side.

### Is it for you?

Smarter AI can be annoying at times: enemy armies are harder to catch, and allied armies change their target more often. Think of playing against people who see as far as you do: they react to every move the enemy makes, and so do these lords. If you enjoy crushing an AI that throws its armies away, and have no patience for armies that change their minds, leave it off. Commanding your armies works either way.

### Switching it on

In the settings file (see [Settings](../settings.md)), set `PrudenceEnabled` to `true`, or tick **Smarter warlords** under **Mod Options > Kingdoms Alive** with Mod Configuration Menu. It applies the next time you start the game. Each piece can then be switched off on its own (see below).

## Turn it off

In the settings file (see [Settings](../settings.md)), set to `false`:

- `PrudenceRealmEnabled`: the whole realm's command (orders, orders to one army, riders, your liege's words). The Marshal of the court stays, with the court's own effect.
- `PrudenceOfficeEnabled`: the Marshal leads no armies: no orders, no orders to one army, no riders.
- `PrudenceArmyOrdersEnabled`: no orders to one army.
- `PrudenceRiderEnabled`: no riders (from towns and castles or from your party).
- `PrudenceFieldRiderEnabled`: no riders from your own party.
- `PrudenceMarshalEnabled`: your liege and army leaders do not explain the war.

Smarter warlords (`PrudenceEnabled`, off by default) and its pieces:

- `PrudenceNoticesEnabled`: the lines on screen about lifted sieges.
- `PrudenceSiegeRetreatEnabled`: lifting lost sieges (and with it the three below).
- `PrudenceWithdrawEnabled`: breaking off a lost battle at the walls.
- `PrudenceStartSeenEnabled`: not starting a siege they would lift at once.
- `PrudenceRememberDefendersEnabled`: remembering lords seen riding into a place.
- `PrudenceRefugeEnabled`: taking refuge (and with it the two below).
- `PrudenceEarlyWarningEnabled`: seeing a stronger host coming from afar.
- `PrudenceWaitOutThreatEnabled`: waiting out the host they fled.
- `PrudenceHuntEnabled`: hunting enemy armies.
- `PrudenceHuntPlayerArmy`: your army as prey.
- `PrudenceHuntGatheringEnabled`: armies still gathering as prey.
- `PrudenceHuntBesiegersEnabled`: armies besieging a third realm as prey.
- `PrudenceReliefWaitEnabled`: the relief waiting out of reach.
- `PrudenceRallyEnabled`: calling more lords.
