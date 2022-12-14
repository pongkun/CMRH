## Countering Modal Redundancy and Heterogeneity: A Self-Correcting Multimodal Fusion

This is the PyTorch implementation of ICDM2022 paper 'Countering Modal Redundancy and Heterogeneity: A Self-Correcting Multimodal Fusion'. The full version will be updated soon.

We propose a unified multimodal fusion strategy to counter modal redundancy and heterogeneity. For heterogeneity, we design a groundbreaking UFIM approach, which can effectively extract and transfer inter-modal fine-grained correlations among features with its inbuilt orthogonal attention and interactive feedback, achieving unified modal interactions. For redundancy, we utilize a novel SCTM to obtain the one-to-many modal correlation information to alleviate two kinds of redundancies in different ways.

<img width="800" src="redundancy.png" alt="redundancy" />

### Usage

#### Environment

    GPU: NVIDIA Tesla V100
    CentOS Linux release 7.7.1908
    CUDA 9.2
    python 3.7
    torch 1.6.0
    torchvision 0.7.0
    cupy 6.0.0
    scipy 1.5.2
    pillow 6.0.0
    numpy 1.17.4
    
#### Dataset

[NTU RGB+D](http://rose1.ntu.edu.sg/datasets/actionrecognition.asp) dataset.

#### Training and Evaluation

    python main_CMRH.py --datadir dataset_path --checkpointdir checkpoint_path --train --ske_cp skecp_path --rgb_cp rgbcp_path
    
    python main_CMRH.py --datadir dataset_path --checkpointdir checkpoint_path --test_cp testcp_path --no_bad_skel

### Acknowledgements

This code is based on MFAS and MMTM.
