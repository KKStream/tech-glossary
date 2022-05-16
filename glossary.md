# Glossary of Technical Terms and Assets

* Version: v0.1
* License: MIT

## Overview

The glossary of technical terms is a freely-licensed, open source lexicon of terms related to streaming technologies and streaming industry.
It has been built using a collaborative process and is designed for easy adoption by the entire edge computing ecosystem,
including by open source projects, vendors, standards groups, analysts, journalists, and practitioners.

## Glossary

### Attention mechanism

- was introduced to improve the performance of the encoder-decoder model for machine translation. The idea behind the attention mechanism was to permit the decoder to utilize the most relevant parts of the input sequence in a flexible manner, by a weighted combination of all of the encoded input vectors, with the most relevant vectors being attributed the highest weights.
- A self-attention means the contextual information, i.e. the weight to the input, comes from the input itself.
- SeeAlso:: https://machinelearningmastery.com/the-attention-mechanism-from-scratch/
- Tags:: deep learning

### Autoencoder

- An autoencoder is a neural network consist of an encoder network and a decoder network.
- The encoder compresses the input to latent embeddings.
- The decoder decompresses the latent embeddings and reconstructs the input.

### Bag-of-words

- is a simplifying representation used in natural language processing and information retrieval. In this model, a text (such as a sentence or a document) is represented as the bag (multiset) of its words, disregarding grammar and even word order but keeping multiplicity.
- SeeAlso:: https://www.wikiwand.com/en/Bag-of-words_model
- Tags:: NLP

### Charbonnier loss

- A loss function to approximate the L1 loss, i.e. absolute value function, while being differentiable at 0.
- Usually being applied in image-to-image comparison tasks, e.g. super-resolution.
- Tags:: loss function

### Convolutional neural network (CNN)

- A foundamental deep learning model to simulate how human perceive things in terms of their closeness, usually space or time.
- It is widely used, but not limited to, in computer vision because visual patterns are usually formed by their surrounding information.
- Tags:: CV, deep learning

### Data augmentation

- This term generally refers to a set of data preprocessing methods to increase the diversity of input data for training a noise-tolerant model and to avoid overfitting.
- For example, in computer vision, an input image may be transformed by random rotation, random cropping, brightness adjustment, or other transformations and their combinations.

### Diffusion model

