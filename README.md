# Shrink-It
File compression and decompression using Huffman coding


# Functions:
createArr():
Initializes an array of 128 nodes, each representing a character with its frequency set to 0.

traverse(Node *r, string str):
Traverses the Huffman tree and assigns binary codes to leaf nodes (0 for left child, 1 for right child).

binToDec(string inStr):
Converts a binary string to its decimal equivalent.

decToBin(int inNum):
Converts a decimal number to an 8-bit binary string.

buildTree(char a_code, string &path):
Builds the Huffman tree based on the character and its Huffman code.

createMinHeap():
Reads characters from the input file and increments their frequencies in the arr array. Creates a min heap of nodes for characters with non-zero frequencies.

createTree():
Constructs the Huffman tree using the min heap.

createCodes():
Traverses the Huffman tree and assigns Huffman codes to characters.

saveEncodedFile():
Saves the compressed data to an output file. It includes meta-data (Huffman tree structure) and encoded characters.

saveDecodedFile():
Reads the Huffman tree structure and decodes the compressed data, saving the output to a file.

getTree():
Reads the Huffman tree structure from the input file.

compress():
Calls functions to perform compression: creates the Huffman tree, assigns codes, and saves the encoded file.

decompress():
Calls functions to perform decompression: reads the Huffman tree, decodes the file, and saves the output.
