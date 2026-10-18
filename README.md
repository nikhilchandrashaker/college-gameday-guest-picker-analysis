# Are College GameDay Guest Pickers Any Good?

An analysis of 2,554 graded College GameDay guest picks (2004–2026) asking whether guest pickers beat chance and who the best of all time is.

## Headline results

- Guests picked the winner **61.47%** of the time (1,570 wins, 984 losses, 220 guests).
- Best records with 25+ picks: Joe Namath and Joel McHale, 21 of 31 (67.7%). Every leader's 95% interval includes the group average.
- Steve Young's 10-for-10 had a 0.77% chance (about 1 in 130) under a simple model. Two of 75 ten-pick appearances were perfect (Bubba Watson 2013, Steve Young 2026); luck predicts about 0.6.
- 13 of 220 guests fall outside the 95% luck funnel; chance predicts about 11. No trend by season; repeat guests do not improve.
- Not tested: guests versus betting favorites (needs point spreads), former athletes, school loyalty.

## Files

| File | What it is |
| --- | --- |
| `GameDay_Guest_Pickers_Research_Paper.pdf` | The paper: abstract, methods, results, limitations, conclusion, sources |
| `Celebrity_GameDay_Guest_Picker_Dataset_filled.xlsx` | Game-by-game dataset (2,554 rows), per-guest summary, Read Me sheet |
| `diagrams/1_leaderboard_25_picks.png` | Win % with 95% range, guests with 25+ picks |
| `diagrams/2_steve_young_perfect_appearance.png` | Ten-pick appearances against the luck-only expectation |
| `diagrams/3_skill_vs_luck_funnel.png` | Every guest against the 95% luck funnel |
| Interactive page (published artifact) | The same three exhibits in ESPN College GameDay red, black and white |

## Definitions

- **Season:** football season; January bowl games belong to the prior season.
- **Appearance:** one guest in one season and week label (numbered weeks, `B` bowls, `FCS`, week 0).
- **Perfect appearance:** 8 or more picks, all correct. Partial appearances with 1 to 5 recorded picks are not counted.
- **Win %:** correct picks divided by graded picks. Intervals are Wilson 95%.

## Method notes

- Luck model: each pick is an independent 61.47% event. Binomial tail probabilities, a chi-square dispersion test (guests with 25+ picks), and a simulation for the expected number of perfect slates.
- Row-level data reproduces the archive aggregate exactly (1,570–984).
- No guest has more than 45 recorded picks, so 50- and 100-pick thresholds are empty; the paper uses 25, 20 and 15.

## Data caveats

- Some older appearances lack complete picks (for example Charles Barkley 2004, Kenny Chesney 2008). Missing games were not invented.
- Joel McHale's official 2023 record differs from the picks the archive could identify.
- Dates are as shown in the archive; Steve Young's last pick is dated 2026-10-16 and his other nine 2026-10-17.

## Source

Cole's Gameday Blog, archival picks: https://gamedaycole.com/archival-picks/ (as of 2026-10-18).
