# Chapter 02: Working With Text Data

This notebook demonstrates how to build a language model from scratch using Byte Pair Encoding (BPE) and PyTorch. The steps include downloading a text file, tokenizing the text, creating a dataloader, and generating token embeddings.

## Steps

1. **Download the Text File**
   - The notebook starts by downloading a text file from a specified URL using `urllib.request`.

2. **Read the File**
   - The downloaded file is read and the total number of characters is printed.

3. **Byte Pair Encoding (BPE)**
   - The `tiktoken` library is used to tokenize the text using BPE.

4. **Data Sampling with a Sliding Window**
   - A custom `TextDataset` class is implemented to create input and target sequences using a sliding window approach.

5. **Creating a DataLoader**
   - A `create_dataloader` function is defined to create a PyTorch DataLoader for batching the tokenized text.

6. **Creating Token Embeddings**
   - A token embedding layer is created using PyTorch's `nn.Embedding`.


