# ASR Error Robustness Dataset

## Description

This dataset contains data used in [1]. We propose a data generation pipeline to generate an ASR dataset with ASR errors given its original reference dataset. 
The released dataset contains four parts: 1) SST, 2) TQ, 3) SQuAD (~8.8k samples) and 4) SUBJ (~5.8k samples).


## License
Dataset distribution under the [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0). 
The released dataset originally comes from four public datasets, i.e. SST [2], TQ [3], SQuAD [4], and SUBJ [5]. 
The released modification version is obtained by injecting ASR errors into the original dataset 
(see [1]). 
We appreciate the authors of the four original public datasets.

## How to Download
The dataset is stored at a public Amazon S3 bucket: `asr-error-robustness`. See more in [Open Data on AWS](https://registry.opendata.aws/asr-error-robustness/). 

You will need to install [AWS Command Line Interface](https://aws.amazon.com/cli/) to access the dataset, e.g. to download the dataset, you can use:

```
aws s3 cp s3://asr-error-robustness ~/ --recursive
```

## Reference

1. [Using Phoneme Representations to Build Predictive Models Robust to ASR Errors](https://www.amazon.science/publications/using-phoneme-representations-to-build-predictive-models-robust-to-asr-errors). 2020. Fang et al. In Proceedings of SIGIR.
2. Recursive deep models for semantic compositionality over a sentiment treebank. 2013. Socher et al. In Proceedings of EMNLP. 
3. Learning question classifiers. 2002. Li et al. In Proceedings of COLING.
4. Know What You Don’t Know: Unanswerable Questions for SQuAD. 2018. Rajpurkar et al. In Proceedings of ACL.
5. A sentimental education: Sentiment analysis using subjectivity summarization based on minimum cuts. 2004. Pang et al. In Proceedings of ACL.

