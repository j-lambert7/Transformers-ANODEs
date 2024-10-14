# Transformer ANODEs

Project by Julien Lambert, Guillaume Février, Vivian Vanheeghe and Pierre Aguié.

In this repository, we create Augmented Neural Ordinary Differential Equation (ANODE) models for transformer architectures, and study the impact of embedding dimension augmentation on the performance of the model on Neural Language Processing tasks. Namely, we compare classic transformers, NODEs and ANODEs on text classification on the IMDb dataset.

This repository builds upon "Augmented Neural ODEs" by Dupont et al. (2019), in which the authors introduce ANODE models, and compare them to NODE models for CNN architectures on image classification tasks. This repository aims to extend their experiments to transformer architectures for text classification. The repository uses scripts from Dupont's repository, available at https://github.com/EmilienDupont/augmented-neural-odes. ODE parameters are optimised using the TorchDiffEq library (https://github.com/rtqichen/torchdiffeq).

`models.py` introduces the ODEFunc, ODEBlock and ODENet classes, used to define NODE models. The transformer NODEs and ANODEs are defined in the `ANODEsComp.ipynb` notebook.