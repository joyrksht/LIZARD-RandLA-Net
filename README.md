# LIZARD RandLA-Net

This repository adapts the [RandLA-Net](https://github.com/QingyongHu/RandLA-Net) framework (originally for the Semantic3D dataset) for the **LIZARD project**: *Liver resection zone prediction using image-based and geometric deep learning* ([DFG Project No. 547369510](https://gepris.dfg.de/gepris/projekt/547369510)).

### Project Goal

- Automated segmentation of liver structures affected by liver cancer. 
- Patient-specific resection planning.  
- Integrating clinical data to enhance prediction accuracy.  
- Improving pre-operaive planning with enhanced visualizations.
  
## Example of Input and Output Data

![Demo](sample/Sample.gif)

## Pretrain Weights

Pretrain weights can be found [here](https://github.com/joyrksht/LIZARD-RandLA-Net/tree/main/results/Log_2025-07-08_16-05-43/snapshots).

## Acknowledgment

- Implementation adapted from the [RandLA-Net](https://github.com/QingyongHu/RandLA-Net) codebase.
- This project is funded by German Cancer Research (project no. 70116062) and the German Research Foundation (project no. 547369510).

## How to cite
Please cite the article “Deep Learning-Based Segmentation of Acute Pulmonary Embolism in Cardiac CT images" by Ehsan Amini, Georg Hille, Janine Hürtgen, Alexey Surov,
Sylvia Saalfeld, 2025. You can also copy the bibtex:

```biblatex
@article{RAKSHIT2025111103,
title = {Geometric deep learning adapted to prediction of liver resection zone},
journal = {Computers in Biology and Medicine},
volume = {197},
pages = {111103},
year = {2025},
issn = {0010-4825},
doi = {https://doi.org/10.1016/j.compbiomed.2025.111103},
url = {https://www.sciencedirect.com/science/article/pii/S0010482525014556},
author = {Joy Rakshit and Robert Kreher and Tobias Huber and Hauke Lang and Florentine Huettl and Sylvia Saalfeld},
keywords = {Geometric deep learning, Hybrid loss function, Attentive pooling, Hepatic surgery, Decision support system, 3D point cloud, 3D geometric mesh},
abstract = {Due to patient-specific anatomical variations in the presence of liver cancer, resection planning can be complex requiring thorough preoperative planning. In addition to the calculation of the Future Liver Remnant, the assessment of any vascular and biliary structures that may be at risk is essential to minimize postoperative morbidity and mortality. Despite the progress of modern technologies, this resection planning is still mostly performed mentally, but can be supported by volumetric calculations or planning on a three-dimensional (3D) model. The aim of this work is to investigate the effectiveness of geometric deep learning (DL) in predicting liver resection zones. We adopted a geometric DL framework, specifically RandLA-Net, a lightweight and efficient neural network designed for semantic segmentation of large-scale 3D point clouds, to support surgical planning for liver tumor resections using 3D geometric data, presented in either mesh or point cloud format. RandLA-Net can process up to one million points in a single pass and operates up to 200 times faster than comparable frameworks, making it particularly well suited for high-resolution anatomical data in clinical settings. We conducted our experiment in two stages. In the first stage, the pilot study, we evaluated two geometric deep learning models in combination with four different loss functions: Cross-Entropy (CE), Dice coefficient (DICE), Intersection over Union (IoU), and a hybrid loss (a combination of CE and IoU) to efficiently predict the resection volume. Among all the configurations tested, RandLA-Net combined with hybrid loss achieved the best performance. In the second stage, the extended study, we increased the dataset size and repeated the experiment using the best-performing configuration identified in the pilot study, with minor modifications. The extended study demonstrated improved performance, with a mean IoU of 0.76, F1-score of 0.84, precision of 0.86, and recall of 0.82.}
}
```

## Contact
Joy.Rakshit@uksh.de
Saalfeld@medinfo.uni-kiel.de
