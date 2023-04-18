# Parallelizing-CPU-Scheduling-Algorithms

To prove the performance improvement for parallelizable serial codes with the help of parallelizing various serial scheduling algorithms and comparing them.

# ABSTRACT
Task scheduling in parallel processing is a technique in which processes are assigned to different processors. Task scheduling in parallel processing uses different types of algorithms and techniques which are used to reduce the number of delayed jobs. Nowadays there is a different kind of scheduling algorithms and techniques used to reduce the execution time of tasks scheduling of jobs in parallel is becoming the subject of much research. The problem of job scheduling is to determine how resources should be shared in order to maximize the system’s utility. This problem has been extensively studied for well over a decade. In this paper, we will first discuss the execution time of scheduling algorithm (FIFO, ROUND ROBIN, SJF, PRIORITY SCHEDULING) in series and parallel, we discuss how deployed scheduling policies can be improved to meet existing requirements, specific research challenges and future scope.

# INTRODUCTION
The Central Processing Unit (CPU) is the brain of the computer system so it should be utilized efficiently. CPU Scheduling is one of the most important concepts of Operating System. Sharing of computer resources among multiple processes is called scheduling.

          The various CPU scheduling algorithms are: -

1. FCFS CPU scheduling: - In this scheduling the process that requests the CPU first is allocated to CPU first. This algorithm is easy to understand and implement but poor in performance as average wait time is very high.

2. SJF CPU scheduling: - In this scheduling the process with the shortest CPU burst time is allocated to CPU first. It is the best way to reduce time. Here the actual time taken by the process to execute is already known by the processor

3. Priority scheduling: - In this scheduling the process with high priority is allocated to CPU first, and process with the same priority are executed in FCFS manner. Priority can be decided on the basis of the memory allocation, or on the basis of the time or on the basis of some resource requirements.

4. Round Robin scheduling: - It is same as FCFS scheduling with pre-emption is added to switch between processes. A static Time Quantum (TQ) is used in this CPU Scheduling. Once a process is executed for given time period that process is preemptied and other process executes for given time period. A process known as Context switching is used to save states of preemptied processes while execution.
The various scheduling parameters for the selection of the scheduling algorithm are :

Context Switch: A context switch is process of storing and restoring context (state) of a pre-empted process, so that execution can be resumed from same point at a later time. Context switching is wastage of time and memory that leads to the increase in the overhead of scheduler, so the goal of CPU scheduling algorithms is to optimize only these switches.

1. Throughput: Throughput is defined as number of processes completed in a period of time. Throughput is less in round robin scheduling. Throughput and context switching are inversely proportional to each other.

2. CPU Utilization: It is defined as the fraction of time CPU is in use. Usually, the maximize the CPU utilization is the goal of the CPU scheduling

3. Turnaround Time: Turnaround time is defined as the total time which is spend to complete the how long it takes the time to execute that process. 4. Waiting Time: Waiting time is defined as the total time a process has been waiting in ready queue.

5. Response Time: Respond Time is better measure than turnaround time. Response time is defined as the time used by the system to respond to the any particular process. Thus the response time should be as low as possible for the best scheduling.

6. Load average: It is the average number of processes residing in the
ready queue waiting for their turn to get into the CPU. The various characteristics of good scheduling algorithm are [3]:

1. Minimum context switches. 
2. Maximum CPU utilization.
3. Maximum throughput.
4. Minimum turnaround time. 
5. Minimum waiting time
