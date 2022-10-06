# YZLFusion

## Methods

plain centerpoint-voxel(without better backbone like focalsparse conv,without better neck like SA-FPN,without better head like transfusionhead) + swin-tiny + fusion strategy.

## News

* (2022.9.4) rank 1st and 1st in the term of NDS and mAP on the nuScenes leaderboard among all methods that don't use TTA and Ensemble.
* (2022.9.21) rank 1st and 2nd in the term of NDS and mAP on the nuScenes learderboard among all methods that use single model and TTA.
* (2022.10.6) rank 1st and 3rd in the term of NDS and mAP on the nuScenes learderboard among all methods that use Ensemble. [learderboard link](https://eval.ai/web/challenges/challenge-page/356/leaderboard/1012)

## Nuscene Single Model Performance

### Valset

| Image     | Lidar              | mAP    | NDS    |
| --------- | ------------------ | ------ | ------ |
| ResNet50  | Pillar-02pillar    | 0.6701 | 0.6988 |
| ResNet50  | VoxelNet-0075voxel | 0.7037 | 0.7259 |
| Swin-Tiny | VoxelNet-0075voxel |        |        |

### Testset

| Image     | Lidar              | mAP   | NDS   |
| --------- | ------------------ | ----- | ----- |
| Swin-Tiny | VoxelNet-0075voxel | 0.722 | 0.738 |

## Nuscene Ensemble Model Performance

| Image     | Lidar         | Strategy                                             | mAP    | NDS    |
| --------- | ------------- | ---------------------------------------------------- | ------ | ------ |
| Swin-Tiny | VoxelNet-0075 | double lidar backbone channel, single-model+flip+rot | 0.7363 | 0.7557 |

