# Convergence-Project-Spring-2023-Team4

## baseline model parameters
---
- Backbone : ResNet50(pretrained with ImageNet)
- Input Size : 224x224
- Batch Size : 32
- Learning Rate : 0.0001
- Epoch : 25
- Optimizer : Adam
- ### [[LINK]](https://github.com/Sejong-VLI-Courses/Convergence-Project-Spring-2023-Team4/tree/baseline)

## proposed improvements
---
- backbone : wide resnet101 
- learning rate : 0.0001
- learning rate scheduling : milestone=[12,20], gamma=0.2
- ### [[LINK]](https://github.com/Sejong-VLI-Courses/Convergence-Project-Spring-2023-Team4/blob/wide_resnet101/README.md)

## performance 
---
- ### [[Excel]](https://github.com/Sejong-VLI-Courses/Convergence-Project-Spring-2023-Team4/blob/main/wideresnet101_results.xlsx)
