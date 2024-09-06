# FileZipper: A Huffman Encoding-Based File Compression and Decompression Utility

**FileZipper** is a C++ project that implements a file compression and decompression utility using the **Huffman Encoding** algorithm. Huffman coding is a well-known lossless data compression technique, which reduces file sizes by encoding characters based on their frequency of occurrence in the input data.

## Features:
- **Lossless Compression:** Efficiently compresses files without any data loss, ensuring that the original content is perfectly restored upon decompression.
- **Huffman Encoding:** Implements the core algorithm to generate binary representations for characters based on frequency, leading to optimized file storage.
- **File Decompression:** Accurately decompresses Huffman-encoded binary files back to their original form.
- **Support for Any File Type:** Capable of compressing and decompressing text-based or binary files.

## How It Works:
### 1. Compression:
- The program reads the input file and calculates the frequency of each character.
- A Huffman Tree is constructed based on the character frequencies.
- Each character is assigned a binary code (shorter codes for more frequent characters).
- The original file is then encoded using these binary codes, resulting in a compressed binary output file.

### 2. Decompression:
- The compressed binary file is read and decoded back into its original form using the Huffman Tree.
- The program removes any added padding to ensure the file content is restored accurately.

## Use Cases:
- **Storage Efficiency:** Reduce file sizes for more efficient storage.
- **Data Transmission:** Compress files for faster data transfer while ensuring no data is lost.
- **Learning Purposes:** Gain a deeper understanding of how Huffman encoding works for file compression.
