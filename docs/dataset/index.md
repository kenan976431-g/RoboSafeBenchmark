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

## Download Datasets

- **Objects**: [https://modelscope.cn/datasets/kenan976431/RoboSafe_objects](https://modelscope.cn/datasets/kenan976431/RoboSafe_objects)
- **Embodiments**: [https://modelscope.cn/datasets/kenan976431/RoboSafe_embodiments](https://modelscope.cn/datasets/kenan976431/RoboSafe_embodiments)
- **Background Texture**: [https://modelscope.cn/datasets/kenan976431/RoboSafe_background_texture](https://modelscope.cn/datasets/kenan976431/RoboSafe_background_texture)
- **Simulation Episodes**: [https://modelscope.cn/datasets/kenan976431/RoboSafe_realworld_episodes](https://modelscope.cn/datasets/kenan976431/RoboSafe_realworld_episodes)
- **Real World Episodes**: [https://www.modelscope.cn/datasets/kenan976431/real_world_pick](https://www.modelscope.cn/datasets/kenan976431/real_world_pick)
