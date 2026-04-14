# contextual-bandits

Runnable notebook for the 2026-04-15 *Contextual Bandits* lecture in Columbia's *Persuasion at Scale* (Prof Eunji Kim, Prof Chris Wiggins).

## What's in here

`notebooks/cb.ipynb` walks through the contextual-bandit idea in three acts:

1. **Warmup: classical 2-arm bandit.** Pure K-armed setup, no context. Reminds you of Monday's material.
2. **LinUCB on a toy 2-arm contextual bandit.** Synthetic 10-dim context vectors, per-arm ridge regression, upper confidence bound. Plots show estimated betas converging, allocation over time.
3. **Real data: Kenya/Nigeria Facebook Messenger misinformation.** Loads the replication data from Offer-Westort, Rosenzweig & Athey (2024) "Battling the coronavirus 'infodemic' among social media users in Kenya and Nigeria," *Nature Human Behaviour*. 15,292 Facebook Messenger users, 40 treatment arms, real outcomes (intent to share misinformation). We collapse to 4 interpretable arms (accuracy nudge on/off × warning flag on/off) and run LinTS on the real context features. Headline from the paper: accuracy nudges reduced sharing by 4.9%.

## Open it

Colab: https://is.gd/20260415PatScolab

Or: https://colab.research.google.com/github/Persuasion-at-Scale/contextual-bandits/blob/main/notebooks/cb.ipynb

## Data source

Replication repo (public, no auth): https://github.com/gsbDBI/infodemic-replication

Primary data file: `data/cleaned-data_2023-03-28.csv` (6.7 MB). Loaded directly from raw GitHub in the notebook, no download needed.

## License

MIT. See `LICENSE`.
