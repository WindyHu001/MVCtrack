### Virtual_cues
- You can choose a segmentation model, such as CenterNet, and generate corresponding virtual clues using the following command.

```
# nuScenes
python tools/create_data.py nuscenes_data_prep --root_path=NUSCENES_TRAINVAL_DATASET_ROOT --version="v1.0-trainval" --nsweeps=10 --virtual True
```
