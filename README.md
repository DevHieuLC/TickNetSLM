# TickNets: Transitional patterns for tick-shape backbones

**Abstract:**

* A lightweight Convolutional Neural Network (CNN) is one of the potential solutions for real applications on edge devices. Recently, TickNets are formed by allocating Full-Residual Point-Depth-Point (FR-PDP) blocks in a multiple of tick-shape backbones. However, it can be a lack of diverse information since only the FR-PDP-based features have been exploited in those backbones. This shortcoming can be the cause of their modest performance in several circumstances, while still taking a high computational cost. To mitigate this issue, a transition layer is proposed to exploit the transitional patterns for learning diverse information in TickNets. Simply, a pointwise convolution is embedded as a hooking connection for pointwise-based features instead of the FR-PDP-based features that have been transferred between two basic tick-shape backbones. It can be seen that addressing such a transition layer would lead to two practical benefits: _i_ extracting diverse patterns for the learning process; _ii_ a significant reduction of model complexity thanks to the lightweight pointwise operation. Experimental results for image classification on benchmark datasets have validated the efficiency of our proposal. Particularly, with less computational complexity, the proposed transitional patterns have boosted about 1.2\% performance on Stanford Dogs versus the original TickNets, while it is the same on CIFAR-10/100. It could be an alternative solution for TickNets in real applications. The implementation code is available at \url{https://github.com/DevHieuLC/TickNetSLM}.

<u>**Training TickNets on Datasets:**</u>

For Stanford Dogs. Note that it will automatically run for all TickNets, i.e., TickNet-SM, TickNet-LM
```
$ python TickNetSLM_Dogs.py --download
```
Note: Subject to your system, modify these training files (*.py) to have the right path to datasets

**Validating the trained models of TickNets:**
* For Stanford Dogs (TickNet-SM)
```
$ python TickNetSLM_Dogs.py --evaluate
```
Note: For instances of validation of TickNet-SM, download the trained model of TickNet-SM on Datasets: [Click here for Stanford Dogs](https://drive.google.com/drive/folders/1RGglukdrd5xDrGSo6ONmHTCZNZ-YwpZb?usp=sharing). And then locate the downloaded file at ./checkpoints/StanfordDogs/SM

**Related citations:**
If you use any materials, please cite the following relevant works.
```
@inproceedings{ISCITLe2025,
  author={Chi-Hieu Le and Thanh Tuan Nguyen and Hoang Anh Pham and Hoai Nam Vu and Thi-Minh-Chau Le and Thanh Phuong Nguyen},
  booktitle={ISCIT}, 
  title={Transitional patterns for tick-shape backbones}, 
  year={Submitted in 2025}
}
```
