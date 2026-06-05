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

Place all `.cpp` and `.h` files in a single directory, along with your input text file.

### Compilation

Open your terminal or command prompt and run the following command to compile the code:

```bash
g++ -o huffman huffman.cpp main.cpp
```

*(Note: On Windows, this will create `huffman.exe`. On Linux/macOS, it will create `huffman`.)*

## Usage

After compiling the program, you can run it to compress or decompress files.

### Running the Program

Execute the following command in your terminal:

```bash
./huffman
```

*(Note: On Windows Command Prompt, you might just need to run `huffman` or `huffman.exe`)*

### 1. Compression

1. When prompted, select option **1** (Compression).
2. Enter the name of the file you want to compress (e.g., `input.txt`).
3. Enter the desired name for the compressed output file (e.g., `compressed.huff`).

The program will compress the file and display the compression time and ratio.

### 2. Decompression

1. Run the program again and select option **2** (Decompression).
2. Enter the name of the compressed file (e.g., `compressed.huff`).
3. Enter the desired name for the decompressed output file (e.g., `output.txt`).

The program will decompress the file and show the decompression time.

## Metrics

After processing, the program prints useful statistics:
- **Compression Time**: Time taken to encode the file.
- **Decompression Time**: Time taken to decode the file.
- **Compression Ratio**: The size reduction achieved.

## Sample Test

1. Create a text file named `input.txt` with some content.
2. Run the program to compress it into `compressed.huff`.
3. Run the program again to decompress `compressed.huff` into `output.txt`.
4. **Verification**: Check that `output.txt` exactly matches `input.txt`. This proves the compression and decompression process is lossless.