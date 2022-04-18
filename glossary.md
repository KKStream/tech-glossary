# Glossary of Technical Terms and Assets

* Version: v0.1
* License: MIT

## Overview

The glossary of technical terms is a freely-licensed, open source lexicon of terms related to streaming technologies and streaming industry.
It has been built using a collaborative process and is designed for easy adoption by the entire edge computing ecosystem,
including by open source projects, vendors, standards groups, analysts, journalists, and practitioners.

## Glossary

### Bag-of-words

- is a simplifying representation used in natural language processing and information retrieval. In this model, a text (such as a sentence or a document) is represented as the bag (multiset) of its words, disregarding grammar and even word order but keeping multiplicity.
- SeeAlso:: https://www.wikiwand.com/en/Bag-of-words_model
- Tags:: NLP

### Charbonnier loss

- is a loss function to approximate the L1 loss, i.e. absolute value function, while being differentiable at 0.
- Usually being applied in image-to-image comparison tasks, e.g. super-resolution.
- Tags:: loss function

### Convolutional neural network (CNN)

- A CNN is a foundamental deep learning model to simulate how human perceive things in terms of their closeness, either space or time.
- It is widely used, but not limited to, in computer vision because visual patterns are usually formed by their surrounding visual information.
- Tags:: CV, deep learning

### Language model

- A language model defines how words in natural languages related to each other.
- A [bag-of-words](#bag-of-words) model is a language model without sequential information.

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
- Tags:: data_model

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
