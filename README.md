# Transforming Drug Development: Exploring the Power of Graph Representations in Predicting Cardiotoxicity

This project delves into the realm of graph representation learning to predict the cardiotoxicity of molecules. It investigates the efficacy of Graph Neural Networks (GNNs) against traditional non-graph Neural Networks (NNs) using the Tox21 toxicity dataset.

## Abstract

    Cardiotoxicity is a major barrier in drug development, often leading to the discontinuation of new drugs and thus decelerating the drug development process. Addressing this challenge through computational prediction could significantly improve the efficiency of drug discovery. This study explores the potential of graph representation learning, a method apt for modeling molecular structures, to predict the cardiotoxicity of molecules. 

    To investigate whether graph-based approaches provide benefits in cardiotoxicity prediction, I carried out experiments using a graph neural network as well as a conventional non-graph neural network. Both models were trained on the same dataset, albeit utilizing distinct representations: graph structures for the former and fixed-sized embeddings for the latter. Due to the lack of cardiotoxicity datasets amendable to both representations, I utilized the more general toxicity dataset Tox21, where I identified four classes indicative of cardiotoxicity. The graph representation model outperformed the non-graph baseline, with AUROC scores of 80\% and 75\%, respectively.
    
    This research explores the efficacy of leveraging molecular structure modeling through graph representation, offering a promising method to reduce cardiotoxicity risks and enhance drug discovery efficiency.
    
## Getting Started

To begin, clone the repository:

```
git clone https://github.com/anonymousoxford2024/Computational-Medicine-Exam.git
```

Or via SSH:

```
git clone git@github.com:anonymousoxford2024/Computational-Medicine-Exam.git
```

Next, create a virtual environment using Python version 3.9.6.

Install the required dependencies:

```
pip install -r requirements.txt
```

With the setup complete, you can proceed to either retrain or evaluate the models.

## Reproducing Results

To perform evaluation:

```
python src/evaluation/run_evaluation.py
```

To retrain the models:

```
python src/train_baseline.py
```

```
python src/train_gnn.py
``` 

This ensures you can replicate the results effectively.
