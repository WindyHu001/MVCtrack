### Virtual_cues
- You can choose a segmentation model, such as CenterNet2, and generate corresponding virtual clues using the following command.

```
# nuScenes
python virtual_gen.py --info_path data/nuScenes/infos_train_10sweeps_withvelo_filter_True.pkl  MODEL.WEIGHTS centernet2_checkpoint.pth 
```
