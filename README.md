# Schedule Compression and Performance in Basketball

## Overview

Teams don’t just win because they’re better—they also win because their schedule is easier.

This project analyzes how schedule compression—measured through travel distance, rest days, and game density—impacts team performance. Using game-level data, I estimate how scheduling factors influence win probability and how these effects accumulate over a season.

---

## Key Findings

- Back-to-back games reduce win probability by ~6.6%
- Opponent strength is the dominant driver of game outcomes
- Schedule effects are small at the game level but compound over a season
- Teams can gain or lose over 100 wins across a sample period due to scheduling differences
- Schedule advantages appear to amplify differences between strong and weak teams
---

## Methodology

- Constructed team schedules with game dates, locations, and travel distances
- Engineered schedule features:
  - Back-to-backs (B2B)
  - 4 games in 6 days (4-in-6)
  - Days of rest between games
- Estimated opponent strength using team net ratings
- Modeled game outcomes using a linear probability model:
  - Win ~ opponent strength + travel + rest + game density
- Aggregated predicted vs. actual outcomes to estimate schedule-driven wins

---

## Why This Matters

Schedule structure creates small but compounding competitive advantages.

While individual game effects are modest, they accumulate over time and can meaningfully impact season outcomes. These effects are especially relevant in tournament environments, where teams may be required to play multiple games in consecutive days.

This framework translates directly to college basketball, where conference tournament structures and bye allocation can significantly influence competitive outcomes.

---

## Tools & Technologies

- R (dplyr, ggplot2, lubridate)
- Data cleaning and feature engineering
- Linear modeling and statistical analysis

---
