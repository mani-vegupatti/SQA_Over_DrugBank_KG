# SQA_Over_DrugBank_KG

Simple Question Answering Over a Domain-Specific Knowledge Graph using BERT by Transfer Learning

We build and evaluate a baseline for simple Question Answering (QA) (mohammed-etal-2018-strong) over a domain-specific Knowledge Graph (KG) by using a pretrained open-domain language model  BERT\footnote{https://github.com/google-research/bert}. Open-domain refers to a very large collection of coarse-grained facts without restriction to any domain, whereas domain-specific is comparatively smaller in size and fine-grained for a domain such as life sciences, academic, tourism,  etc., (dimitrakis-etal-2019survey)

Training a neural network from scratch for QA task needs a large annotated dataset and creation of such a large dataset is time and resource-intensive. Transfer learning helps to adapt a pretrained Language Model (LM) and finetune for a specific task with less amount of data.

Training a domain-specific LM needs a large amount of domain-specific text, time, and computing power which are scarce, in contrast open-domain LM is trained with easily available large data and pretrained models such as BERT are readily available for download and use. 

For simple QA over a domain-specific KG, often we do not have readily available data for either training the LM or QA task. Hence, we evaluate the usage of open-domain pretrained LM like BERT to create a domain-specific QA baseline model that requires less amount of training data. We built a BioMed domain simple QA system using open-domain pretrained BERT and finetuned with manually curated \textasciitilde 600 QA dataset from the Drug KG published by BIO2RDF \footnote{https://bio2rdf.org/}.
