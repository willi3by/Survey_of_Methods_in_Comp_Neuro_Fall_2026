# Week 6 data dictionary

## population_activity.csv

Each row is one neural-response trial.

- `animal_id`: animal identifier
- `trial_id`: trial number within animal
- `neuron_01` ... `neuron_30`: simulated response magnitude for 30 recorded neurons

## animal_metadata.csv

One row per animal.

- `animal_id`: animal identifier
- `treatment`: `Control` or `Stimulated`
- `treatment_binary`: 0 for control, 1 for stimulated
- `pair_id`: matched animal pair used for held-out-pair validation; each pair contains one animal from each treatment group

The dataset is synthetic and is intended for teaching neural decoding, validation design, grouped validation, and permutation controls.
