# Project 1

## Overview

In this project, we implemented rasterization in the 2D setting, implementing at least some of what is required of rendering SVG files that are comprised of monochromatic shapes and textured shapes.

## Task 1

### How it works:
1) Triangle rasterization works by first creating a bounding box around each shape that we will be rasterizing the triangle in.
	- I did this by taking the max and min of the x and y values of each vertex of the triangle and adding and subtracting one respectively just to be certain that we're including all of the pixels that we need to.
2) Then, we iterate through each pixel in the bounding box and check if the pixel is inside the triangle.
3) If it's inside the triangle, then we 