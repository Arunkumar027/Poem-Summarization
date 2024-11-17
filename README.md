Poem Summarization Using T5 (Text-to-Text Transfer Transformer)
This repository implements an abstractive poem summarization system leveraging the T5 (Text-to-Text Transfer Transformer) model. It addresses the challenges of summarizing poetic texts, which often feature intricate language, abstract themes, and emotional depth. The model effectively captures the essence, sentiment, and themes of poems while maintaining coherence and relevance.

Features
Utilizes the encoder-decoder architecture of T5.
Implements advanced attention mechanisms for context and thematic integrity.
Outputs concise, human-readable poem summaries.
Employs preprocessing techniques like tokenization and punctuation removal.
Workflow
Input: Poetry dataset (e.g., Poetry Foundation) with features like title, tags, and content.
Preprocessing: Tokenization, special character removal, and sentence padding.
Encoding & Decoding: Employs the T5 architecture for text encoding and beam search-based decoding.
Output: Summarized text capturing the poem's themes and essence.
