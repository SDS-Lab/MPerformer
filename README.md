# MPerformer: An SE(3) Transformer-based Molecular Perceptron

[![License: GPL-3.0](https://img.shields.io/badge/License-GPL3.0-blue)](https://github.com/FanmengWang/MPerformer/blob/master/LICENCE.txt)

This is the official implementation of "MPerformer: An SE(3) Transformer-based Molecular Perceptron" (CIKM 2023 FULL PAPER)

MPerformer is a universal learning-based molecular perception method to construct 3D molecules with complete chemical information purely based on molecular 3D atom clouds.
<p align="center"><img src="figures/Overview.png" width=80%></p>
<p align="center"><b>An illustration of MPerformer and its learning paradigm.</b></p>


Dependencies
------------
 - [Uni-Core](https://github.com/dptech-corp/Uni-Core), you can check its [Installation Documentation](https://github.com/dptech-corp/Uni-Core#installation).
 - `pip install rdkit-pypi==2021.9.4`

Quick Start
------------
- Please download the [checkpoint](https://drive.google.com/file/d/1sHWm1xOy0I8_R50dPANfMUXoRQkoPCBJ/view?usp=drive_link) and place it to the fold `./weight`
- Then you can use the following command to get the corresponding sdf file 
  ```bash
  XYZ_PATH='PATH OF YOUR XYZ FILE/FOLD'
  SDF_PATH='PATH TO SAVE SDF FILE'
  python predict.py --filename $XYZ_PATH --outputs_path $SDF_PATH
  ```
