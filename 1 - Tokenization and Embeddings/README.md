# Week 1 - Tokenization and Embeddings

This week, we dive into the foundational steps of making an AI model understand text: **Tokenization** and **Embeddings**. These processes are crucial for converting raw text into a format that machine learning models can process and learn from.

## Tokenization

### Introduction to Tokenization
Tokenization is the process of converting words or sub-words into numerical representations. This allows text to be represented as a list of numbers, which is essential for further processing by AI models.

- **Tokenization Intro Video**: [Watch Here](https://www.youtube.com/watch?v=fNxaJsNG3-s)
  
### Byte Pair Encoding (BPE)
One of the most common and widely used tokenization algorithms is **Byte Pair Encoding (BPE)**. This method is particularly effective for handling sub-word tokenization.

- **Byte Pair Encoding Video**: [Watch Here](https://www.youtube.com/watch?v=hL4ZnAWSyuU) (First 2 minutes)

### Task 1.1 - Why Sub-word Tokenization is Optimal
**Question**: Why is sub-word tokenization more optimal than word-by-word tokenization?

**Reference**: [Tokenization Blog](https://aman.ai/primers/ai/tokenizer/)

## Embeddings

### Introduction to Embeddings
After tokenizing text into a list of numbers, the next step is to create **embeddings**. Embeddings provide semantic meaning to the tokenized numbers, enabling the model to understand the context and relationships between words.

- **Embedding Intro Video**: [Watch Here](https://www.youtube.com/watch?v=gQddtTdmG_8&t)

### Types of Embeddings
There are three main types of embeddings:
1. **Count-Based Embeddings**: These methods create sparse embeddings and include approaches like Bag of Words (BoW), TF-IDF, and BM25.
   - **Bag of Words (BoW)**: Represents a sentence as a vector of word counts.
     - Example: If the vocabulary is `["the", "cat", "sat", "on", "mat", "dog", "log"]`, the sentence `"the dog sat on the log"` is represented as `[2, 0, 1, 1, 0, 1]`.
   - **TF-IDF and BM25**: [Watch Here](https://www.youtube.com/watch?v=ziiF1eFM3_4&) (First 20 minutes)

2. **Co-occurrence/Static Embeddings**: The most notable method in this category is **Word2Vec** (2013), which revolutionized NLP.
   - **Word2Vec Video**: [Watch Here](https://www.youtube.com/watch?v=gQddtTdmG_8&)

3. **Contextual/Dynamic Embeddings**: We will cover this type later in the course.

### Task 1.2 - Creating and Visualizing Embeddings
**Task**: 
1. Create a dataset containing two classes of sentences, each with roughly the same length (preferably 7-10 sentences per class).
2. Use the [sentence-transformers/all-MiniLM-L6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) model to generate embeddings for these sentences.
3. Reduce the dimensionality of the embeddings to 2D using **t-SNE** (a method for reducing higher-dimensional vectors to lower dimensions).
4. Visualize the embeddings in a 2D space and observe if the sentences from the two classes are separately clustered.
5. Reflect on the type of embedding method used.

**Deadline**: February 10th, Monday E.O.D

## Note
You are expected to watch all the provided videos and complete the two tasks by the deadline.

---

This README provides a structured overview of the topics covered in Week 1, along with the tasks and resources needed to complete them. Make sure to follow the instructions carefully and reach out if you have any questions!