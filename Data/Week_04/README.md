# Week 4 microscopy dataset

This is a **synthetic microscopy-style teaching dataset** created for the Week 4 class. It is designed to reproduce realistic analysis structure without requiring an external download or representing measurements from real animals.

- 14 animals: 7 control and 7 stimulation.
- 2 fields of view (FOVs) per animal.
- About 40 segmented cells per FOV.
- Pixel size: 0.75 µm/pixel.
- Each `.npz` file contains a DAPI-like nuclear channel (`dapi`), an activity-marker channel (`marker`), a simulation truth label image (`true_labels`), the stimulation-site coordinates, and pixel size.
- `cell_features.csv` contains one row per cell with spatial coordinates, distance to the stimulation site, soma area, treatment, and activity-marker intensity.

The analysis intentionally contains animal-level and FOV-level variation so that treating every cell as an independent experimental unit gives overconfident uncertainty estimates for animal-level treatment effects.
