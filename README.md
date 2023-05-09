# Convergence-Project-Spring-2023-Team4

## baseline model parameters
---
- Backbone : ResNet50(pretrained with ImageNet)
- Input Size : 224x224
- Batch Size : 32
- Learning Rate : 0.0001
- Epoch : 25
- Optimizer : Adam

## proposed improvements
---
- backbone : wide resnet101 
- learning rate : 0.0001
- learning rate scheduling : milestone=[12,20], gamma=0.2

## Compared with baseline scores
- rounded up from the third decimal place

| Scenario 5 | score |
|:--:|:--:|
| top1 | 61.20% -> 63.72%(+2.52%)|
| top2 | 83.28% -> 83.91%(+0.63%)|
| top3 | 91.80% -> 94.01%(+2.21%)|
| mse loss | 19.92 -> 0.98(-18.94)|

| Scenario 6 | score |
|:--:|:--:|
| top1 | 48.78% -> 53.66%(+4.88%)|
| top2 | 78.66% -> 74.39%(-4.27%)|
| top3 | 87.80% -> 82.32%(+5.48)|
| mse loss | 0.97 -> 1.91(+0.94)|

| Scenario 7 | score |
|:--:|:--:|
| top1 | 39.81% -> 39.81%(+0%)|
| top2 | 59.22% -> 61.17%(+1.95%)|
| top3 | 70.87% -> 67.00%(-3.87%)|
| mse loss | 2.27 -> 1.25(1.02)|

| Scenario 8 | score |
|:--:|:--:|
| top1 | 68.19% -> 70.94%(+2.75%)|
| top2 | 91.99% -> 93.14%(+1.15%)|
| top3 | 98.17% -> 96.57%(-1.60%)|
| mse loss | 1.61 -> 0.42(-1.19)|

| Scenario 9 | score |
|:--:|:--:|
| top1 | 56.32% -> 58.18%(+1.86)|
| top2 | 80.94% -> 81.79%(+0.85)|
| top3 | 89.04% -> 90.56%(+1.52)|
| mse loss | 3.22 -> 0.74(-2.48)|


## Data augmentation version
---
- backbone : wide resnet101 
- learning rate : 0.0001
- learning rate scheduling : milestone=[12,20], gamma=0.2
- ColorJitter(brightness=0.1, contrast=0.1, saturation=0.1)]
- rounded up from the third decimal place

| Scenario 5 | score |
|:--:|:--:|
| top1 | 62.78%|
| top2 | 83.60%|
| top3 | 91.48%|
| mse loss | 1.01|

| Scenario 6 | score |
|:--:|:--:|
| top1 | 56.10%|
| top2 | 77.44%|
| top3 | 84.15%|
| mse loss | 31.37|

| Scenario 7 (brightness=0.1, contrast=0.1, saturation=0.1) | score | 
|:--:|:--:|
| top1 | 37.86%|
| top2 | 62.13%|
| top3 | 66.02%|
| mse loss | 3.87|

| Scenario 7 (brightness=0.3, contrast=0.3, saturation=0.3) | score | 
|:--:|:--:|
| top1 | 41.75%|
| top2 | 59.22%|
| top3 | 66.02%|
| mse loss | 3.41|

| Scenario 8 | score |
|:--:|:--:|
| top1 | 70.71%|
| top2 | 91.76%|
| top3 | 96.80%|
| mse loss | 1.62|

| Scenario 9 | score |
|:--:|:--:|
| top1 | 58.01%|
| top2 | 82.97%|
| top3 | 91.40%|
| mse loss | 3.07|

