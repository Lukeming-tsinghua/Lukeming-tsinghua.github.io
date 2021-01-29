---
title: Paper Review
date: 2021-01-29 12:02:40
tags: NLP
description: This is a content for paper reviewed
---

# Relation Extraction

1 Label-Free Distant Supervision for Relation Extraction via Knowledge Graph Embedding (EMNLP2018)

https://www.aclweb.org/anthology/D18-1248.pdf

2 NERO: A Neural Rule Grounding Framework for Label-Efficient Relation Extraction (WWW2020)

https://arxiv.org/pdf/1909.02177.pdf

<!-- more -->

3 Matching the Blanks: Distributional Similarity for Relation Learning(ACL2019)

https://arxiv.org/pdf/1906.03158.pdf

4 A Frustratingly Easy Approach for Joint Entity and Relation Extraction

https://arxiv.org/pdf/2010.12812.pdf

5 Relation Extraction Using Supervision from Topic Knowledge of Relation Labels(IJCAI2019)

https://www.ijcai.org/Proceedings/2019/0698.pdf

6 Cross Relation Cross Bag attention for distantly supervision(AAAI19)

https://www.aaai.org/ojs/index.php/AAAI/article/download/3813/3691

7 Relation Extraction with Multi-instance Multi-label Convolutional Neural Networks (COLING 2016)

https://www.aclweb.org/anthology/C16-1139.pdf

8 Looking Beyond Label Noise: Shifted Label Distribution Matters in Distantly Supervised Relation Extraction

https://arxiv.org/pdf/1904.09331.pdf

This work focuses on study what limits the performance of DS-trained neural models. After conducting analyses, the authors believe a significant factor - shifted label distribution is overlooked before. The difference between DS training dataset and correspondding human-annotated dataset comes from the miss-labeling of distant supervision, since distant supervision may bring false negative and false positive samples into training dataset and results in a different label distribution. Then, authors introduce two threshold-based methods - max threshold and entrophy threshold and demontrate a good F1 improvements when adopting these methods to both DS dataset KBP, NYT and annotated dataset TACRED. Besides, inspiring by domain adaption, authors also propose another theoretically-sound adaptation method - bias adjustment to enhance model performance under label distribution shift. With two bias adjustment strategies BA-Set and BA-Fix, impressed gains of F1 score are witnessed on DS dataset.
 
9 Learning Dual Retrieval Module for Semi-supervised Relation Extraction (WWW19)

https://arxiv.org/pdf/1902.07814.pdf
 
 
# Interpretation

1 Towards Hierarchical Importance Attribution: Explaining Compositional Semantics for Neural Sequence Models(ICLR2020)

https://openreview.net/pdf?id=BkxRRkSKwr

2 Visualizing and Understanding Neural Models in NLP

https://arxiv.org/pdf/1506.01066.pdf

3 Axiomatic Attribution for Deep Networks

https://arxiv.org/pdf/1703.01365.pdf

4 Generating Hierarchical Explanations on Text Classification via Feature Interaction Detection

https://arxiv.org/pdf/2004.02015.pdf

5 Hierarchical Interpretations For Neural Network Predictions

https://arxiv.org/pdf/1806.05337.pdf

6 Incorporating Priors with Feature Attribution on Text Classification

https://arxiv.org/pdf/1906.08286.pdf

7 Did the Model Understand the Question?

https://www.aclweb.org/anthology/P18-1176.pdf

# NER

1 TriggerNER: Learning with Entity Triggers as Explanations for Named Entity Recognition(ACL2020)

https://arxiv.org/pdf/2004.07493.pdf

2 A Rigorous Study on Named Entity Recognition: Can Fine-tuning Pretrained Model Lead to the Promised Land?

https://arxiv.org/pdf/2004.12126.pdf

3 Interpretable Multi-dataset Evaluation for Named Entity Recognition

https://arxiv.org/pdf/2011.06854.pdf

4 Event Extraction by Answering (Almost) Natural Questions

https://arxiv.org/pdf/2004.13625.pdf

# Few-shot/Zero-shot RE

1 Zero-shot Learning by Generating Task-specific Adapters

