# headline-entailment


Datasets created in the paper [Improving Truthfulness of Headline Generation](https://www.aclweb.org/anthology/2020.acl-main.123/)

## Gigaword Entailment Dataset

We put datasets of annotation results we conducted against a part of Gigaword dataset in [gigaword directory](https://github.com/nlp-titech/headline-entailment/blob/master/gigaword).

`giga_entail_annotation.tsv` includes 1,000 records of the annotatiton and id of a gigaword article.

`giga_entail_annotation_filtered.tsv` is a subset of `giga_entail_annotation.tsv`.
This subset is created by the same filtering procedure as [Rush et al., 2015](https://github.com/facebookarchive/NAMAS).
We used this version to report the entailment ratio of Gigaword dataset in Section 3.2 of our paper.
