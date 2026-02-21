# Stat550_project1


## Project Overview

This project investigates **occlusion-robust** and **amodal object detection** methods. The primary goal is to detect or segment objects that are **partially occluded** within an image.

In real-world environments, objects are frequently obstructed by other objects. Traditional object detection and instance segmentation models often struggle under these conditions. This project focuses on improving robustness under occlusion and exploring amodal reasoning, where the model predicts the full extent of an object—even when parts are not visible.

As part of this research effort, multiple open-source amodal segmentation frameworks were studied and evaluated using real-world datasets to develop a functional and reproducible system. The two primary codebases explored include:

- **:contentReference[oaicite:0]{index=0}** – *Amodal Segmentation by Synthesizing Wholes*  
- **:contentReference[oaicite:1]{index=1} (BMVC 2024)** – A sequential learning approach to cumulative occlusion reasoning

The second framework was introduced at **:contentReference[oaicite:2]{index=2}** (British Machine Vision Conference 2024).

Through hands-on experimentation with these repositories, this project evaluates architectural approaches, training strategies, and dataset handling techniques for improving amodal segmentation performance under realistic occlusion scenarios.
