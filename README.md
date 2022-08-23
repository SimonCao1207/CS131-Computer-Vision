# Assignments CS131: Computer Vision Foundations and Applications (self study)

## Overview
- This repository contains solutions of released assignments for the fall 2021 course of CS131 Standford course. 

## Takeaway
- **HW0**: go through basic linear algebra, NumPy, and image manipulation
- **HW1**: covers linear filters, convolution and correlation.
    - *Cross-correlation* can be used for template matching: a template  𝑔  is multiplied with regions of a larger image  𝑓  to measure how similar each region is to the template. 
    - The running time of *a separable 2D convolution* is slower than its equivalent two 1D convolutions.
- **HW2**:  Canny edge detector and Line Detection with Hough transform.
    - Canny edge detector: 
        - Smoothing the image by convoluting with Gaussian Kernel.
        - Finding gradients.
        - Non-maximum  suppression: convert the blurred edges to sharp edges.
        - Double thresholding: use high and low threshold to discern between true edges and noises/color variations.
        - Edge Tracking: weak edges due to true edges are much more likely to be connected directly to strong edges.
    - Lane Detection with Hough transform
        - Detect edge with Canny edge detection
        - Extract the edge in the ROI (region of interest)
        - Line Detection with [Hough transform](https://web.ipac.caltech.edu/staff/fmasci/home/astro_refs/HoughTrans_lines_09.pdf)
