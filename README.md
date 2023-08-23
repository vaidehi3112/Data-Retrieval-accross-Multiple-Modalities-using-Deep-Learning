# Data Retrieval across Multiple Modalities using Deep Learning

**Authors:** Vaidehi Pareshkumar Parikh, Shaival Sujalkumar Shah, Nidutt Nilay Bhuptani  
**GitHub Repository:** [Data Retrieval across Multiple Modalities using Deep Learning](https://github.com/vaidehi3112/Data-Retrieval-across-Multiple-Modalities-using-Deep-Learning)

## Summary

Multi-modal processing has been an active area of work in the last decade. The primary objective is to retrieve relevant images based on a text query. This project focuses on utilizing natural language for image retrieval. The baseline model is OpenAI’s CLIP, which projects both images and text to the same embedding space. The proposed model uses an encoder-decoder layout, with a convolutional neural architecture projecting image features into a latent dimension. These are then input to a recurrent neural network to generate a meaningful sequence of words describing the input image.

## Dataset

The project uses the Flickr30K dataset, consisting of 31,784 images, each with 5 captions, totaling about 150K captions. The dataset is split into 28K images for training, 1.5K for validation, and 1.5K for testing.

## Evaluation Metrics

- **BLEU Score:** Used for caption generation evaluation.
- **Precision@K and Recall@K:** Used for image retrieval evaluation.

## Proposed Models

1. **CLIP (Contrastive Language–Image Pre-training):** Developed by OpenAI, CLIP can understand images paired with natural language. It is trained on a variety of internet text–image pairs and can be applied to a wide range of visual tasks without task-specific training.
2. **Image Captioning (without Attention) + Text Embedding:** This model uses an encoder-decoder architecture, incorporating a vision model in the encoder and a text model in the decoder. The generated caption is then encoded using HuggingFace's BERT weights.
3. **Show Attend and Tell (with Attention):** This model adds an attention mechanism, allowing for salient features of an image to be highlighted. It uses an LSTM network to generate captions based on a context vector, previous hidden state, and previously generated words.

## Project Workflow

![Project Workflow](https://showme.redstarplugin.com/d/d:eSsIe10f)

[View the flowchart in a new tab](https://showme.redstarplugin.com/d/d:eSsIe10f)

