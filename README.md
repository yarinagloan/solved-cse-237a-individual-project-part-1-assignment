Download Link: https://assignmentchef.com/product/solved-cse-237a-individual-project-part-1-assignment
<br>



The goal of this project is to develop an energy-efficient EDF(Earliest Deadline First) scheduler, which handles multiple workloads controlling sensors running on Raspberry P1 2 (RPi2) . During the course of the project, you will develop a program which characterizes workloads using performance counters (part 1), and an energy-efficient user-level earliest deadline first scheduler program which manages the sensors (part 2) . For more detailed information see the instructions document at the class website.

Individual Project Part 1 Assignment

During the first part of the project, you will setup the development environment for Raspberry P1 2 ( RPi2) , and then measure performance of sample code running on RPi2.

Complete the following steps:

<ol>

 <li>Cross-compile/install the provided Linux kernel and the sample kernel module</li>

</ol>

– Linux kernel source code is available via git: http://seelab.ucsd.edu/~shepherd/cse237a<sub>—</sub>rpikernel.git

– sample kernel code is in ” sample<sub>—</sub>module” directory

<ol start="2">

 <li>Implement a kernel module to access the performance measurement unit ( PMU) using the provided skeleton code</li>

</ol>

– Skeleton code is in “pmuon” directory.

– Kernel module should monitor Li accesses, Li misses, L2 accesses, and L2 misses.

<ol start="3">

 <li>Study how the provided workload execution time changes over various frequency settings and data sizes and access patterns. Modify the provided skeleton code to capture performance counter readings for the workload ( …/memmeasurement/memmeasurement.c) across various program array sizes and CPU frequencies.</li>

 <li>Write a report that provides detailed performance analysis using the implemented kernel module (pmuon) and the user-space program (memmeasurement)</li>

</ol>

– Analyze the program performance over different workload sizes and CPU frequencies.

– Provide at least the following plots for min and max frequency of operation, and for array sizes from iK to 4MB:

<ol>

 <li>execution time vs. array sizes</li>

 <li>Li and L2 cache miss number/rate vs. array sizes</li>

</ol>

<ul>

 <li>execution time vs. cycle count</li>

</ul>

<ol>

 <li>execution time vs. Li and L2 cache miss numbers/rates</li>

 <li>CPU energy vs. CPU frequency for array sizes</li>

</ol>

–