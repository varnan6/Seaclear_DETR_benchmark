<h1 align = "center"> # Seaclear_DETR_benchmark </h1>

<p align = "center"> Placeholder for summary of abstract </p>

## Table of Content
* [1. Model Zoo](https://github.com/varnan6/Seaclear_DETR_benchmark?tab=readme-ov-file#1-model-zoo)
* [2. Quick start](https://github.com/varnan6/Seaclear_DETR_benchmark?tab=readme-ov-file#2-quick-start)
* [3. Usage](https://github.com/varnan6/Seaclear_DETR_benchmark?tab=readme-ov-file#3-usage)
* [5. Citation](https://github.com/varnan6/Seaclear_DETR_benchmark?tab=readme-ov-file#5-citation)
* [6. Acknowledgement](https://github.com/varnan6/Seaclear_DETR_benchmark?tab=readme-ov-file#6-acknowledgement)

## 1. Model Zoo

### COCO
| Model                   | Baseline     | Epochs | APval | APval50 | APval75 | APvalS | APvalM | APvalL | Config |
| :---------------------: | :----------: | :----: | :---: | :-----: | :-----: | :----: | :----: | :----: | :----: |
| YOLOv6-S                | EfficientRep | -      | 45.0  |   -     |   -     |   -    |   -    |   -    |   -    |
| DETR                    | ResNet-50    | 500    | 43.3  | 63.1    | 45.9    | 22.5   | 47.3   | 61.1   |   -    |
| DAB-Deformable-DETR     | ResNet-50    | 50     | 46.9  | 66.0    | 50.8    | 30.1   | 50.4   | 62.5   |   -    |
| DN-Deformable-DETR      | ResNet-50    | 50     | 48.6  | 67.4    | 52.7    | 31.0   | 52.0   | 63.7   |   -    |
| DiffusionDet (1@500)    | ResNet-50    | 300    | 46.3  | 64.8    | 50.7    | 28.6   | 49.0   | 62.1   |   -    |
| DiffusionDet (1@500)    | ResNet-101   | 300    | 47.2  | 65.7    | 51.6    | 30.2   | 50.2   | 62.7   |   -    |
| DEIM-M                  | D-Fine-M     | 90     | 52.7  | 70.0    | 57.3    | 35.3   | 56.7   | 69.5   | [yml](./configs/deim_dfine/deim_hgnetv2_m_coco.yml) |
| DEIM-X                  | D-Fine-X     | 50     | 56.5  | 74.0    | 61.5    | 38.8   | 61.4   | 74.2   | [yml](./configs/deim_dfine/deim_hgnetv2_x_coco.yml) |
| DEIM-RTDETRv2-M*        | ResNet-50    | 60     | 55.5  | 73.5    | 60.3    | 37.9   | 59.9   | 73.0   |   -    |

### Seaclear
| Model                   | Baseline     | Best Epochs | APval | APval50 | APval75 | APvalS | APvalM | APvalL |
| :---------------------: | :--------:   | :---------: | :---: | :-----: | :-----: | :----: | :----: | :----: |
| DiffusionDet (1@500)[8] | ResNet-50    | 80          | 63.5  | 89.6    | 69.3    | 33.1   | 47.9   | 69.7   |
| DiffusionDet (1@500)[8] | ResNet-101   | 60          | 64.2  | 89.4    | 70.5    | 33.4   | 48.4   | 70.2   |
| YOLOv6-S                | EfficientRep | -           | 68.3  |   -     |   -     |   -    |   -    |   -    |
| DEIM-M                  | D-Fine       | 151         | 68.7  | 89.5    | 76.5    | 32.0   | 56.2   | 75.2   |
| DEIM-X                  | D-Fine       | 111         | 70.2  | 90.8    | 76.9    | 34.8   | 57.3   | 77.4   |
| DEIM-RTDETRv2-M*        | ResNet-50    | 106         | 71.9  | 92.7    | 80.2    | 34.8   | 57.6   | 77.8   |
