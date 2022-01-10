[English](#Requirement)
[中文](#运行环境)

# FlatTN
This repository contains code accompanying the paper "AN END-TO-END CHINESE TEXT NORMALIZATION MODEL BASED ON RULE-GUIDED FLAT-LATTICE TRANSFORMER" which is submitted to ICASSP 2022.
# Requirement

```
Python: 3.7.3
PyTorch: 1.2.0
FastNLP: 0.5.0
Numpy: 1.16.4
```
you can go [here](https://fastnlp.readthedocs.io/zh/latest/) to know more about FastNLP.

# Dataset download
Chinese Text Normalization Dataset can be available at https://www.data-baker.com/en/#/data/index/TNtts.

To browse the Chinese version of the download page, please click https://www.data-baker.com/data/index/TNtts.

#Data preprocessing

The raw dataset in jsonl format are saved at : 
```
dataset/cleaned_dataset_by_myself/CN_TN_epoch-01-28645_2.jsonl
```

Preprocessed data are saved at : 
`dataset/cleaned_dataset_by_myself/shuffled_BMES`

We divided data into `train` 、`dev` 、`test` by 8:1:1.

#Training
Our code are in version V1, To run training code:
```
cd V1
python flat_main.py --dataset databaker
```
Our proposed rule base are saved in a python file: 
`/V1/add_rule.py`










