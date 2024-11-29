### Test
- To test a trained model, specify the checkpoint location with --resume_from argument and set the --phase argument as test.
```
# single-gpu testing
python test.py --config configs/voxel/kitti/car.py --load_from pretrained/voxel/kitti/car.pth
# multi-n-gpu testing
python -m torch.distributed.launch --nproc_per_node=n test.py --config configs/voxel/kitti/car.py --load_from pretrained/voxel/kitti/car.pth --launcher pytorch
./dist_test.sh
```



