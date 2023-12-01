# Architected Material Lab: Multiclassification for 3D Printing Error Detection 
### Fall 2023 Continuation of Summer 2023 PURM Research project 

## Information and code for Summer contributions: 

[High-Level Project Breakdown](https://liuyuhan.me/research/)

[Research Expo Poster and Abstract](https://presentations.curf.upenn.edu/poster/improving-precision-direct-write-3d-printing-computer-vision-and-machine-learning
)

[Full Code Base without Fall 2023 Contributions](https://github.com/yuhanliu-tech/aml_multiclassification)

## Fall 2023 Contributions Summary 

Trainsitioning from Summer to Fall, progress had been made on error detection for single-stroke images. 
Improve test accuracy for predicting single-layer images, in which multiple strokes combine. We decided to use different models for single-stroke and single-layer because of inherent visual differences. 
Training models on single-layer resulted in solid accuracies, but that may be due to overfitting, since live predictions yielded poor results. 
Our goal is to improve the model and training process so that accuracies for both single-stroke and single-layer improved, thus allowing us to eventually move into multi-layer error detection. 

Our main improvement for Fall 2023 is converting image resolutions in model training. Models from the summer were trained on 32x32 images. The small image size may contribute to overfitting and live prediction inaccuracy. 
Thus, one approach is to update the model so that it now trains on 64x64 images. 

This conversion was completed and ran on some re-sized images from older data collections. It yielded an accuracy of approximately 93%. It has yet to be tested on live predictions. 

File breakdown follows the same naming system and methodology as [Summer 2023 Error Detection File Breakdown on Github](https://github.com/yuhanliu-tech/aml_multiclassification#error-detection-five-classes). 
