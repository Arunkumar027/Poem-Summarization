# Leveraging Encoder-Decoder Architecture for Effective Poem Summarisation

## Overview
This project explores the use of an encoder-decoder architecture to perform effective poem summarisation. Poetic language, known for its intricate structure, metaphors, and creative expressions, poses unique challenges for conventional summarisation techniques. This research addresses these challenges by utilizing advanced deep learning methods tailored to the nuances of poetic content.

## Objective
The goal of this project is to design and implement a system capable of producing concise and meaningful summaries of poems while preserving their core themes and emotional tone. The model leverages a sequence-to-sequence (Seq2Seq) framework with an encoder-decoder architecture to understand and generate coherent summaries of poetic texts.

## Key Contributions
- *Customised Seq2Seq Model*: Utilizes an encoder to understand complex poetic structures and a decoder to generate summaries that are both fluent and contextually accurate.
- *Attention Mechanism*: Integrates an attention layer to ensure the model effectively focuses on significant parts of the input sequence during summarisation.
- *Pre-trained Embeddings*: Employs pre-trained word embeddings to enrich the model's understanding of nuanced language and literary devices present in poems.
- *Training Strategy*: Includes a fine-tuning process with a curated dataset of poems and their respective human-written summaries to achieve robust performance.

## Architecture
- *Encoder*: Processes the input poem, encodes its structure, and captures contextual dependencies using recurrent layers (LSTM/GRU) or a transformer-based approach.
- *Attention Layer*: Enhances the model’s ability to selectively focus on important words or phrases within the poem, allowing for better content comprehension.
- *Decoder*: Generates the summary by decoding the contextual representation learned by the encoder into a cohesive and meaningful output.

## Dataset
- The project utilizes a custom dataset consisting of various poems alongside human-written summaries. This dataset was preprocessed to maintain the quality of language, structure, and semantics necessary for effective training.

## Implementation
1. *Preprocessing*: Text cleaning, tokenization, and padding to handle varying poem lengths.
2. *Model Training*:
   - The model is trained using a combination of teacher forcing and cross-entropy loss.
   - Validation steps include ROUGE and BLEU scores to measure summarisation quality.
3. *Fine-Tuning*: A pre-trained language model (e.g., BERT, GPT) can be fine-tuned within the encoder-decoder framework to enhance the model's capacity for understanding nuanced language.

## Evaluation
The model's performance is evaluated through automated metrics such as BLEU, ROUGE, and human assessment to ensure the summaries are faithful to the original text's content and style.

## Results
Initial experiments demonstrated that incorporating attention mechanisms and pre-trained embeddings significantly improved the summarisation quality, preserving both the thematic elements and the emotional essence of the original poems.

## Future Work
- *Expansion of the Dataset*: Collecting a more extensive set of poems across different styles and eras to improve model generalizability.
- *Incorporating Multimodal Inputs*: Exploring the use of visual and auditory features from spoken-word poetry for more comprehensive summarisation.
- *Model Optimization*: Enhancing performance with transformer-based models such as BART or T5.

## How to Use
- Clone this repository and set up the environment using requirements.txt.
- Train the model using the provided scripts or download the pre-trained weights.
- Test the summarisation using custom inputs through the command line or provided API interface.

## License
This project is open-source and distributed under the MIT License. Please refer to the [LICENSE](LICENSE) file for more details.

## Acknowledgements
- Inspired by existing research on neural summarisation and the complexities of natural language processing for creative content.
- Special thanks to the NLP and poetry communities for their resources and inspiration.

Feel free to modify or contribute to the project to extend its capabilities for better handling of complex poetic texts.
