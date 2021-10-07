---
layout: page
permalink: /resources/
title: Resources
description: Open-sourced datasets, pretrained transformers, and translation systems.
nav: true
---

## **Datasets** 
Here's a list of datasets that we use in our papers.

- **NewsPH-NLI Dataset**  
*Sentence Entailment Dataset in Filipino*  
First benchmark dataset for sentence entailment in the low-resource Filipino language. Constructed through exploting the structure of news articles. Contains 600,000 premise-hypothesis pairs, in 70-15-15 split for training, validation, and testing. Originally published in [(Cruz et al., 2021)](https://arxiv.org/abs/2010.11574).  
[`download`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/newsph/newsph-nli.zip) &nbsp; [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2021exploiting.txt)


- **WikiText-TL-39**  
*Large Scale Unlabeled Corpora in Filipino*  
Text dataset with 39 Million tokens in the training split. The TL infix refers to Tagalog[^1]. Inspired by the original [WikiText Long Term Dependency dataset](https://blog.einstein.ai/the-wikitext-long-term-dependency-language-modeling-dataset/) (Merity et al., 2016). Published in [Cruz & Cheng (2019)](https://arxiv.org/abs/1907.00409).  
[`download`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/wikitext-tl-39/wikitext-tl-39.zip) &nbsp; [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2019evaluating.txt)  

- **Fake News Filipino Dataset**  
*Low-Resource Fake News Detection Corpora in Filipino*  
The first of its kind. Contains 3,206 expertly-labeled news samples, half of which are real and half of which are fake. Published in [Cruz et al. (2020)](http://www.lrec-conf.org/proceedings/lrec2020/pdf/2020.lrec-1.315.pdf).  
[`download`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/fakenews/fakenews.zip) &nbsp; [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2020localization.txt)  

- **Hate Speech Dataset**  
*Text Classification Dataset in Filipino*  
Contains 10k tweets (training set) that are labeled as hate speech or non-hate speech. Released with 4,232 validation and 4,232 testing samples. Collected during the 2016 Philippine Presidential Elections and originally used in Cabasag et al. (2019). Published in [Cruz & Cheng (2020)](https://arxiv.org/abs/2005.02068).  
[`download (raw)`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/hatenonhate/hatespeech_raw.zip) &nbsp; [`download (processed)`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/hatenonhate/hatespeech_processed.zip) &nbsp; [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2020establishing.txt)  

- **Filipino Dengue Dataset**   
*Low-Resource Multiclass Text Classification Dataset in Filipino*  
Benchmark dataset for low-resource multiclass classification, with 4,015 training, 500 testing, and 500 validation examples, each labeled as part of five classes. Each sample can be a part of multiple classes. Collected as tweets and originally used in Livelo & Cheng (2018). Published in [Cruz & Cheng (2020)](https://arxiv.org/abs/2005.02068).  
[`download (raw)`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/dengue/dengue_raw.zip) &nbsp; [`download (processed)`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/datasets/dengue/dengue_processed.zip) &nbsp; [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2020establishing.txt) 

<br>

## **Pretrained Transformers**
We provide a number of pretrained models in Filipino that you can use for your projects.

#### ELECTRA Models
Tagalog ELECTRA models that we used for [Cruz et al. (2021)](https://arxiv.org/abs/2010.11574) to test the NewsPH-NLI dataset. Our models are available in HuggingFace. Use the discriminator models for downstream tasks, unless you need a mask-filling model, in which case you should use the generator models. [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2021exploiting.txt)  

- [`electra-tagalog-base-cased-discriminator`](https://huggingface.co/jcblaise/electra-tagalog-base-cased-discriminator)
- [`electra-tagalog-base-uncased-discriminator`](https://huggingface.co/jcblaise/electra-tagalog-base-uncased-discriminator)
- [`electra-tagalog-small-cased-discriminator`](https://huggingface.co/jcblaise/electra-tagalog-small-cased-discriminator)
- [`electra-tagalog-small-uncased-discriminator`](https://huggingface.co/jcblaise/electra-tagalog-small-uncased-discriminator)
- [`electra-tagalog-base-cased-generator`](https://huggingface.co/jcblaise/electra-tagalog-base-cased-generator)
- [`electra-tagalog-base-uncased-generator`](https://huggingface.co/jcblaise/electra-tagalog-base-uncased-generator)
- [`electra-tagalog-small-cased-generator`](https://huggingface.co/jcblaise/electra-tagalog-small-cased-generator)
- [`electra-tagalog-small-uncased-generator`](https://huggingface.co/jcblaise/electra-tagalog-small-uncased-generator)

#### BERT Models
Tagalog BERT models for general purpose finetuning. The checkpoints available on HuggingFace are the improved models used in [Cruz & Cheng (2020)](https://arxiv.org/abs/2005.02068). Older versions of the models used in [Cruz et al. (2019)](https://s3.us-east-2.amazonaws.com/blaisecruz.com/assets/undergraduate_thesis.pdf) and [Cruz & Cheng (2019)](https://arxiv.org/abs/1907.00409) are available upon request. [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2020establishing.txt) 

- [`bert-tagalog-base-cased`](https://huggingface.co/jcblaise/bert-tagalog-base-cased)
- [`bert-tagalog-base-uncased`](https://huggingface.co/jcblaise/bert-tagalog-base-uncased)
- [`bert-tagalog-base-cased-WWM`](https://huggingface.co/jcblaise/bert-tagalog-base-cased-WWM)
- [`bert-tagalog-base-uncased-WWM`](https://huggingface.co/jcblaise/bert-tagalog-base-uncased-WWM)
- [`distilbert-tagalog-base-cased`](https://huggingface.co/jcblaise/distilbert-tagalog-base-cased)

#### GPT-2 Models
The Tagalog GPT-2 model used to benchmark our fake news detection system [Cruz et al. (2020)](https://aclanthology.org/2020.lrec-1.316/). We make available an improved version of our GPT-2 model trained with NewsPH in addition to WikiText-TL-39. [`bibtex`](https://s3.us-east-2.amazonaws.com/blaisecruz.com/bib/cruz2020localization.txt) 

- [`gpt2-tagalog`](https://huggingface.co/jcblaise/gpt2-tagalog)


#### Others
Here's a list of other models used for demos, presentations, or proofs-of-concept. 

- [`roberta-tagalog-small`](https://huggingface.co/jcblaise/roberta-tagalog-small) -- Demo version of RoBERTa trained with WikiText-TL-39.
- [`electra-tagalog-small-uncased-discriminator-newsphnli`](https://huggingface.co/jcblaise/electra-tagalog-small-uncased-discriminator-newsphnli) -- ELECTRA model finetuned on NewsPH-NLI for demo purposes.

<br>

## **Translation Models**
Checkpoints for translation systems used for WMT submissions and for research papers are available here.

*Coming Soon*

----

[^1]: It is worth clearing up that the difference between "Filipino" and "Tagalog" is more sociopolitical than sociolinguistic. Given that the Philippines is home to 7000+ spoken languages, Commonwealth Act No. 184 of 1936 created a national committee whose purpose is to "develop a national language" for the country. The result of this is what is knows as "Filipino," which is based on the Tagalog language. In practice, Filipino is identical to Tagalog, with the addition of letters f, j, c , x, and z, plus loanwords. For more information, see this [link](https://ncca.gov.ph/about-ncca-3/subcommissions/subcommission-on-cultural-disseminationscd/language-and-translation/development-of-filipino-the-national-language-of-the-philippines/).