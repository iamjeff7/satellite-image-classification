# satellite-image-classification

Classification on satellite image are performed using Machine Learning and Deep Learning algorithms. The
algorithms are trained on the subset of NPU-RESISC45 dataset which consists of 12 scene
classes, with 700 images. The classification model performance is evaluated using accuracy,
precision, recall, F1-score and confusion matrix.

| Description                                                                                       | Accuracy  | Precision  | Recall  | F1 score |
|---------------------------------------------------------------------------------------------------|-----------|------------|---------|----------|
| 1. Bag-of-Visual-Words                                                                            | 50.5      | 52.41      | 50.5    | 48.52    |
| 2. VGG16(ImageNet) + FullyConnected                                                               | 87.83     | 88.20      | 87.83   | 87.93    |
| 3. VGG16(ImageNet) +SVM                                                                           | 82.06     | 82.06      | 82.06   | 82.06    |
| 4. FineTune VGG16(ImageNet) +FullyConnected                                                       | 88.61     | 89.45      | 88.61   | 88.61    |
| 5. FineTune VGG16(ImageNet) withdata augmentation +FullyConnected                                 | 90.94     | 91.36      | 90.94   | 90.95    |
| 6. FineTune VGG16(Places365) +FullyConnected                                                      | 85.00     | 85.93      | 85.00   | 85.00    |
| 7. FineTune VGG16(Places365) withdata augmentation +FullyConnected                                | 85.50     | 86.25      | 85.50   | 85.54    |
| 8. Ensemble model 1:BoVW +FineTuneVGG16(Places365) +FullyConnected                                | 89.28     | 89.43      | 89.28   | 89.30    |
| 9. Ensemble model 2:FineTune VGG16(ImageNet)withdata augmentation + FineTuneVGG16(Places365) +SVM | 81.61     | 82.00      | 81.61   | 81.62    |

## Samples of images
### beach
![Alt text](/images/beach_001.jpg?raw=true)
![Alt text](/images/beach_002.jpg?raw=true)
![Alt text](/images/beach_003.jpg?raw=true)
### commercial_area
![Alt text](/images/commercial_area_001.jpg?raw=true)
![Alt text](/images/commercial_area_002.jpg?raw=true)
![Alt text](/images/commercial_area_003.jpg?raw=true)
### desert
![Alt text](/images/desert_001.jpg?raw=true)
![Alt text](/images/desert_002.jpg?raw=true)
![Alt text](/images/desert_003.jpg?raw=true)
### farmland
![Alt text](/images/farmland_001.jpg?raw=true)
![Alt text](/images/farmland_002.jpg?raw=true)
![Alt text](/images/farmland_003.jpg?raw=true)
### forest
![Alt text](/images/forest_001.jpg?raw=true)
![Alt text](/images/forest_002.jpg?raw=true)
![Alt text](/images/forest_003.jpg?raw=true)
### industrial_area
![Alt text](/images/industrial_area_001.jpg?raw=true)
![Alt text](/images/industrial_area_002.jpg?raw=true)
![Alt text](/images/industrial_area_003.jpg?raw=true)
### island
![Alt text](/images/island_001.jpg?raw=true)
![Alt text](/images/island_002.jpg?raw=true)
![Alt text](/images/island_003.jpg?raw=true)
### lake
![Alt text](/images/lake_001.jpg?raw=true)
![Alt text](/images/lake_002.jpg?raw=true)
![Alt text](/images/lake_003.jpg?raw=true)
### mountain
![Alt text](/images/mountain_001.jpg?raw=true)
![Alt text](/images/mountain_002.jpg?raw=true)
![Alt text](/images/mountain_003.jpg?raw=true)
### residential
![Alt text](/images/residential_001.jpg?raw=true)
![Alt text](/images/residential_002.jpg?raw=true)
![Alt text](/images/residential_003.jpg?raw=true)
### river
![Alt text](/images/river_001.jpg?raw=true)
![Alt text](/images/river_002.jpg?raw=true)
![Alt text](/images/river_003.jpg?raw=true)
