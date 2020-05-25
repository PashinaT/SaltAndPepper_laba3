# SaltAndPepper_laba3
Calculation of π on GPU with Monte-Carlo method using CUDA

### Task definition
Given the image of size M×N with “Salt and Pepper” noise, implement and apply a CUDA version of 9-point median filter and store the result to output image. Missing values for edge rows and columns are to be taken from nearest pixels. CUDA implementation must make use of texture memory. 


To do this task, we need to count the number of points in circle - n_in_circle. Then find 4* n_in_circle/N.

#### Input data
• image with "Salt and Pepper" noise

![alt text](personGray512.bmp)

#### Output data

![alt text](personGray512.bmp)

### Results

The average time in milliseconds for 3 measurements

|   Image Size  | time CPU |  time GPU  | 
|---------------|----------|------------|
| 64x64         | 6 ms     | 1.21258 ms |
| 128x128       | 11 ms    | 1.38746 ms |
| 256x256       | 23 ms    | 2.61971 ms |
| 512x512       | 46 ms    | 7.64291 ms |
| 1024x1024     | 92 ms    | 8.93002 ms |

   
