# HuffmanTextZip
**HuffTextZip** is a simple file compression and decompression tool built using the Huffman coding algorithm. It is designed to work specifically with plain text files (`.txt`), reducing their size by encoding frequently used characters with shorter binary codes.

## Features

- Compresses text files using Huffman encoding
- Decompresses encoded files back to original text
- Writes and reads custom headers for metadata
- Easy to compile and run from the command line

## How It Works

1. **Frequency Analysis**: Counts how often each character appears in the text.
2. **Huffman Tree Construction**: Builds a binary tree based on character frequencies.
3. **Encoding**: Assigns binary codes to characters and writes encoded content.
4. **Decoding**: Reconstructs the original text using the Huffman tree.

## Setup and Compilation

Place all `.cpp` and `.h` files in a single directory, along with the input text file.

###Run the following command to compile and run the code:

  g++ -o huffman.exe huffman.cpp main.cpp

After compilation :

# Compression:
  run the command :    ./huffman
  
  -Enter your choice as 1 (for compression)
  
  -Enter the input text file name and the desired name for the compressed output
  
  -The program compresses the file and displays the compression time and ratio
  
  Example:
  
  -Input file:   input.txt
  
  -Compressed file:   compressed.txt.huff   (recommended format)
  
# Decompression:

  run the command :    ./huffman
  
  -Enter your choice as 2 (for decompression)
  
  -Enter the compressed file name and the desired name for the decompressed output file.
  
  -The program decompresses the file and shows the decompression time
  
  Example:
  
  -Compressed file:    compressed.txt.huff
  
  -Decompressed file:    output.txt
  
# Metrics:

  The program prints:
  
    -Compression Time
    
    -Decompression Time
    
    -Compression Ratio


# Sample Test
  Input file:   input.txt
  
  Compressed file:   compressed.txt.huff
  
  Decompressed file:   output.txt

* * You can verify that output.txt exactly matches input.txt, proving the process is lossless.