- A diffusion model is a [generative](#generative-model). It assumes true data samples can be converted to pure noises, and learns how to "denoise" pure noises into true data samples.

### Discriminitive model

- A model that aims to learn how to discriminate, or differentiate, from the given information. Most of the traditional machine learning models are discriminitive. For example, a classifier discriminates two samples by their labels, a regressor finds the differences to the predicted value, and a cluster gathers similar information while distances from the other clusters.
- Contrast to [generative model](#generative-model)

### Dropout

- Dropout is a layer used in deep neural network to avoid overfitting by randomly masking (dropping) the output of a neuron in each iteration.
- In forward propagation, the outputs of masked neurons are 0, so they does not contribute to the next layer.
- In backward propagation, the gradients of masked neurons are also 0, so they does not get updated.
- Tags:: deep learning, regularization

### Generative advisarial network (GAN)
- GAN is an architecture of deep neural networks which consist of a generator (i.e. a [generative](#generative-model) network) and a discriminator (i.e. a [discriminitive](#discriminitive-model) network).
- The generator produces fake samples from a sampled distribution (e.g. Gaussian noise) which should be as close as true samples.
- The discriminator learns how to differentiate fake samples from true samples.

### Generative model

- The goal of a generative model is to learn how to produce new data from given data samples.
- It is widely used in video/image/speech synthesis and simulation.
- Contrast to [discriminitive model](#discriminitive-model)

### Knowledge Graph (KG)

- A graph structure used to represent the entities (nodes) and their relations (edges) of real-world knowledges.
- Entities are usually nouns or adjectives, representing a real object, a virtual concept, or an attribute.
- Relations are usually verbs, representing how two entities interact with each other, e.g. has, involves in, consists of, etc.
- A knowledge graph is an implementation of [Ontology](#ontology).
- Tags:: data model

### Language model

- A language model defines how words in natural languages related to each other.
- [Bag-of-words](#bag-of-words) is a language model without sequential information.
- Tags:: NLP

### Long short-term memory (LSTM)

- A LSTM is an improved [RNN](#recurrent-neural-network-rnn) simulating how human memorizes and forgets things. It learns a gating mechanism to filter the informative data for the task.
- Tags:: deep learning

### Multi-model database

- is a database that can store, index and query data in more than one model. For some time, databases have primarily supported only one model, such as: relational database, document-oriented database, graph database or triplestore. A database that combines many of these is multi-model.
- SeeAlso:: https://www.wikiwand.com/en/Multi-model_database

### Ontology

- is a semantic data model that define the types of things that exist in our domain and the properties that can be used to describe them.
- Ontologies are generalized data models, meaning that they only model general types of things that share certain properties, but don’t include information about specific individuals in our domain. For example, instead of describing your dog, Spot, and all of his individual characteristics, an ontology should focus on the general concept of dogs, trying to capture characteristics that most/many dogs might have.
- Three main components:
  - Classes: the distinct types of things that exist in our data.
  - Relationships: properties that connect two classes.
  - Attributes: properties that describe an individual class.
- SeeAlso:: https://enterprise-knowledge.com/whats-the-difference-between-an-ontology-and-a-knowledge-graph/
- Tags:: data model

### Recurrent neural network (RNN)

- A RNN is a foundamental deep learning model to simulate how human perceive things in sequential order.
- It is widely used in natural language tasks and time-series analysis.
- Tags:: deep learning, NLP

### Relational Dataset Repository (RDR)

- having famous public dataset but in easier form as database (MariaDB).
- MoveLens on RDR: https://relational.fit.cvut.cz/dataset/MovieLens
- IMDb on RDR: https://relational.fit.cvut.cz/dataset/IMDb
- SeeAlso:: https://relational.fit.cvut.cz/
- Tags:: dataset, metadata

### Residual neural network

- A deep learning model with several skipped connections by adding the input and output of a block. This makes the residual, i.e. differences between input and output, learnable.
- A residual neural network also solves the gradient vanishing problem in a very deep neural network, as some gradients are back-propagated via the skip connections.
- Tags:: deep learning

### Transformer

- A deep encoder-decoder model that is built upon the [self-attention mechanism](#attention-mechanism). The encoder encodes the input sequence (e.g. how are you &lt;EOS&gt;) by multi-head self-attention layers, while the decoder decodes the target sequence of previous tokens (shifted right by 1, e.g. &lt;BOS&gt; fine thank you) by masked multi-head self-attention laters. The goal is to predict the taget sequence (e.g. fine thank you &lt;EOS&gt;).
- Tags:: deep learning

### Variational autoencoder (VAE)

- A VAE follows a classical [autoencoder](#autoencoder) architecture, only that the latent embeddings are parameters of a distribution (usually Gaussian). Therefore, the decoder randomly samples from the distribution and reconstructs the input.
- A VAE provides highly continuous and robust embeddings compared to AEs.

### Venn diagram

- A Venn diagram is a widely used diagram style that shows the logical relation between sets, popularized by John Venn in the 1880s. The diagrams are used to teach elementary set theory, and to illustrate simple set relationships in probability, logic, statistics, linguistics and computer science.
- A Venn diagram uses overlapping circles or other shapes to illustrate the logical relationships between two or more sets of items. Often, they serve to graphically organize things, highlighting how the items are similar and different.
- purpose and benefits:
  - To visually organize information
  - To compare two or more choices
  - To solve complex mathematical problems
  - To compare data sets
  - To reason through the logic
- SeeAlso::
  - https://www.wikiwand.com/en/Venn_diagram
  - https://www.lucidchart.com/pages/tutorial/venn-diagram/
- Tags:: diagram, visualization
