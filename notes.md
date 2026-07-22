Gen AI Learnings — Personal Notes
Types of AI
Non-Generative AI

AI that predicts or classifies based on existing data.

Examples:

Spam detection
Disease prediction
Credit risk prediction

Output: Label / decision.

Generative AI

AI that creates new content such as text, images, code, audio, or video.

Examples:

ChatGPT
Gemini
GitHub Copilot
Midjourney

Output: New content.

Evolution of Generative AI
1. Statistical Machine Learning

Uses structured data and human-created features to make predictions.

Example: Predicting house prices using area, bedrooms, and location.

Key idea: Humans design the features.

2. Deep Learning

Uses neural networks to automatically learn patterns from data.

Example: Detecting cats directly from images.

Key idea: The model learns features by itself.

3. Recurrent Neural Networks (RNNs)

Designed for sequential data such as text and speech.

Example: Language translation and next-word prediction.

Limitation: Struggles with long sequences.

4. Transformers

Introduced the attention mechanism, allowing the model to look at all words in a sentence at once.

Example: Modern chatbots and large language models.

Key idea: Better understanding of context and long-range relationships.

Language Models (LM)

A model that predicts the next word or token in a sequence.

Example:

Input: “I love”
Output: “Python”

Simple definition: A smart autocomplete system.

Large Language Models (LLMs)

Very large transformer-based language models trained on massive text datasets.

Examples:

GPT
Gemini
Llama
Claude

Simple definition: An LLM is a transformer trained on huge amounts of text to generate human-like responses.

Parameters

Parameters are the model’s learned weights.

They store patterns learned during training, such as relationships between words and concepts.

Simple definition: Parameters are the numbers inside a model that get updated during training and help the model make predictions.

RLHF (Reinforcement Learning with Human Feedback)

A process where humans rank model responses, and the model learns which answers are more helpful and safe.

Goal:

Better instruction following
Safer responses
More useful conversations

Simple definition: RLHF uses human feedback to make an LLM more helpful and aligned with user expectations.

Embeddings

Embeddings are numerical vector representations of text that capture semantic meaning.

Example: “car” and “automobile” will have similar embeddings.

Simple definition: An embedding converts text into a list of numbers that represents its meaning.

Vector Database

A database optimized for storing and searching embedding vectors.

Examples:

Pinecone
Qdrant
Chroma
pgvector

Simple definition: A vector database stores embeddings and quickly finds the most similar ones.

Similarity Search

The process of finding vectors that are closest in meaning to a query vector.

Common metric: Cosine similarity.

Example: A query about “learning Python” retrieves documents about Python tutorials even if the exact words are different.

Simple definition: Similarity search finds content with similar meaning, not just matching keywords.

LangChain Learnings
What is LangChain?

LangChain is a framework for building applications using Large Language Models (LLMs).

It acts as a bridge between the LLM and external data/tools such as PDFs, databases, APIs, and memory.

Why LangChain?

An LLM alone can generate text, but real AI applications also need to:

Read documents
Search a vector database
Remember conversations
Call APIs/tools
Perform multi-step workflows

LangChain helps orchestrate all these components.

Core Components
LLM / Chat Model

The AI model that generates responses (GPT, Gemini, Claude, Llama).

Prompt Template

Reusable prompts with placeholders.

Chain

Connects multiple steps into a workflow.

Example: Question → Retriever → LLM → Answer

Retriever

Fetches the most relevant document chunks from a vector database.

Memory

Stores conversation history.

Agent

Allows the LLM to choose and use external tools dynamically.