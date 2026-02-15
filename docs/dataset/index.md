# Dataset

## Overview

The dataset contains extensive safety-critical scenarios for robotic manipulation.

## Statistics

- **Trajectories**: 100,000+
- **Objects**: 200+
- **Tasks**: 80+
- **Safety Scenarios**: Multiple failure modes and edge cases

## Download

```bash
# Download dataset
robosafe download --split train
```

## Data Format

Each episode contains:

```python
episode = {
    "rgb": np.array(...),        # RGB images
    "depth": np.array(...),      # Depth images  
    "actions": np.array(...),    # Action trajectory
    "states": np.array(...),     # Robot states
    "safety_flags": np.array(...)  # Safety indicators
}
```

## Data Collection

See our [data collection guide](collection.md) for details.
