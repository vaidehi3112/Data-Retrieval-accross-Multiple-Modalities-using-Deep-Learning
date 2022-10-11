# Data Retrieval across Multiple Modalities using Deep Learning


In this massive information era, where data is constantly being generated, it becomes difficult to sift through gazillion bytes of
multimedia data such as images, videos, or audio files to find the desired item. Hence it becomes crucial to establish a semantic
correlation to access multimedia data in an efficient manner. Exploring semantic relationships with images, texts, and videos has
been an active field of research for the computer vision community.

Our primary objective is to retrieve relevant images based on a text query. It has numerous applications, such as e-commerce
look-ups using user queries, audio and video look-ups. We have used an approach where natural language can be utilized for
image retrieval. State-of-the-art models have already mentioned techniques to predict entities from a set of predefined object
categories. These predefined categories limit our utility of learning directly from raw texts.

As our baseline model, we will be implementing OpenAI’s CLIP, which learns to project both the images and the text to the
same embedding space. Hence text and images can be combined and projected to the same latent space.

Our proposed model concepts in the form of encoder and decoder layout. Here a convolution neural architecture is used to
project the image features into the latent dimension , which are further provided as an input to the recurrent neural network to
generate meaningful sequence of words that describes the input image.

To fine-tune and assess our model performance, we plan to use Precision@K and Recall@K as our evaluation metric.
