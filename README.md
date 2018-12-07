# Database-Buffer-Manager

To implement a simplified version of Buffer Manager layer of minibase, without support for concurrency control or recovery.
Disk manager layer was provided already for this project. For page replacement, it uses clock algorithm, which approximates LRU behavior with less overhead.

# Functionality implemented 

The buffer manager manages an array of main memory pages. The array is called the buffer pool, each page is called a frame.  

It provides the following:
1. Pinning and unpinning disk pages to/from frames

2. Allocating and deallocating runs of disk pages and coordinating this with the buffer pool

3. Flushing pages from the buffer pool

4. Getting relevant data

5. The buffer manager is used by access methods, heap files, and relational operators