https://arxiv.org/pdf/2101.00420.pdf

2 Hybrid Attention-Based Prototypical Networks for Noisy Few-Shot Relation Classification (AAAI2019)

https://gaotianyu1350.github.io/assets/aaai2019_hatt_paper.pdf

3 Prototypical Networks for Few-shot Learning

https://arxiv.org/pdf/1703.05175.pdf

# Integrate PLMs with KG

## Entity-aware language models

1 ERNIE: Enhanced Representation through Knowledge Integration

https://arxiv.org/pdf/1904.09223.pdf

ERNIE from Baidu proposes the knowledge masking strategy for masked language model to enhance language representation by knowledge.
 
2 Knowledge Enhanced Contextual Word Representations

https://arxiv.org/pdf/1909.04164.pdf

This model incorporates WordNet knowledge bases into BERT using Knowledge attention and recontextualization, and entity linking information in Wikipedia. If entity linking supervision is available, the model is learned with an additional knowledge-aware log-likelihood or max-margin objective.
 
3 Entities as Experts: Sparse Memory Access with Entity Supervision

https://arxiv.org/pdf/2004.07202.pdf

This work focuses on the problem of capturing declarative knowledge about entities in the learned parameters of a language model. The proposed model Entities as Experts (EAE) can access distinct memories of the entities mentioned in a piece of text. It's entity representations are learned directly from text instead of integrate entity knowledge into sequence models.
 

## Integrate PLMs with KGE & Transformer structure

1 ERNIE-THU

https://www.aclweb.org/anthology/P19-1139.pdf

This work injects a knowledge graph into BERT. They align entities from Wikipedia sentences to fact triples in WikiData. In the training process, the input includes sentences and linked facts, and the knowledge-aware learning objective is to predict the correct token-entity alignment. Entity embeddings are trained on fact triples from WikiData via TransE
 
2 K-BERT: Enabling Language Representation with Knowledge Graph

https://arxiv.org/pdf/1909.07606.pdf

3 Integrating Graph Contextualized Knowledge into Pre-trained Language Models

https://arxiv.org/pdf/1912.00147.pdf

This work integrates fact triples from knowledge graph. For each entity, it sample incoming and outcoming instances from the neighbors on the knowledge graph, and replaces head or tail entity to cre- ate negative instances. The model is learned to discriminate between real and fake facts.
 
4 CoLAKE: Contextualized Language and Knowledge Embedding

https://arxiv.org/pdf/2010.00309.pdf

This work proposes CoLAKE which jointly learns contextualized representation for both language and knowledge with the extended MLM objective. Instead of injecting only entity embeddings, CoLAKE extracts the knowledge context of an entity from large-scale knowledge bases. To handle the heterogeneity of knowledge context and language context, knowledge graph and text are integrated in a unified data structure, word-knowledge graph (WK graph).
 
5 K-ADAPTER: Infusing Knowledge into Pre-Trained Models with Adapters

https://arxiv.org/pdf/2002.01808v3.pdf

6 KEPLER: A Unified Model for Knowledge Embedding and Pre-trained Language Representation

https://arxiv.org/pdf/1911.06136.pdf

7 JAKET: JOINT PRE-TRAINING OF KNOWLEDGE GRAPH AND LANGUAGE UNDERSTANDING

https://arxiv.org/pdf/2010.00796.pdf

# Knowledge Graph Embedding

## Text-enhanced KGE

1 Joint Representation Learning of Text and Knowledge for Knowledge Graph Completion

https://arxiv.org/pdf/1611.04125.pdf

2 Accurate Text-Enhanced Knowledge Graph Representation Learning (NAACL2018)

https://www.aclweb.org/anthology/N18-1068.pdf

3 A Model of Text-enhanced Knowledge Graph Representation Learning with Mutual Attention (IEEE Access)

https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9037292

## Calibration

1 Evaluating the Calibration of Knowledge Graph Embeddings for Trustworthy Link Prediction(2020EMNLP)

https://www.aclweb.org/anthology/2020.emnlp-main.667.pdf

2 Probability Calibration For Knowledge Graph Embedding Models(ICLR2020)

https://arxiv.org/pdf/1912.10000.pdf
