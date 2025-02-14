# Image-clasification
Image clasification - CIFAR-10
For more Knowledge about the project read the article
[<iframe src="https://wandb.ai/himajakolavuennu-vellore-institute-of-technology/cifar10-classification/reports/Tata-communications-CIFAR-10-Image-Classification-Experimentation-Report--VmlldzoxMTI4NDAyOQ?accessToken=mngrv6fdzwkj1fy1btmiiy8mwxmyouzxyz3q5gm22dml09ddff3d01wsrpqlvakh" style="border:none;height:1024px;width:100%">](https://api.wandb.ai/links/himajakolavuennu-vellore-institute-of-technology/sjwo1si3)](https://api.wandb.ai/links/himajakolavuennu-vellore-institute-of-technology/sjwo1si3)

In this report, we analyze multiple CNN-based image classification experiments on the CIFAR-10 dataset using ResNet-18. The goal is to evaluate how different hyperparameters impact model performance.
Kolavennu Himaja
Created on February 10
|
Last edited on February 10
Comment
Experiment Setup
Dataset:
CIFAR-10 (60,000 images, 10 classes, 32x32 resolution).
Model:
ResNet-18 (pre-trained) with a modified final layer for 10-class classification.
Training Details:
Loss Function: CrossEntropyLoss
Epochs: 5 (for quick experimentation)
Logging: Weights & Biases (W&B)
Experiments & Results
Experiment 1: Adam Optimizer, Learning Rate = 0.001, Batch Size = 128
Training Accuracy: 67.21%
Validation Accuracy: 63.88%
Observation: The model converged quickly with Adam, but showed minor overfitting.
Experiment 2: Adam Optimizer, Learning Rate = 0.0005, Batch Size = 64
Training Accuracy: 64.35%
Validation Accuracy: 61.02%
Observation: Lowering the learning rate improved stability but resulted in slower convergence.
Experiment 3: SGD Optimizer, Learning Rate = 0.001, Batch Size = 128
Training Accuracy: 62.18%
Validation Accuracy: 59.75%
Observation: SGD performed worse than Adam at this learning rate, indicating it may require more tuning.
Insights & Analysis
Optimizer Impact: Adam outperformed SGD in our tests, achieving higher accuracy in fewer epochs.
Learning Rate Effect: A lower learning rate (0.0005) led to more stable training but slowed convergence.
 Batch Size: A batch size of 128 provided better generalization compared to 64.
Best Experiment: Adam with LR=0.001 and Batch Size=128 gave the best validation accuracy (63.88%).
In this report, we analyze multiple CNN-based image classification experiments on the CIFAR-10 dataset using ResNet-18. The goal is to evaluate how different hyperparameters impact model performance.
Kolavennu Himaja
Created on February 10
|
Last edited on February 10
Comment
Experiment Setup
Dataset:
CIFAR-10 (60,000 images, 10 classes, 32x32 resolution).
Model:
ResNet-18 (pre-trained) with a modified final layer for 10-class classification.
Training Details:
Loss Function: CrossEntropyLoss
Epochs: 5 (for quick experimentation)
Logging: Weights & Biases (W&B)
Experiments & Results
Experiment 1: Adam Optimizer, Learning Rate = 0.001, Batch Size = 128
Training Accuracy: 67.21%
Validation Accuracy: 63.88%
Observation: The model converged quickly with Adam, but showed minor overfitting.
Experiment 2: Adam Optimizer, Learning Rate = 0.0005, Batch Size = 64
Training Accuracy: 64.35%
Validation Accuracy: 61.02%
Observation: Lowering the learning rate improved stability but resulted in slower convergence.
Experiment 3: SGD Optimizer, Learning Rate = 0.001, Batch Size = 128
Training Accuracy: 62.18%
Validation Accuracy: 59.75%
Observation: SGD performed worse than Adam at this learning rate, indicating it may require more tuning.
Insights & Analysis
Optimizer Impact: Adam outperformed SGD in our tests, achieving higher accuracy in fewer epochs.
Learning Rate Effect: A lower learning rate (0.0005) led to more stable training but slowed convergence.
 Batch Size: A batch size of 128 provided better generalization compared to 64.
Best Experiment: Adam with LR=0.001 and Batch Size=128 gave the best validation accuracy (63.88%).
