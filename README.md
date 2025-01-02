Name: Ranjana P
Company: CODTECH IT SOLUTION
ID: CT08FPL
Domain: C++ Programming
Duration: 20 December 2024 to 20 January 2025
Mentor: Santhosh N

Overview of the Program

This C++ program demonstrates how to compress and decompress files efficiently using multithreading to optimize performance. It leverages the Run-Length Encoding (RLE) algorithm to compress the data and splits the file into chunks for parallel processing.


---

Key Features

1. Multithreading:

The program uses the std::thread library to process chunks of the file concurrently.

Threads improve performance, especially for large files, by utilizing multiple CPU cores.



2. Run-Length Encoding (RLE):

A simple compression algorithm that replaces consecutive occurrences of a character with the character followed by its count.

Example: aaabbbccc → a3b3c3.



3. File Handling:

Reads the input file in chunks.

Writes compressed and decompressed data into separate output files.



4. Performance Optimization:

By dividing the file into chunks and processing them simultaneously, the program reduces execution time compared to a single-threaded approach.





---

Program Workflow

1. Input File:

The program reads data from an input file (e.g., input.txt).



2. Compression:

Splits the file into chunks and processes each chunk using multiple threads.

Each chunk is compressed using RLE and combined into the compressed.txt file.



3. Decompression:

Reads the compressed file, splits it into chunks, and decompresses each chunk using multiple threads.

The decompressed data is written into decompressed.txt.



4. Output:

compressed.txt: The compressed representation of the input file.

decompressed.txt: The reconstructed original file, matching the input file.





---

Advantages

Improved Performance: Multithreading allows faster processing of large files.

Scalable Design: Handles files of varying sizes efficiently.

Easy to Extend: The program can be adapted to use more complex compression algorithms.



---

Example Execution

1. Input File (input.txt):

aaabbbcccaaa


2. Compressed File (compressed.txt):

a3b3c3a3


3. Decompressed File (decompressed.txt):

aaabbbcccaaa

Applications

Data Storage: Compressing files to save disk space.

Data Transfer: Reducing file size for faster transmission over networks.

Learning Example: Demonstrates multithreading and file operations in C++.


This program showcases how multithreading can significantly improve performance for tasks like file compression and decompression.

![image](https://github.com/user-attachments/assets/0998e57a-8312-44b8-8f96-a85f66b863b5)


