# Fast mode families

In fast mode the years fly, but the base game does not let AI lords marry and have children any faster, so noble houses thin out generation after generation. The mod lets AI lords marry and have children at a pace that fits the short year, so Calradia's great families carry on for as long as you play.

## What fast mode is
Fast mode is chosen when you start a campaign. In the base game it changes three things: a year lasts **24 days** instead of 84, a pregnancy takes 18 days instead of 36, and skills need less experience per level.

## The base-game problem
The daily chance that two AI lords marry, or that a married couple conceives, is the same in both modes. A year of life passes 3.5 times faster in fast mode, so each lord gets 3.5 times fewer chances per year of age. A woman's fertile years (18 to 45) shrink from about 2,270 days to about 650. Many lords die single, couples have fewer children, and houses with no heir disappear.

## What the mod changes (fast mode only)
These changes apply only in fast mode campaigns, and only to AI lords. Nobody of your clan is affected, and the marriage offers that AI clans make to your clan stay as in the base game.

### More marriages
- In the base game, each year over 18 makes a lord 2% likelier to marry. With the mod it is **10% per year**, for each of the two.
- On top of that, every AI match is **3 times as likely**.

How much likelier a couple of the same age is to marry than in the base game:

| Age of both | 18 | 25 | 30 | 40 | 50 |
|---|---|---|---|---|---|
| Times the base game's chance | x3 | x6.7 | x9.4 | x14.8 | x19.7 |

So young lords marry a little sooner, and older bachelors and widowers much sooner.

### The older-woman rule
More marriages should mean more children, not men who could still father children tied to wives who can no longer bear them. When the man is **under 60**:

- from the woman's age of **38**, her extra chance fades away in a straight line;
- from **45** on, the match is very unlikely: one twentieth of the base game's chance.

Men of 60 or more marry women of any age as freely as anyone else, so old widows and widowers still pair up.

### More children
In the base game, an AI husband and wife who are in different places "meet" on 20% of days, and only then can she conceive. With the mod they meet on **30%** of days, so couples who are apart conceive half as often again. Couples who are together, the base game's limits on large families, and your own family are unchanged.

## The result: a 63-year test
A fast mode campaign was run for 63 years of game time, with the AI on its own:

- **81 of the 82 noble clans survived.** The only one lost had three daughters, all married into other houses (children belong to the father's clan), and no son.
- **791 marriages and 1,707 births.** Lord parties grew from 218 to 255.
- Couples where the bride was under 38, married for 15 years or more, had **about 2.66 children** on average (about 3 if she married at 18 to 22, about 1.6 if at 33 to 37). That is above the 2 needed for every generation to replace the last.
- Births per 5 years: about 100 to 130 in the first 15 years, a dip to about 95 between years 16 and 30 (the lords alive at the start were all married off, and the children born in the campaign were not grown up yet), then rising to 140 to 190 for the rest of the campaign.
- No woman of 45 or more married a man under 60.

## Children's culture (all modes)
In the base game, a child of two parents takes the father's or the mother's culture at a coin flip. With the mod, it takes the **father's culture 9 times in 10**. The child's name and clothes follow that culture. Since the child also belongs to the father's clan, houses keep their culture over the generations instead of drifting at random.

- Applies in **normal and fast mode** alike.
- Applies to every child whose parents are both not you, including children born in your own clan to your relatives (companions never marry, so they have no children).
- **Your own children** always take your culture, as in the base game.
- Measured in the 63-year test: 1,047 of 1,157 children of mixed-culture parents took the father's culture (90.5%).

## Turn it off
In the settings file, set the switch to `false`. See [Settings](../settings.md).

- `FastModeMarriagesEnabled`: AI lords marry at the base game's pace in fast mode (also turns off the older-woman rule).
- `FastModeChildrenEnabled`: AI couples have children at the base game's pace in fast mode.
- `ChildCultureEnabled`: children take the father's or the mother's culture at a coin flip again.
