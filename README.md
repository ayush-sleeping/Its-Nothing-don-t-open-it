* [PCB block](#PCB-block)
* [Process lifecycle](#Process-lifecycle)
* [What is memory](#What-is-memory)
* [Types of memory](#Types-of-memory)

<hr>

* [Operating System](#Operating-System)
* [Dual mode Operation](#Dual-mode-Operation)
* [Timer](#Timer)
* [Function of operating system](#Function-of-operating-system)
* [Web based computing](#Web-based-computing)
* [Peer to peer computing](#Peer-to-peer-computing)
* [Operating system services](#Operating-system-services)
* [System call](#System-call)
* [Types of system calls](#Types-of-system-calls)
* [Threads](#Threads)
* [Schedulers](#Schedulers)
* [Types of schedulers](#Types-of-schedulers)
* [Thread in detail](#Thread-in-detail)
* [Multi threadng](#Multi-threadng)
<hr>

* [CPU Scheduling](#CPU-Scheduling)
* [Deadlock](#Deadlock)
* [Deadlock condition](#Deadlock-condition)
* [Swapping](#Swapping)
* [Virtual memory](#Virtual-memory)
* [Trashing](#Trashing)
* [Concept of file](#Concept-of-file)
* [Linear list](#Linear-list)
* [Hash table](#Hash-table)
<hr>
<br>

## PCB block
Process Control Block is a data structure that contains information of the process related to it. The process control block is also known as a task control block, entry of the process table, etc.

It is very important for process management as the data structuring for processes is done in terms of the PCB. It also defines the current state of the operating system.
<br>
<br>

## Process lifecycle
The process life cycle can be defined by a state diagram. Which has states representing the execution status of process at various time and transitions. That shows the changes in the execution status. To maintain the management information about a process the operating system uses the process control block (PCB).

<br>
<br>

## What is memory
Computer memory is any physical device capable of storing information temporarily, like RAM (random access memory), or permanently, like ROM (read-only memory). Memory devices utilize integrated circuits and are used by operating systems, software, and hardware.

<br>
<br>

## Types of memory
here are two types of memories: <br>

1. Primary memory (RAM,  ROM ) <br>
2. Secondary memory () <br>
<br>
<br>

## Operating System 
An operating system is the most important software that runs on a computer. It manages the computer's memory and processes, as well as all of its software and hardware. It also allows you to communicate with the computer without knowing how to speak the computer's language. Without an operating system, a computer is useless.
<br>
<br>

## Dual mode Operation
The dual-mode operations in the operating system protect the operating system from illegal users. We accomplish this defense by designating some of the system instructions as privileged instructions that can cause harm. The hardware only allows for the execution of privileged instructions in kernel mode. An example of a privileged instruction is the command to switch to user mode. Other examples include monitoring of I/O, controlling timers and handling interruptions. <br>

To ensure proper operating system execution, we must differentiate between machine code execution and user-defined code. Most computer systems have embraced offering hardware support that helps distinguish between different execution modes. We have two modes of the operating system: user mode and kernel mode.
<br>
<br>

## Timer
As all we know that it is only the operating system that has full control over the CPU,and it is the primary duty of operating system to prevent user programs from getting stuck into an infinite loop or not calling to system services and never returning control back to the operating system.To accomplish all those services an operating system uses a device known as Timer.
<br>
<br>

## Function of operating system
1. Memory Management
2. Processor Management/Scheduling
3. Device Management
4. File Management
5. Security
7. Accounting
8. Other Functions
<br>
<br>


## Web based computing
A Web Operating System is an internet based user interface that allows people to access applications not stored on their computers but completely or partly on Internet. It is a dummy operating system that does not directly interact with computer hardware and depends on traditional operating system to work. In other words, it is an interface for distributed computing system such as cloud. 
<br>
<br>

## Peer to peer computing
The peer to peer computing architecture contains nodes that are equal participants in data sharing. All the tasks are equally divided between all the nodes. The nodes interact with each other as required as share resources.
Each computer in the peer to peer network manages itself. So, the network is quite easy to set up and maintain.
In the client server network, the server handles all the requests of the clients. This provision is not required in peer to peer computing and the cost of the server is saved.
<br>
<br>

## Operating system services
An Operating System supplies different kinds of services to both the users and to the programs as well. It also provides application programs (that run within an Operating system) an environment to execute it freely. It provides users the services run various programs in a convenient manner. <br>
Here is a list of common services offered by an almost all operating systems: <br>
User Interface <br>
Program Execution <br>
File system manipulation <br>
Input / Output Operations <br>
Communication <br>
Resource Allocation <br>
Error Detection <br>
Accounting <br>
Security and protection <br>
<br>
<br>

## System call
The interface between a process and an operating system is provided by system calls. In general, system calls are available as assembly language instructions. They are also included in the manuals used by the assembly level programmers. System calls are usually made when a process in user mode requires access to a resource. Then it requests the kernel to provide the resource via a system call.
<br>
<br>

## Types of system calls
Types of System Calls <br>
There are mainly five types of system calls. These are explained in detail as follows − <br>

Process Control <br>


File Management <br>


Device Management <br>


Information Maintenance <br>

Communication <br>
<br>
<br>

## Threads
A thread is a single sequential flow of execution of tasks of a process so it is also known as thread of execution or thread of control. There is a way of thread execution inside the process of any operating system. Apart from this, there can be more than one thread inside a process. Each thread of the same process makes use of a separate program counter and a stack of activation records and control blocks. Thread is often referred to as a lightweight process.
<br>
<br>

## Schedulers
Operating system uses various schedulers for the process scheduling described below. <br>
1. Long term scheduler <br>
Long term scheduler is also known as job scheduler. It chooses the processes from the pool (secondary memory) and keeps them in the ready queue maintained in the primary memory. <br>
2. Short term scheduler
Short term scheduler is also known as CPU scheduler. It selects one of the Jobs from the ready queue and dispatch to the CPU for the execution. <br>
3. Medium term scheduler
Medium term scheduler takes care of the swapped out processes.If the running state processes needs some IO time for the completion then there is a need to change its state from running to waiting. <br>
<br>

## Types of schedulers
1. Long term scheduler <br>
2. Short term scheduler <br>
3. Medium term scheduler
<br>
<br>

## Thread in detail
A thread is a path of execution within a process. A process can contain multiple threads.
<br>
<br>

## Multi threadng
A thread is also known as lightweight process. The idea is to achieve parallelism by dividing a process into multiple threads. For example, in a browser, multiple tabs can be different threads. MS Word uses multiple threads: one thread to format the text, another thread to process inputs, etc. More advantages of multithreading are discussed below
<br>
<br>
<hr>
<hr>
 
## CPU Scheduling
CPU scheduling is a process that allows one process to use the CPU while the execution of another process is on hold(in waiting state) due to unavailability of any resource like I/O etc, thereby making full use of CPU. The aim of CPU scheduling is to make the system efficient, fast, and fair.
<br>
<br>

## Deadlock
A Deadlock is a situation where each of the computer process waits for a resource which is being assigned to some another process. In this situation, none of the process gets executed since the resource it needs, is held by some other process which is also waiting for some other resource to be released.
<br>
<br>

## Deadlock condition
here are 4 conditions necessary for the occurrence of a deadlock. They can be understood with the help of the above illustrated example of staircase : <BR>
Mutual Exclusion: <br>
Hold and Wait: <br>
No Preemption: <br>
Circular Wait: <br>
<br>
<br>

## Swapping
Swapping is a process of swapping a process temporarily to a secondary memory from main memory which is fast as compared to secondary memory. But as RAM is of less size so the process that is inactive is transferred to secondary memory. The main part of swapping is transferred time and the total time directly proportional to the amount of memory swapped.
<br>
<br>

## Virtual memory
Virtual Memory is a storage scheme that provides user an illusion of having a very big main memory. This is done by treating a part of secondary memory as the main memory.
<br>
In this scheme, User can load the bigger size processes than the available main memory by having the illusion that the memory is available to load the process.
<br>
<br>

## Trashing
thrash is the poor performance of a virtual memory (or paging) system when the same pages are being loaded repeatedly due to a lack of main memory to keep them in memory. Depending on the configuration and algorithm, the actual throughput of a system can degrade by multiple orders of magnitude.
<br>
<br>

## Concept of file
Computer store information in storage media such as disk, tape drives, and optical disks. The operating system provides a logical view of the information stored in the disk. This logical storage unit is a file.
<br>
The information stored in files are non-volatile, means they are not lost during power failures. A file is named collection of related information that is stored on physical storage.
<br>
<br>


## Linear list
The simplest method of implementing a directory is to use a linear list of file names with pointers to the data blocks. This method is simple to program but time consuming to execute. The real disadvantage of a linear list of directory entries is that finding a file requires a linear search.
<br>
<br>
 
## Hash table 
Another data structure used for a file directory is a hash table. With this method, a linear list stores the directory entries but a hash data structure is also used. The hash table takes a value computed from the file name and returns a pointer to the file name in the linear list. The major difficulties with a hash table are its generally fixed size and the dependence of the hash function on that size.
<br>
<br>
<hr>
<hr>
