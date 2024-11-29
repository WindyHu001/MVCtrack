### Train
- To train a model, you must specify the .py file. The .py file contains all the configurations of the dataset and the model. We provide .py files under the configs directory.

```
# single-gpu testing
python train.py --config configs/voxel/kitti/car.py --load_from pretrained/voxel/kitti/car.pth
# multi-n-gpu testing
python -m torch.distributed.launch --nproc_per_node=n train.py --config configs/voxel/kitti/car.py --load_from pretrained/voxel/kitti/car.pth --launcher pytorch
./dist_test.sh
```


