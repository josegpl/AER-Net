# AER-Net

Official github repository for the proposed convoluted neural network: Attention Efficient Residual U-Net. This project contributed to my bachelor thesis "Attention Efficient Residual U-Net: uma Rede Neural para a Segmentação de Lesões de Pele" written and presented at Federal University of Maranhão in April 2021 which achieved the highest grade for approval.

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#Motivation">Motivation</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#About the Project">About the Project</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#Results">Results</a></li>
  </ol>
</details>

<!-- MOTIVATION AND INTRODUCTION -->

## Motivation

Melanoma is one of the most severe skin cancer types due to its high mortality rate, which can achieve 70%. An early diagnosis of the disease is crucial as it increases the ten-year survival rate up to 97%. The segmentation of skin lesions is one of the essential steps of the diagnosis process for accurate melanoma detection. However, even for specialist doctors, segmenting these lesions is costly and challenging due to the wide variety of stains, which can have irregular edges, different dimensions, and colors, and due to the high amounts of exams to analyze. Automatic detection of the lesion area for segmentation proves to be an important area of study so that the specialist doctor can focus on the correct diagnosis of the disease itself. 

This work aims to propose a new model based on encoder-decoder architectures that achieve efficiency and performance parameters for the segmentation of dermoscopic images.

## About the Project

In this paper we propose a new convolutional neural netwok called AER-Net, short for Attention Efficient Residual U-Net. It is based on three main components:
Pre-trained EfficientNet backbone encoder, residual connections througout the paths of the architecture and skip connections through the usage of Attention Gates. 

<div  align="center">
<img src="./imgs/AER-Net architecture.png" width = "700">
</div>
<div  align="center">
<figcaption>AER-Net architecture. Author: José Guilherme P. Lima</figcaption>
</div>

## Results

In our experiments, we use AER-NET on dermoscopic images taken from the public ISIC 2018 challenge dataset. The new proposed technique outperforms existing non-assembling techniques, including U-Net and Attention U-Net based on Jaccard Index and/or Dice Coefficient index metrics.

<div  align="center">
<img src="./imgs/Comparison_Table.PNG" width = "500">
</div>
<div  align="center">
<figcaption>Comparison Table. Author: José Guilherme P. Lima</figcaption>
</div>

<div  align="center">
<img src="./imgs/aer example.png" width = "500">
</div>
<div  align="center">
<figcaption>AER-NET outputs: good, medium, unsatisfactory examples from top to bottom</figcaption>
</div>


