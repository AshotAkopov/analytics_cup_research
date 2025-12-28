# Phase-Dependent Physical Profiles in Football
### SkillCorner × PySport Analytics Cup – Research Track

This repository is intended for evaluation as part of the SkillCorner × PySport Analytics Cup. The `submission.ipynb` notebook represents the full research submission.

## Introduction

Physical performance in football is inherently phase-dependent, as players are exposed to distinct tactical and physiological demands when their team is in possession (TIP) versus out of possession (OTIP). While previous studies have described overall physical outputs, fewer have quantified how individual players adapt their physical profiles across game phases, and how these adaptations differ by position. Using season-level physical aggregates from the 2024/25 Australian A-League, this study proposes a novel framework to characterize and quantify phase-dependent physical adaptations at both the player and positional levels.

## Methods

Season-long physical aggregates were collected for all midfielders and attacking players across 175 matches. After normalizing physical metrics by minutes played, a Principal Component Analysis (PCA) was applied to standardized physical features to derive a low-dimensional representation of player physical profiles. The first two principal components captured the dominant axes of physical variation, broadly reflecting intensity-related actions and running-volume trade-offs.

To assess phase dependency, separate PCA projections were computed for in-possession (TIP) and out-of-possession (OTIP) phases using a shared PCA space fitted on full-match data. For each player, a Possession Shift Index (PSI) was defined as the Euclidean distance between their TIP and OTIP coordinates in the PC1–PC2 space, quantifying the magnitude of physical adaptation between phases. Directional changes were further analyzed using component-wise differences (dPC1, dPC2), enabling classification of shift types and aggregation by playing position.

## Results

The analysis revealed substantial inter-individual variability in phase-dependent physical adaptations. While some players exhibited minimal shifts between TIP and OTIP, others demonstrated pronounced changes in both magnitude and direction, as reflected by high PSI values. At the positional level, central defenders and midfielders displayed the largest average PSI, indicating strong adaptation to out-of-possession physical demands, whereas forwards and wide attackers showed more balanced or possession-oriented profiles.

Directional analyses highlighted clear positional trends: defensive roles predominantly shifted toward OTIP-dominated profiles, while attacking roles exhibited mixed or TIP-oriented adaptations. Importantly, within-team variability exceeded between-team differences, suggesting that physical adaptation is primarily structured by individual roles rather than collective team identity.

## Conclusion

This study introduces the Possession Shift Index as a simple yet powerful metric to quantify phase-dependent physical adaptations in football. By embedding physical performance within a shared PCA space, the approach captures both the magnitude and direction of player-specific adaptations across game phases. The findings underline the importance of considering possession context when evaluating physical performance and highlight strong positional signatures in phase dependency. This framework offers practical applications for performance profiling, role-specific conditioning, and tactical analysis in elite football.

## Repository structure

- `submission.ipynb` : Main submission notebook (runs end-to-end)
- `src/` (optional) : Utility functions used in the notebook
- `README.md` : Project overview

