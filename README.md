# Stat550_project1


## Project Overview

This project investigates **occlusion-robust** and **amodal object detection** methods. The primary goal is to detect or segment objects that are **partially occluded** within an image.

In real-world environments, objects are frequently obstructed by other objects. Traditional object detection and instance segmentation models often struggle under these conditions. This project focuses on improving robustness under occlusion and exploring amodal reasoning, where the model predicts the full extent of an object—even when parts are not visible.

## Codebases Used
As part of this research effort, multiple open-source amodal segmentation frameworks were studied and evaluated using real-world datasets to develop a functional and reproducible system. The two primary codebases explored were [pix2gestalt: Amodal Segmentation by Synthesizing Wholes](https://github.com/cvlab-columbia/pix2gestalt) and [Sequential Amodal Segmentation via Cumulative Occlusion Learning (BMVC2024)](https://github.com/saraao/SAS)

Ultimately, SAS was used sa the primary codebase to reasearch for this project. 

## Reproducability instructions
Following the instructions provided in the repo for SAS, I was able to sucessfully install SAS while utilizing the ISL Vecotr 6 machine for its hardware capabilities. When running the initial training script, python scripts/train.py --data_dir './example_data/training/'  --save_dir './you/path/to/save/' --noise_rate 0.0 $TRAIN_FLAGS $MODEL_FLAGS $DIFFUSION_FLAGS, an error was produced saying "FileNotFoundError: [Errno 2] No such file or directory: 'you/path/here/'". The acomloader.py script had hard coded a place holder for a directory that was supposed to contain noise. This directory would influence the --noise_rate flage should it be adjusted past 0. In order to get around this, I made a dummy folder in the location of the SAS parent directory call data/noise. I then pointed to that directory in the acomloader.py script and ran the train script as provided. This then led to the training for the model to start. 
