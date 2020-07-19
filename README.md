# headline-entailment

Datasets created in the paper [Improving Truthfulness of Headline Generation](https://www.aclweb.org/anthology/2020.acl-main.123/).

## Gigaword Entailment Dataset

We put datasets of annotation results we conducted against a part of Gigaword dataset in [gigaword directory](https://github.com/nlp-titech/headline-entailment/blob/master/gigaword).

`giga_entail_annotation.tsv` includes 1,000 records of the annotatiton and id of a gigaword article.

`giga_entail_annotation_filtered.tsv` is a subset of `giga_entail_annotation.tsv`.
This subset is created by the same filtering procedure as [Rush et al., 2015](https://github.com/facebookarchive/NAMAS).
We used this version to report the entailment ratio of Gigaword dataset in Section 3.2 of our paper.

The meaning of each column is:

| Header | Description |
| ------------- | ------------- |
| id | The id of articles in the original English Gigaword dataset ([Graff and Cieri, 2003](https://catalog.ldc.upenn.edu/LDC2003T05); [Napoles et al., 2012](https://catalog.ldc.upenn.edu/LDC2012T21)) |
| lead1_worker{1-3} | The result of worker {1-3} determining whether the first sentence of the article entails its headline. 1 is entailment, 2 is non-entailment, and 3 is incomprehensible. |
| full_worker{1-3} | Same as `lead1_worker` but full article is used instead of lead-1. |
| lead1_result | Majority vote among the results of the annotation. If every worker has different annotations, the result is 0. |
| full_result | Same as `lead1_result` |
