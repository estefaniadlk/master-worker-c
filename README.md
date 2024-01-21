# master-worker-c

Master-Worker Binary-to-Decimal Conversion Project

In this collaborative project, our team undertook the implementation of a binary-to-decimal conversion using advanced inter-process communication techniques, including message queues, shared memory, semaphores, and signals.

Master (Server):

Creates a message queue, attaches to shared memory, and initializes semaphores for worker coordination.
Generates a matrix representing the binary number, with the size of the matrix equal to the number of workers.
Coordinates the reception of binary digits from workers (filled matrix) and performs the conversion to obtain the decimal equivalent.
Worker (Client):

Attaches to shared memory and receives the necessary semaphore.
Each worker is uniquely identified by its process id, corresponding to its designated cell in the matrix.
Randomly assigned a binary digit (0 or 1) for processing.
This project showcases our team's expertise in leveraging low-level inter-process communication mechanisms to efficiently distribute tasks among multiple processes for the conversion of binary numbers to their decimal equivalents. The use of message queues, shared memory, semaphores, and signals demonstrates our proficiency in handling complex parallel computing tasks in a collaborative environment.
