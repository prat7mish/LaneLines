# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I applied Gaussian smoothing to let edges features easier to find. Afterwards, I used Canny edge detection to find edges, then mask out uninterested region using 4 sided polygon. Then, hough transform is applied to find the line segments.


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would be the intersecting lines seen at the end which might cause some problem.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to to improve on the intersecting lines as I mentioned before and also to make the skewed lines more clearer. Also there could be improvements for banked and curved roads.
