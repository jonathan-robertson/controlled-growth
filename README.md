# Controlled Growth

[![🧪 Tested On](https://img.shields.io/badge/🧪%20Tested%20On-A20.6%20b9-blue.svg)](https://7daystodie.com/) [![📦 Automated Release](https://github.com/jonathan-robertson/controlled-growth/actions/workflows/release.yml/badge.svg)](https://github.com/jonathan-robertson/controlled-growth/actions/workflows/release.yml)

- [Controlled Growth](#controlled-growth)
  - [Summary](#summary)
  - [Reasoning](#reasoning)
  - [Adjustments](#adjustments)
    - [XP Multipliers](#xp-multipliers)
    - [Loot Stage Multipliers](#loot-stage-multipliers)
    - [Trader Quest Rewards](#trader-quest-rewards)
  - [Compatibility](#compatibility)

## Summary

7 Days to Die Modlet: Reduce loot stage bonus multipliers and certain xp gains for a more controlled growth experience.

TFP added a mechanic to support bonuses to Loot Stage while in more difficult biomes. While this originally sounded exciting (and to some degree, it was!), the fun wore off fairly quickly as players began receiving end-game gear in Tier 1 Wasteland after reaching level 100.

This is not the way to keep a game or server feeling fresh for multiple months, so I've finally adjusted these mechanics.

## Reasoning

I am personally *in favor* of loot bonuses when exploring more dangerous areas - *it only makes sense*, after all, since fewer survivors would explore these areas. **These adjustments should be carefully balanced against the added risk one is taking**, however... and after playing A20 for a long, long time, it's my opinion that the Wasteland does not justify a greater than 2.5x increase to Loot Stage.

Instead, I've opted for the changes listed below.

## Adjustments

### XP Multipliers

Type | Multiplier | Reasoning
--- | :---: | ---
Crafting | 0% | exploitable stack crafting
Selling | 0% | too powerful
Upgrading | 25% | very low risk, op xp option
Debug | 100% | type used when issuing admin commands
Harvesting | 100% | very low value, not exploitable, adds minor risk, encourages raw resource collection, noisy
Kill | 100% | provides high risk, noisy
Looting | 100% | very low value, not exploitable, adds risk
Max | 100% | not used in game
Other | 100% | covers minor, non-categorized xp types that do not appear to be exploitable
Party | 100% | not used in game
Quest | 100% | quests make the world go round
Repairing | 100% | no risk, but also extremely low value xp source

### Loot Stage Multipliers

Factor | Original | Adjusted
--- | :---: | :---:
apparelAviatorGoggles | 3,5.2 | 1,3
drugEyeKandy | 5 + 10% | 3 + 5%
perkLuckyLooter | 5-25% | 2-10%
Tier 1 POI | 3 + 5% | 2 + 2%
Tier 2 POI | 6 + 10% | 4 + 4%
Tier 3 POI | 9 + 15% | 6 + 6%
Tier 4 POI | 12 + 20% | 8 + 8%
Tier 5 POI | 15 + 25% | 10 + 10%
Forest | 0 + 0% | 25 - 80%
Desert | 10 + 50% | 25 - 60%
Burnt Forest | 10 + 50% | 25 - 60%
Snow | 20 + 100% | 25 - 40%
Wasteland | 30 + 150% | 25 - 20%

### Trader Quest Rewards

All tools, weapons, and armor have been removed from trader quest reward lists and replaced with resource stacks.

This change is motivated by the realization that Trader reward gear (both tier and level) are informed solely by the tier of quest one completes.

In some ways, this approach makes sense and would be considered realistic... but in other ways, it further breaks the growth cycle by rewarding low level players with high tier gear far sooner than they would get access to it otherwise.

See the `loot.xml` file for more details.

## Compatibility

Setup | Works?
--- | ---
Local Game | Yes
Peer 2 Peer Game | Yes
Dedicated Server | Yes
