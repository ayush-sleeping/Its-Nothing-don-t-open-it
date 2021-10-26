# DBMS short viva revision :- 
## Some Basic Concept of DBMS _
* [Database Management System](#Database-Management-System)
* [Characteristics of DBMS](#Characteristics-of-DBMS)
* [Advantages of DBMS](#Advantages-of-DBMS)
* [Disadvantages of DBMS](#Disadvantages-of-DBMS)

## Unit 1:

* [Stored Procedures](#Stored-Procedures)
  * [Advantages of stored procedures](#Advantages-of-stored-procedures)
  * [Disadvantages of stored procedures](#Disadvantages-of-stored-procedures)
* [System defined stored procedure](#System-defined-stored-procedure)
* [User defined stored procedure](#User-defined-stored-procedure)
  * [Benefit of stored procedure](#Benefit-of-stored-procedure)
* [Triggers](#Triggers)
  * [Purpose of trigger](#Purpose-of-trigger)
  * [Nested Triggers](#Nested-Triggers)
* [Sequence](#Sequence)
  * [How to drop a sequence](#How-to-drop-a-sequence)
* [Types of file organisation](#Types-of-file-organisation)
  * [File Organisation](#File-Organisation)
  * [Hash file organisation](#Hash-file-organisation)
* [Indexes Sequential Access Method](#Indexes-Sequential-Access-Method)
* [B+Tree](#B+Tree)
* [Clustered Tables](#Clustered-Tables)
* [Index](#Index)
* [Indexing Types](#Indexing-Types)
* [Cost model](#Cost-model)
* [Heap file organisation](#Heap-file-organisation)
* [Sequential file organisation](#Sequential-file-organisation)

## Unit 2

## Unit 3 

* [ACID Properties ](#ACID-Properties )
* [Serizable Schedule](#Serizable-Schedule )
* [Explain read write blocks](#Explain-read-write-blocks)
* [Shared locks](#Shared-locks)
* [Exclusive locks](#Exclusive-locks)
* [Deadlock Handling](#Deadlock-Handling)
* [ARIES algorithm](#ARIES-algorithm)
* [RECOVERY from system crash](#RECOVERY-from-system-crash)
* [SQL in Rollback](#SQL-in-Rollback)
* [timestamp based protocoll](#timestamp-based-protocoll)
* [concurenccy control](#concurenccy-control)
* [how to make permanent change in database ](#how-to-make-permanent-change-in-database )
* [Shadow pagging](#Shadow-pagging)



<hr>
<br>
<br>



## Database Management System
* Database management system is a software which is used to manage the database. For example: MySQL, Oracle, etc are a very popular commercial database which is used in different applications.
* DBMS provides an interface to perform various operations like database creation, storing data in it, updating data, creating a table in the database and a lot more.
* It provides protection and security to the database. In the case of multiple users, it also maintains data consistency.

<br>
<br>

## Characteristics of DBMS
* It uses a digital repository established on a server to store and manage the information.
* It can provide a clear and logical view of the process that manipulates data.
* DBMS contains automatic backup and recovery procedures.
* It contains ACID properties which maintain data in a healthy state in case of failure.

<br>
<br>

## Advantages of DBMS
* Controls database redundancy
* Data sharing
* Easily Maintenance
* Reduce time
* Backup
* multiple user interface

<br>
<br>

## Disadvantages of DBMS
* Cost of Hardware and Software
* Size
* Complexity
* Higher impact of failure

<br>
<br>

## Stored Procedures
Stored Procedures are created to perform one or more DML operations on Database. It is nothing but the group of SQL statements that accepts some input in the form of parameters and performs some task and may or may not returns a value.
<br>
<br>

## Advantages of stored procedures
* Since stored procedures are compiled and stored, whenever you call a procedure the response is quick.

* you can group all the required SQL statements in a procedure and execute them at once.

* Since procedures are stored on the database server which is faster than client. You can execute all the complicated quires using it, which will be faster.

* Using procedures, you can avoid repetition of code moreover with these you can use additional SQL functionalities like calling stored functions.


<br>
<br>

## Disadvantages of stored procedures
The only disadvantage of a Stored Procedure is that it can be executed only in the database and utilizes more memory in the database server.
<br>
<br>

## System defined stored procedure
The stored procedure accepts the parameters and executes the T-SQL statements in the procedure, returns the result set if any.
<br>
<br>

## User defined stored procedure
User defined stored procedures are created by database developers or database administrators. These SPs contains one more more SQL statements to select, update, or delete records from database tables. User defined stored procedure can take input parameters and return output parameters
<br>
<br>

## Benefit of stored procedure
* Reduce network traffic
* Security
* Maintainability
<br>
<br>

## Triggers
Triggers are the SQL statements that are automatically executed when there is any change in the database. The triggers are executed in response to certain events(INSERT, UPDATE or DELETE) in a particular table. These triggers help in maintaining the integrity of the data by changing the data of the database in a systematic fashion.
<br>
<br>

## Purpose of trigger
1. Triggers provide a way to check the integrity of the data. When there is a change in the database the triggers can adjust the entire database.
2. Triggers help in keeking User Interface lightweight. Instead of putting the same function call all over the application you can put a trigger and it will be executed.
<br>
<br>

## Nested Triggers
A trigger that contains data modification logic within itself is called a nested trigger. A trigger can also contain INSERT, UPDATE and DELETE logic within itself, so when the trigger is fired because of data modification it can also cause another data modification, thereby firing another trigger

<br>
<br>

## Sequence
A sequence is a user-defined schema bound object that generates a sequence of numeric values according to the specification with which the sequence was created
<br>
<br>

## How to drop a sequence
The syntax to a drop a sequence in Oracle is: DROP SEQUENCE sequence_name; sequence_name. The name of the sequence that you wish to drop.
<br>
<br>

## Types of file organisation
1. Types of file organization are as follows:
2. Sequential file organization.
3. Heap file organization.
4. Hash file organization.
5. B+ file organization.
6. Indexed sequential access method (ISAM)
7. Cluster file organization.
<br>
<br>

## File Organisation
File Organization in DBMS: A database contains a huge amount of data, which is stored is in the physical memory in the form of files. A file is a set of multiple records stored in the binary format.
<br>
<br>

## Hash file organisation
In this method of file organization, hash function is used to calculate the address of the block to store the records. The hash function can be any simple or complex mathematical function. The hash function is applied on some columns/attributes – either key or non-key columns to get the block address. Hence each record is stored randomly irrespective of the order they come. 
<br>
<br>

## Indexes Sequential Access Method
ISAM method is an advanced sequential file organization. In this method, records are stored in the file using the primary key. An index value is generated for each primary key and mapped with the record. This index contains the address of the record in the file.
<br>
<br>

## B+Tree
The B+ tree is a balanced binary search tree. It follows a multi-level index format.
In the B+ tree, leaf nodes denote actual data pointers. B+ tree ensures that all leaf nodes remain at the same height.
<br>
<br>

## Clustered Tables
A cluster is a schema object that contains data from one or more tables, all of which have one or more columns in common. 
<br>
<br>

## Index
Indexing is a data structure technique to efficiently retrieve records from the database files based on some attributes on which the indexing has been done. Indexing in database systems is similar to what we see in books.
<br>
<br>



## Indexing Types
* Primary Indexing
  * Dense Index
  * Sparse Index
* Secondary Indexing
<br>
<br>

## Cost model
a cost model is a mathematical algorithm or equation for estimating costs of a product or project.
<br>
<br>

## Heap file organisation
Here records are inserted at the end of the file as and when they are inserted. There is no sorting or ordering of the records.  Once the data block is full, the next record is stored in the new block. This new block need not be the very next block.
<br>
<br>

## Sequential file organisation
A sequential file contains records organized by the order in which they were entered. The order of the records is fixed. Records in sequential files can be read or written only sequentially. After you place a record into a sequential file, you cannot shorten, lengthen, or delete the record.
<br>
<br>

##

<br>
<br>
<hr>

## SQL in Rollback
a rollback is an operation which returns the database to some previous state. Rollbacks are important for database integrity, because they mean that the database can be restored to a clean copy even after erroneous operations are performed.

## timestamp based protocoll
Timestamp based Protocol in DBMS is an algorithm which uses the System Time or Logical Counter as a timestamp to serialize the execution of concurrent transactions.
<br>
<br>

## concurenccy control
Concurrency Control is the management procedure that is required for controlling concurrent execution of the operations that take place on a database.

But before knowing about concurrency control, we should know about concurrent execution
<br>

## how to make permanent change in database 
the commit statement is used to save changes permanetly to the database so that they will become visible yo consequent transaction 
<br>

## Shadow pagging 
Shadow Paging is recovery technique that is used to recover database. In this recovery technique, database is considered as made up of fixed size of logical units of storage which are referred as pages. pages are mapped into physical blocks of storage
<br>
<br>

## Unit 3 
## ACID Properties 
In computer science ACID (Atomicity consistensy isolation durability ) is a set of properties of database transaction in context of database a sequence of a database operations thatr specifies the ACID properties .
<br>
<br>

## Serizable Schedule 
if execution of all transaction is a concurrent schedule produces same result as in serial schedule then it is called serizable schedule
<br>
<br>

## Explain read write blocks 
ReadWriteLock is an advanced thread lock mechanism. It allows multiple threads to read a certain resource, but only one to write it, at a time. The idea is, that multiple threads can read from a shared resource without causing concurrency errors.
<br>

## Shared locks
shared lock is qalso known as read lock is acquried on the transaction when concurrent transaction granted the permission for read access of the data 
<br>

## Exclusive locks 
When a statement modifies data, its transaction holds an exclusive lock on data that prevents other transactions from accessing the data. This lock remains in place until the transaction holding the lock issues a commit or rollback.
<br>
<br>

## Deadlock Handling
A system is said to be in a state of deadlock . if every transaction in schedule is waiting for another transaction in schedule to release a lock of some data item 
<br>
<br>

## DCL statement 
The data control language statements are used to create a priviliges to permits users access and manipulations of the database 
<br>

## REVOKE statements 
 REVOKE statements is used to remove priviliges given to users by system 
<br>
<br>

## Define transaction 
A transaction is a program unit whose execution may or may not change the contents of a database. The transaction concept in DBMS is executed as a single unit
<br>
<br>

## ROLLBACK statement
The ROLLBACK statement is the inverse of the COMMIT statement. It undoes some or all database changes made during the current transaction. ... If the statement fails, a rollback to this implicit savepoint is done
<br>
<br>

## ARIES algorithm 
ARIES stands for “Algorithm for Recovery and Isolation Exploiting Semantics.” It was designed to support the needs of industrial strength transaction processing systems. 
<br>
<br>

## RECOVERY from system crash 
- Recovery from system crash can be done by using three phrase 
1. Analysis phrases 
2. REDO phrases
3. Undo phrases 




## OS Viva Revision

* [Memory Management](#Memory-Management)
* [Traversal in Scheduling](#Traversal-in-Scheduling)
* [Dynamic memory allocation](#Dynamic-memory-allocation)
* [fragmentation](#fragmentation)
* [](#)


<hr>

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

## Memory Management
The term Memory can be defined as a collection of data in a specific format. It is used to store instructions and processed data. The memory comprises a large array or group of words or bytes, each with its own location. The primary motive of a computer system is to execute programs. 

<br>

## Traversal in Scheduling

<br>

## Dynamic memory allocation
Dynamic memory allocation is when an executing program requests that the operating system give it a block of main memory.
<br>

## fragmentation
Fragmentation is an unwanted problem where the memory blocks cannot be allocated to the processes due to their small size and the blocks remain unused. It can also be understood as when the processes are loaded and removed from the memory they create free space or hole in the memory and these small blocks cannot be allocated to new upcoming processes and results in inefficient use of memory. Basically, there are two types of fragmentation: <br>

Internal Fragmentation <br>
External Fragmentation

<br>

## Memory Management

<br>

## Memory Management

<br>

## Memory Management

<br>

## Memory Management

<br>

## Memory Management

<br>

## Memory Management

<br>

## Memory Management

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
An operating system is the most important software that runs on a computer. It manages the computer's memory and processes, as well as all of its software and hardware. It also allows you to communicate with the computer without knowing how to speak the computer's language. Without an operating system, a computer is useless. <br>
Types of Operating Systems
Batch OS
Distributed OS
Multitasking OS
Network OS
Real-OS
Mobile OS
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
