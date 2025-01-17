# Kaggle-HuBMap+HPA
## Kaggle Competition - HuBMap + HPA [Team : H2]
### 대회 개요

* 목적 : 인체를 구성하는 37조 개의 세포 사이의 기능과 관계를 파악하여 세포 구성에 대한 이해도 증진.
* 비전 : 세포와 조직 조직 간의 관계에 대한 이해를 가속화하는 데 도움
* 목표 : 5개의 인간 장기에 걸쳐 기능 조직 단위(FTU)를 식별하고 분류. FTU를 가능한 한 정확하게 분할하는 것이 중요. 조직 섹션 이미지의 데이터 세트를 사용하여 모델을 구축.

## 사용한 방법론

### Structure
* UNet + EfficientNetB6
* DeepLabV3plus + Resnet
* Unet + Swin Transformer

### Loss
* 1 * Weight Binary Cross Entropy + 0.5 * dice_coef_loss

### Augmentation
* Flip
* cell staining, Color

## High Score
* Unet + Swin Transformer -> 0.69737
