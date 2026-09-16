# Depth Sensor Evaluation Reproduction

The data/ folder contains the point-cloud data used to evaluate depth
sensor accuracy against manually sampled stylus reference points.

## Data Layout

Each object folder in `data/{bone, meat, phantom}` contains:

- `stylus_points_object.pcd`: manually sampled object surface reference points.
- `stylus_points_cubes.pcd`: manually sampled calibration cube points.
- `sensors/<camera>/*.pcd`: aligned depth-camera captures.

Objects:

- `phantom`
- `bone`
- `meat`

Camera conditions:

- `d405`
- `flexx`
- `zed`
- `zivid`
- `meat/d405_closeup` is evaluated as a separate camera condition.
