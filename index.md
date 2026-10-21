---
layout: default
title: Liang Hanquan | Data Science Portfolio
---

# Liang Hanquan

**Data Science Portfolio** | MSc Data Science, University of Macau

I am a data science student who enjoys turning raw data into clear,
reproducible answers. My work focuses on exploratory analysis, careful
visualisation and honest reporting of what the data can and cannot support.
This site collects the projects I build as I develop those skills.

## Technical skills

- **Programming:** Python (pandas, NumPy, matplotlib, seaborn)
- **Analysis:** data cleaning, exploratory data analysis, summary statistics,
  simple classifiers, model evaluation
- **Reproducibility:** Git and GitHub, dependency pinning with
  `requirements.txt`, README-driven project documentation
- **Currently developing:** SQL and scikit-learn

## Project showcase

### Penguin Morphology: Can Bill Shape and Body Mass Separate Species?

**Research question:** Do bill dimensions and body mass separate Adelie,
Chinstrap and Gentoo penguins, and how much overlap remains between Adelie
and Chinstrap?

![Bill length versus bill depth by penguin species](https://raw.githubusercontent.com/kai117799/data-science-project/main/fig_bill_dimensions.png)

**What the visualization shows.** Each point is one penguin, coloured by
species; crosses mark species medians and the shaded regions show 1.5 SD
covariance ellipses. Gentoo forms a distinct cluster at shallower bill
depths (median 15.0 mm). Adelie and Chinstrap share a similar bill depth
(both 18.4 mm) but separate along bill length, with medians of 38.8 mm and
49.6 mm respectively. The overlap at the boundary is real, which is why a
single measurement is not enough for confident identification.

**Key findings**

- Gentoo penguins are about 35% heavier than the other two species
  (median 5,000 g versus 3,700 g).
- A leave-one-out nearest-centroid classifier using only bill length and
  depth reaches **93.6% accuracy**, showing how informative bill shape is.
- Flipper length correlates strongly with body mass (**r = 0.87**), and the
  relationship holds within each species.
- **Limitation:** the sample is observational, unevenly sized and limited to
  three islands, so the classifier describes separation in this dataset
  rather than a validated field identification tool.

[View the code and full README](https://github.com/kai117799/data-science-project)

**Status:** Completed

## What I will improve next

The next iteration will add a held-out test set and a model that controls
for sex and island, since both are associated with body size. I also want to
turn the analysis into a small interactive page so readers can filter by
species and island instead of reading static figures.

## About this site

This portfolio is built with GitHub Pages from the
[`data-science-portfolio`](https://github.com/kai117799/data-science-portfolio)
repository. The featured analysis is fully reproducible from its project
repository using the instructions in its README.

## Contact

- GitHub: [kai117799](https://github.com/kai117799)
- University of Macau, MSc Data Science
