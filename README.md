# SaltAndPepper_laba3
Calculation of π on GPU with Monte-Carlo method using CUDA

### Task definition
Given the image of size M×N with “Salt and Pepper” noise, implement and apply a CUDA version of 9-point median filter and store the result to output image. Missing values for edge rows and columns are to be taken from nearest pixels. CUDA implementation must make use of texture memory. 


To do this task, we need to count the number of points in circle - n_in_circle. Then find 4* n_in_circle/N.

#### Input data
• image with "Salt and Pepper" noise
![alt text](personGray512.bmp)

#### Output data
• The time of GPU and CPU programs execution;
• π values calculated by GPU and CPU programs (results may be different).

### Results

The average time in milliseconds for 3 measurements

| Total points  | time CPU |  time GPU  | result π CPU | result π GPU  |
|---------------|----------|------------|--------------|---------------|
| 1048576=2^20  | 6 ms     | 1.21258 ms |   3.14075    |    3.14075    |
| 2097152=2^21  | 11 ms    | 1.38746 ms |   3.13811    |    3.13811    |
| 4194304=2^22  | 23 ms    | 2.61971 ms |   3.14039    |    3.14039    |
| 8388608=2^23  | 46 ms    | 7.64291 ms |   3.14089    |    3.14089    |
| 16777216=2^24 | 92 ms    | 8.93002 ms |   3.14197    |    3.14197    |
| 33554432=2^25 | 182 ms   | 17.1488 ms |   3.14196    |    3.14196    |
   
