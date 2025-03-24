# Data used for Population Level Label Distribution Learning Experiments

The datasets were used to evaluate PLDL discussed in these papers.

```
@inproceedings{Liu2019HCOMP,
    title = {{Learning to Predict Population-Level Label Distributions}},
    author = {Liu, Tong and Venkatachalam, Akash and Bongale, Pratik Sanjay and Homan, Christopher M.},
    booktitle = "Proceedings of the Seventh AAAI Conference on Human Computation and Crowdsourcing",
    year = {2019},
    volume = {7},
    number = {1},
    pages = {68--76},
    url = "https://www.aaai.org/ojs/index.php/HCOMP/article/view/5286",
    note = {A preliminary version appears in \cite{Liu2019WWW}},
}
```

```
@inproceedings{Liu2019WWW,
    author = {Liu, Tong and Venkatachalam, Akash and Sanjay Bongale, Pratik and Homan, Christopher},
    title = {Learning to Predict Population-Level Label Distributions},
    year = {2019},
    isbn = {9781450366755},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi.org/10.1145/3308560.3317082},
    doi = {10.1145/3308560.3317082},
    booktitle = {Companion Proceedings of The 2019 World Wide Web Conference},
    pages = {1111–1120},
    numpages = {10},
    keywords = {clustering and classification, Subjectivity in crowdsourcing, label distribution learning, social media.},
    location = {San Francisco, USA},
    series = {WWW ’19}
}
```

# Jobs Dataset

Jobs dataset is a set of Tweets that are job related. The dataset is annotated by annotators from Amazon MTurk and Figure8 (now Appen). The dataset consists of 2,000 tweets and each is annotated by five annotators from each platform. 

### Folder Structure

````
datasets/
└── job_related_dataset/
    └── jobQ1_BOTH/
        ├── jobQ1_BOTH_annotations.json
        ├── jobQ1_BOTH.json
        └── split/
            ├── jobQ1_BOTH_train.json
            ├── jobQ1_BOTH_test.json
            └── jobQ1_BOTH_dev.json
````

This is the structure for JobQ1 (the structure is the same for JobQ2 and JobQ3). The `jobQ1_BOTH_annotations.json` contains annotator level labels for the entire dataset (all train, dev, and test splits combined). Each row in this file represents contains;

* Message ID
* Label choice
* Annotator ID
* Platform (F8 or MT)

`jobQ1_BOTH.json` contains compressed labels for each data item, similar structure to `jobQ1_BOTH_annotations.json` but labels are compressed per item. 

### Citation

```

@inproceedings{Liu2019ACL,
    title = "Understanding Discourse on Work and Job-Related Well-Being in Public Social Media",
    author = "Liu, Tong and Homan, Christopher and Ovesdotter Alm, Cecilia and Lytle, Megan and Marie White, Ann and Kautz, Henry",
    booktitle = "Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = aug,
    year = "2016",
    address = "Berlin, Germany",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/P16-1099",
    doi = "10.18653/v1/P16-1099",
    pages = "1044--1053",
}
```
