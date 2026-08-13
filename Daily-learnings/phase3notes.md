# Phase 3 — Embeddings & Vector Search: Completed Notes

**Verified progress: Lessons 1–14 complete.**

1. **What Are Embeddings?** — An embedding is a vector of numbers that represents the meaning of text or other data.
2. **How Text Becomes Vectors** — Text is tokenized, processed in context by an embedding model, and returned as a fixed-size vector. A token ID is not an embedding.
3. **Semantic Meaning & Similarity** — Text with related meaning usually has nearby or similar vectors, even when the words are different.
4. **Dimensions & Embedding Space** — Dimensions are the number of values in a vector. The full vector represents meaning; one dimension usually does not have one simple human meaning.
5. **Cosine Similarity** — Compares vector direction. Higher is more similar; +1 is the same direction, 0 is perpendicular, and -1 is opposite direction.
6. **Euclidean Distance & Dot Product** — Euclidean distance is straight-line distance, so lower is more similar. Dot product uses direction and magnitude, so higher is generally more similar. With normalized vectors, dot product and cosine can give the same ranking.
7. **Semantic Search** — Convert the query into an embedding, compare it with document vectors, and return documents with similar meaning.
8. **Similarity Search vs Keyword Search** — Keyword search matches words; similarity search compares vectors. Hybrid search combines both.

