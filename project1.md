AI/ML Model Training - Take Home Assignment
Objective
This assignment is designed to evaluate your ability to:
● Quickly learn and implement model fine-tuning/training workflows
● Work beyond hosted APIs and interact directly with open-source models
● Handle multilingual NLP problems (especially Sanskrit + English)
● Make practical engineering decisions under limited compute constraints
● Evaluate models rigorously and communicate tradeoffs clearly
● Debug and iterate independently
The assignment is intentionally open-ended. We are less interested in achieving
state-of-the-art metrics and more interested in:
● Your approach
● How quickly you learn unfamiliar tooling
● Your reasoning and experimentation process
● Your ability to make practical engineering tradeoffs
● Your understanding of evaluation and failure analysis
Environment Constraints
● Target environment: Google Colab (You may use other GPU environments if you
have access to them)
● GPU target: T4 / L4
● Expected completion time: 1–2 days
● You may use:
○ Hugging Face
○ PyTorch
○ PEFT / LoRA / QLoRA
○ SentenceTransformers
○ Transformers
○ TRL
○ BitsAndBytes
○ OCR tools if applicable



Option 2 - Train/Fine-Tune a Multilingual Embedding Model
for Sanskrit + English Retrieval
Problem Statement
Build a multilingual retrieval system by fine-tuning an embedding model for Sanskrit-English
semantic search.
The goal is to evaluate:
● understanding of embedding models
● contrastive learning/triplet training
● retrieval evaluation
● RAG-oriented thinking
Example Use Case
Given a Sanskrit verse or English query:
“What does this verse say about karma?”
The system should retrieve relevant Sanskrit passages and/or English explanations.
Suggested Base Models
Possible candidates:
● bge-small-en-v1.5
● multilingual-e5-small
● gte-multilingual
● Indic embedding models
● SentenceTransformers-compatible models
Suggested Datasets
Parallel / Aligned Text Sources
● Bhagavad Gita Sanskrit + English translations
● Upanishads
● Sanskrit-English aligned corpora
● AI4Bharat datasets
● OPUS multilingual corpora
Suggested Data Format
You may create:
● query-document pairs
● positive/negative triplets
● hard negatives
● synthetic retrieval queries
Suggested Tasks
● Fine-tune embeddings using contrastive learning
● Build a mini RAG/retrieval demo
● Evaluate top-k retrieval quality
Expected Evaluation
We care about:
● retrieval quality
● embedding space reasoning
● negative sampling strategy
● evaluation rigor
Possible metrics:
● Recall@K
● MRR
● nDCG
