# Computational Intelligence - Lab 1
## Set Cover Problem

In this repository there are two files. The one called "set-cover-threads" exploits a threadpool of 4 threads for each instance examined.
Since the algorithm used to solve the set cover problem employs simulated annealing with temperature and cooling rate, i don't know which initial temperature is best to start with. Therefore, for each instance of the problem, I am using 4 different initial temperatures.
When all the threads (for each instance) have finished, the best solution is displyed, indicating the initial temperature used.

### Results with Fixed Initial Temperature

The following table shows the results obtained in the "set-cover" file with a fixed initial temperature of 7000:

| Instance | Best Cost                 | Num Iterations | Initial Temperature |
|----------|---------------------------|----------------|---------------------|
| 1        | 279.0280561742059         | 1000           | 7000                |
| 2        | 6708.367353432016         | 1000           | 7000                |
| 3        | 1131628.7381450636        | 1000           | 7000                |
| 4        | 107483212.70203757        | 1000           | 7000                |
| 5        | 227458975.22152615        | 1000           | 7000                |
| 6        | 359460786.89962685        | 1000           | 7000                |

### Results with Thread Pool and Different Initial Temperatures

The following table displays the best results obtained after executing the thread pool for each instance, with particular reference to the initial temperature used:

| Instance | Best Cost                 | Num Iterations | Initial Temperature |
|----------|---------------------------|----------------|---------------------|
| 1        | 301.41089319790115        | 1000           | 17000               |
| 2        | 6842.383862045828         | 1000           | 25000               |
| 3        | 1147787.8210480367        | 1000           | 7000                |
| 4        | 105649574.6579897         | 1000           | 7000                |
| 5        | 227435351.39098784        | 1000           | 7000                |
| 6        | 354687657.1795525         | 1000           | 25000               |