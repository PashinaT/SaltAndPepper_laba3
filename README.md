# SaltAndPepper_laba3
Calculation of π on GPU with Monte-Carlo method using CUDA

### Task definition
Given the number of points N, generate a random distribution in (0, 0) − (1, 1) area and calculate the π number
using CPU and GPU. The resulting π values should be printed out along with the execution times.

To do this task, we need to count the number of points in circle - n_in_circle. Then find 4* n_in_circle/N.

#### Input data
• N – number of points;
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
   
