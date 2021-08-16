# DeepPurpose : a deep learning library for drug-target interaction prediction

## Abstract

## 1. Introduction

## 2. DeepPurpose Library

### 2.1 Module for encoding proteins and compounds
  - DeepPurpose takes the compound's SMILES string and protein amino acid sequence pair as input.
  - They are fed into molecular encoders which specifies a deep transformation function that maps compoundsand 

### 2.2 Module for DTI prediction
  - DeepPurpose feeds the learned protein and compound embeddings into an MLP decoder to generate predictions.
  - 
### 2.3 Modules for other downstream prediction tasks
  - 1.
  - 2. DeepPurpose supports user-friendly programming frameworks for other modeling tasks, including drug and protein property prediction, drug-drug intereaction prediction and protein-protein interaction prediction
  - 3. DeepPurpose provides an interface to many types of data, including public large binding affinity dataset, bioassay data and a drug repurposing library.
### 2.4 Programming framework and implementation details
  - The functionality of DeepPurpose is modularized into six key steps where a single line of code can invoke each step
    + (i) Load the dataset from a local file or load a DeepPurpose benchmark dataset
    + (ii) Specify the names of compound and protein encoders.
    + (iii) Split the dataset into training, validation and testing sets using data_process function, which implements a variety of data-split strategies.
    + (iv) Create a configuration file and specify model parameters. If needed, DeepPurpose can automatically search for optimal values of hyper-parameters.
    + (v) Initialze a model using the configuration file. Alternatively, the user can load a pre-trained model or a previously saved model.
    + (vi) Fianlly, train the model using train function and monitor the progress of training and performance metrics.
    + [https://github.com/kexinhuang12345/DeepPurpose.

## 3. Using DeepPurpose for DTI prediction
  - KronRLS : a popular DTI method
  - GraphDTA
  - DeepDTA

## 4. DeepPurpose with interactive web interface
  - DeepPurpose also provides utility functions to load a pre-trained model and make predictions for a new drug and target inputs.
  - This web interface takes the SMILES and amino acid sequence as the input and return prediction scores with elss than 1-second latency.
