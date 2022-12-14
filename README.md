# PThreads

What are PThreads?

The default multithreading mechanism for the UNIX system is PThreads, which is quite concrete. The acronym PThreads stands for POSIX threads, while POSIX stands for Portable Operating System Interface, a sort of interface that the operating system is required to support. The threading APIs that the operating system must offer are defined by PThreads in POSIX.

PThreads performs well on multiprocessor or multi-core systems where the process flow may be scheduled to execute on a different processor, increasing speed through parallel or distributed processing. Because the system does not create a new system, virtual memory space, or environment for the process, threads do not incur any additional overhead when compared to forking or creating a new process.

Advantages:

Adopting PThreads is mostly done to enhance program performance.
A thread can be created with substantially less operating system overhead when compared to the cost of creating and administering a process. Process management uses more system resources than thread management does.

A process's address space is shared by all of its threads. In many situations, inter-thread communication is more effective and convenient to employ than inter-process communication. Applications that are threaded have a number of advantages versus applications that are not threaded, including potential performance gains.




Monte-Carlo Method:-

Consider throwing darts at a square dartboard with two-foot-long sides and a bullseye that is located at the board's center at random. Consider as well that the square dartboard has a circle etched into it. The circle has a radius of 1 foot and a surface area of square feet. Given that the ratio of the area of the circle to the area of the square is π/4, the number of darts that hit inside the circle should roughly satisfy the following equation if the locations that are hit by the darts are randomly distributed (and we always hit the square):

number_in_circle / total_number_of_tosses = π / 4.
