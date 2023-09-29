# Abstractive Text Summarization with Knowledge-based Word Sense Disambiguation

This repository contains code and resources for abstractive text summarization (TS) using a novel framework that leverages knowledge-based word sense disambiguation (WSD) and semantic content generalization to enhance the performance of sequence-to-sequence (seq2seq) neural-based TS.

## Overview
This work focuses on abstractive TS of single documents and introduces a framework that unifies the characteristics of three dominant aspects of abstractive TS: structure, semantic, and neural-based approaches. The approach combines machine learning and knowledge-based techniques to achieve this integration.
## Framework Overview
The overall framework is illustrated in Figure 1. The input comprises a single-document text, along with a taxonomy of concepts T, while the output is a human-readable summary. Its main components are five, starting with WSD, whose purpose is to generalize ambiguous words. This is an important step for increasing the accuracy of content generalization that follows next and deals with OOV or rare words. Both of the aforementioned steps constitute the pre-processing phase, which is discussed in more detail in Section 4.

The generalized text is subsequently mapped to a continuous vector space, using neural language processing techniques. The said vectors are then provided to a deep seq2seq model of encoder-decoder architecture, which additionally incorporates an attention mechanism. The model, having been trained on a corpus of text-summary pairs, predicts a generalized summary for the new input it has been given. Both the vector-mapping and deep learning prediction steps are components of the machine learning phase and are further analyzed in Section 5 of the paper(project.pdf).



## Screenshots

![App Screenshot](https://github.com/priyansh4320/Abstractive-Text-Summarization-Enhancing-Sequence-to-Sequence-Models-Using-Word-Sense-Disambiguatio/blob/main/suvidha_foundation_project.png)


## Overview
This work focuses on abstractive TS of single documents and introduces a framework that unifies the characteristics of three dominant aspects of abstractive TS: structure, semantic, and neural-based approaches. The approach combines machine learning and knowledge-based techniques to achieve this integration.
## Key Contributions
Proposes a novel framework utilizing knowledge-based WSD and semantic content generalization for abstractive TS.
Combines characteristics of structure, semantic, and neural-based approaches to unify methodologies often treated separately in the literature.
Utilizes a three-step methodology: pre-processing, machine learning, and post-processing, to generate the final summary.

## Methodology
The proposed methodology comprises three main steps:

1. Pre-processing

- Utilizes knowledge-based semantic ontologies and named entity recognition (NER) to achieve text generalization.
- Extracts named entities, concepts, and senses from the original document.
2. Machine Learning Methodology

- Utilizes a seq2seq deep learning model of an attentive encoder-decoder architecture.
- Investigates five variants of the deep learning model to predict a generalized version of the summary.
3. Post-processing

- Creates the final summary using heuristic algorithms and text similarity metrics.
- Matches concepts of the generalized summary to specific ones for a cohesive output.

## Experimental Results
Extensive experiments were conducted on three widely used datasets: Gigaword, Duc 2004, and CNN/DailyMail. The results demonstrate promising outcomes, including alleviation of rare and out-of-vocabulary (OOV) words and outperforming state-of-the-art seq2seq deep learning techniques.

## Dataset Used
- Gigaword Dataset
- Duc 2004 Dataset
- CNN/DailyMail Dataset

## Reference

`
@article{Kouris, P., Alexandridis, G., & Stafylopatis, A. (2021). Abstractive text summarization: Enhancing sequence-to-sequence models using word sense disambiguation and semantic content generalization. Computational Linguistics, 47(4), 813-859.},
  title={Abstractive Text Summarization with Knowledge-based Word Sense Disambiguation},
  author={Kouris, P., Alexandridis, G., & Stafylopatis},
  year={2021},
}
`
