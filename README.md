# Stat550_project1


## Project Overview

This project investigates **occlusion-robust** and **amodal object detection** methods. The primary goal is to detect or segment objects that are **partially occluded** within an image.

In real-world environments, objects are frequently obstructed by other objects. Traditional object detection and instance segmentation models often struggle under these conditions. This project focuses on improving robustness under occlusion and exploring amodal reasoning, where the model predicts the full extent of an object—even when parts are not visible.

As part of this research effort, multiple open-source amodal segmentation frameworks were studied and evaluated using real-world datasets to develop a functional and reproducible system. The two primary codebases explored were [pix2gestalt: Amodal Segmentation by Synthesizing Wholes](https://github.com/cvlab-columbia/pix2gestalt) and [Sequential Amodal Segmentation via Cumulative Occlusion Learning (BMVC2024)](https://github.com/saraao/SAS)
