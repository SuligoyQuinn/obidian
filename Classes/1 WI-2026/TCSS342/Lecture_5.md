# Data Compression
- First step in data storage is encoding in binary
- Always alternatives to standard encoding schemes and some will be more efficient in terms of storage
	- standard encoding schemes are used because they are simple and well known
## Huffman Coding
- *Huffman Coding* is a coding scheme that is designed for text data.
	- Also looks to information about the frequency of occurrence of the characters in the message
### Huffman Coding Algorithm
- Initial step: create a tree with a single node for every character that occurs on the message, label this tree with the character's frequency (weight of the tree)
- Iterative Step: Select the two trees with the lowest weights and merge them into one tree. The weight of the new tree is the sum of the two old weights
	- New tree left node is one old tree, and right node is other old tree
- Final Step: Label the edges of the final tree with 0 for the left edge and 1 for the right edge of every node. Read the code word for each character by spelling out the bits along the path from the root to the leaf node containing the character
## Huffman Coding in Practice
- Huffman coding requires knowledge of the frequency of occurrence of each symbol in the message to be coded
	- When we have the whole message available before encoding we can count the occurrences ahead of time
	- If we do not know we can approximate with known values
- Since we use a different code for every message we must provide the means of decoding the sequence along with the sequence
## Lempel-Ziv
- family of compression algorithms first designed by Lempel and Ziv in 1977
- Zip format uses a variant of LZ77 + Huffman
### Lempel-Ziv Motivation
- Observation that sometimes certain sub-sequences of characters are more common than others.
## Lempel-Ziv Algorithm
- Initialization: Begin with the message $M$ and a dictionary $D$ consisting of one code word per character in the underlying alphabet
- Iterative step: repeat the following steps until the string is encoded
	- Encoding: look for the longest prefix $m$ of $M$ for which there is a code word $w$ in $D$. Encode $m$ with the code word $w$.
	- Updating Directory: Let $c$ be the first character in $M$ after $m$. Add the string $mc$ to the dictionary
## LZW Exception
- Structure: add to $D$ at the new index $k$ a new string of form $ca$ concatenated with the first character of the string at the very index $k$