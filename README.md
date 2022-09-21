# YZLFusion



## Nuscene Single Model Performance

### Valset

| Image     | Lidar              | mAP    | NDS    |
| --------- | ------------------ | ------ | ------ |
| ResNet50  | Pillar-02pillar    | 0.6701 | 0.6988 |
| ResNet50  | VoxelNet-0075voxel | 0.7037 | 0.7259 |
| Swin-Tiny | VoxelNet-0075voxel |        |        |

### Testset

| Image     | Lidar              | mAP   | NDS   |      |
| --------- | ------------------ | ----- | ----- | ---- |
| Swin-Tiny | VoxelNet-0075voxel | 0.722 | 0.738 |      |

## Nuscene Ensemble Model Performance

| Image     | Lidar         | Strategy                                             | mAP    | NDS    |
| --------- | ------------- | ---------------------------------------------------- | ------ | ------ |
| Swin-Tiny | VoxelNet-0075 | double lidar backbone channel, single-model+flip+rot | 0.7363 | 0.7557 |
|           |               |                                                      |        |        |

