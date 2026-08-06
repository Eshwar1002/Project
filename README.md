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


 Fine-Tune an LLM for Sanskrit–English
Instruction Following
Problem Statement
Fine-tune a small open-source multilingual language model to better answer Sanskrit-related
questions, translations, or explanations.
The goal is to test:
● Instruction tuning
● Multilingual tokenization handling
● Dataset preparation
● Efficient fine-tuning techniques
● Evaluation methodology
Example Tasks
Your model should improve on tasks such as:
● Sanskrit → English translation
● English → Sanskrit translation
● Explaining Sanskrit verses
● Answering questions about Sanskrit text
● Simple grammar/morphology reasoning
● Summarization of Sanskrit passages
Suggested Base Models
You are expected to choose and justify your model.
Possible starting points:
● Hugging Face models such as:
○ Llama-3.2-1B
○ Gemma-2B
○ IndicTrans2
○ Sarvam
○ multilingual T5 variants
You may use LoRA/QLoRA or full fine-tuning depending on feasibility.
Suggested Datasets
You may combine or curate datasets from sources such as:
Sanskrit Resources
● Sanskrit Documents
● AI4Bharat IndicCorp
● Hugging Face Sanskrit Datasets
● OPUS Parallel Corpora
● Wikipedia Sanskrit Dumps
Possible Data Construction
You may:
● Create instruction-response pairs
● Generate synthetic instructions
● Build QA pairs
● Build translation datasets
● Build summarization datasets
Interesting Challenges We Expect You to Think About
[Optional to Implement]
Tokenization / Vocabulary
Sanskrit has:
● compound words
● transliteration variations
● Devanagari + Roman scripts
● rare tokens
We are interested in:
● whether you inspect tokenizer behavior
● how OOV/subword fragmentation affects training
● whether you attempt tokenizer adaptation or explain why not
Expected Deliverables
Code
● Colab notebook or repo
● Training scripts
● Inference scripts
Documentation
A short report covering:
1. Problem understanding
2. Dataset preparation
3. Why you selected the base model
4. Fine-tuning approach
5. Hardware constraints and optimizations
6. Evaluation methodology
7. Failure cases
8. Challenges encountered
9. What you would improve with more time
Evaluation
Include:
● qualitative outputs
● before vs after comparison
● any metrics used
● hallucination/error analysis
