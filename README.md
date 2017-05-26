MDNNMD
===============================
An implementation of multimodal deep neural network, a new model for human breast cancer prognosis prediction.

Requirements
========================
    python 2.7
    TensorFilow 1.0
    scikit-learn 0.18
    cuda 8.0
Usage
========================
python MDNNMD.py


Parameters of MDNNMD
=====================
The Parameters of MDNNMD are in our configuration file `configuration.txt`. The descriptions of these parameters of MDNNMD are provided below:

    =================================================================================================
    | PARAMETER NAME       | DESCRIPTION                                                            |
    =================================================================================================
    |       α,β,γ          |α,β,γ are three damping factors used to balance the contribution for    |
    |                      |each DNN model. Here the sum of three damping factors should be equal 1.|
    -------------------------------------------------------------------------------------------------
    |         K            |the number of fold with cross validation experiment or an index file.   |
    -------------------------------------------------------------------------------------------------    
    |         D1           |the data file of gene expression profile                                |
    -------------------------------------------------------------------------------------------------
    |         D2           |the data file of copy number alteration profile.                        |
    -------------------------------------------------------------------------------------------------
    |         D3           |the data file of clinical information                                   |
    -------------------------------------------------------------------------------------------------
    |         M            |mini-batch size.                                                        |
    -------------------------------------------------------------------------------------------------
    |         bne          |batch normalization epsilon.                                            |
    -------------------------------------------------------------------------------------------------
    
Output variables of MDNNMD
=====================
The descriptions of output variables of MDNNMD are provided below:

    ====================================================================================================================
    | VARIABLE NAME         |                                   DESCRIPTION                                            |
    ====================================================================================================================
    | Prediction_score.txt  |The final prediction score of all samples with 10 fold cross validation experiment.       |
    |                       |The output of the MDNNMD with a softmax function.                                         |
    --------------------------------------------------------------------------------------------------------------------
    | Prediction_labels.txt |The prediction labels represent long-term patients with 0 and short-term patients with 1. |
    --------------------------------------------------------------------------------------------------------------------    

Contact
=====================
Author: Dongdong Sun @HILAB  
Maintainer: Dongdong Sun  
Mail: sddchina@mail.ustc.edu.cn
Date: 2017-5-30  
Health Informatics Lab, School of Information Science and Technology, University of Science and Technology of China

