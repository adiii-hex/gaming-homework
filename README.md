# 🚀 Martian Scout Alien Expedition 👽

## Overview

Martian Scout Alien Expedition is a creature-collecting game that runs inside a Jupyter notebook. You play a Cub Scout on Mars: explore real Martian locations, scan alien creatures into your Field Journal, earn merit badges, and climb five scout ranks. Each rank-up plays a new celebration song written by Google's Lyria music AI.

- **41 creatures** across Martian craters, volcanoes, canyons and polar caps, each with a type, rarity, danger level and scout tip
- **5 ranks** that unlock new places and creatures as you earn XP
- **Merit badges** earned by scanning creatures from each badge group
- **AI rank-up songs** that play once while the game pauses
- **A hidden mythic creature** that only appears once you reach the top rank

## How to play

Each turn you pick a place, explore it, and try to scan what you find. The game panel shows these four steps under the title.

1. **Pick a place** from the **Go to:** dropdown. It lists only places your rank has unlocked.
2. **Press Explore!** You see the location's temperature, radiation, dust storm risk and ice. Places with a higher storm risk are more likely to send you back to the rover before you find anything.
3. **Press Scan** when a creature appears. You get 3 tries. Each try succeeds at the creature's catch rate, so rare creatures are harder to scan. A creature you haven't scanned before is marked NEW.
4. **Earn XP** from every successful scan. Enough XP moves you up a rank and unlocks new places and creatures.

Press **Field Journal** at any time to see every creature you've scanned and the badges you've earned. The status bar shows your current rank, XP, the next rank's target, and how many of the 41 creatures you've found.

### Ranks

| Rank | XP needed | Creatures it unlocks |
| --- | --- | --- |
| Tiger | 0 | 4 |
| Wolf | 50 | 9 |
| Bear | 150 | 9 |
| Gryffin | 300 | 13 |
| Arrow of Light | 500 | 6 |

### Merit badges

Every creature belongs to a merit badge group. The first time you scan a creature from a group, you earn that badge.

### Rank-up songs

When you rank up, Lyria composes a short celebration song about your new rank and plays it once. Explore!, Field Journal and the dropdown are locked until the song has loaded and finished playing, about 30 seconds. If the song can't be made, the game shows why and carries on right away.

### The mythic creature

Once you reach Arrow of Light, every Explore! has a 3% chance of finding Areonyx, a mythic creature that roams all of Mars and appears on no map.

## Game rules

- **Dust storms:** each Explore! has a storm chance of the location's storm risk × 5%, so risk 10 means a 50% chance.
- **Which creature appears:** a random pick among unlocked creatures at that place, weighted by catch rate, so common creatures show up more often.
- **Scanning:** each of the 3 tries succeeds with a chance equal to the creature's catch rate.
- **Ranking up:** after every successful scan, the game moves you to the highest rank your XP allows. Jumping two ranks at once plays one song, for the higher rank.
- **Progress:** rank, XP, journal and badges are kept in memory while the notebook runs. Restarting the kernel starts a new game.
