# Microsoft-Research-Sentence-Completion-Challenge
Collection of methods for approaching the MSR-SCC. LSA, n-gram, and neural network implementations.

This challenge consists of 1040 sentences. In each sentence a word has been removed and in it's place are 4 alternative incorrect options (selection was based on various criteria but they all have similar occurence statistics) and the 1 true option (the original word). The goal is to predict as many valid sentences as possible and so present a system that performs well in modelling semantic meaning in text. 

The dataset was built from Project Gutenberg data, with seed sentences being selected from Sir Arthur Conan-Doyle's "Sherlock Holmes" novels. The imposter words were suggested by way of a language model trained on over 500 19th centurary novels. This language model computed alternative words for a given low frequency word in a sentence, from which human judges selected the most appropriate 4 imposter words. The criteria which candidate words were assessed by as well as more information regarding the challenge can be found in the [original publication](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/MSR_SCCD.pdf).


This repository contains a collection of methods for this sentence completion task:
* **N-gram Language Models**
* **Latent Semantic Analysis**
* **Neural Networks**
