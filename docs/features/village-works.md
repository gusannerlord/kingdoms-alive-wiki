# Works in a village

In the base game only towns and castles have buildings. With Kingdoms Alive, whoever holds a village may raise a few small works there: nothing grand, cheap and quick, each helping the village a little.

## Who builds

- The **landed knight** who holds the village; if none does, the **lord of its castle or town**.
- You and the AI follow the same rules. You build in your own village (as a landed knight) or in the villages of your towns and castles that no knight of yours holds.
- AI lords build too, now and then, when they would still have 80,000 denars left after paying.

## The works

| Work | Cost | Days | What it does |
|---|---|---|---|
| Well and Irrigation Ditches | 5,000 | 10 | +0.15 hearths per day. |
| Palisade and Watchtower | 6,500 | 15 | +0.5 militia per day, and raiders loot the village 20% more slowly. |
| Mill | 8,000 | 20 | +5% to the goods the village makes, so it has more to sell. |
| Storehouse | 4,000 | 10 | After a raid, +3% of the village mended each day on top of its own recovery: it is back on its feet 25 to 50% faster (more in a large realm, which recovers slowly; less in a small one). |

The hearths and the militia only grow while the village is not raided or looted, as in the base game.

A village raises one work at a time. Each can be raised once.

## How to build

Go to the village and choose **See to the works of the village (Village works)** in its menu. Its tooltip tells you what the village has and what is being raised.

The option opens a screen like the **Manage** screen of a town or castle: one card per work, with its picture. A raised work shows level I; the one under way carries the hammer and fills up as it progresses. Hover over a card to see, on the right, what the work does with its exact value, its cost and how many days it takes, or how many days are left. Click a card you can pay for and then the hammer to start it: the gold is paid at once, the villagers set to it, and word reaches you when it is finished. Clicking a card you cannot start tells you why (already raised, the men are busy on another work, the village must recover first, or you cannot pay for it). **Done** or Esc closes the screen.

The option only shows when there is something to see or to build. Nothing can be started while the village is being raided or still lies looted.

## Raids

A raid that loots the village stops the work under way (what was paid for it is lost), and one of the works already raised lies in ruins. You can raise it again once the village has recovered.

## Turn it off

In the [settings file](../settings.md), set `VillageWorksEnabled` to `false`.
