---
title: I would like to test the performance of a sequence-based prediction method: Can I use UniProt to build a negative data set?
type: help
categories: UniProtKB,Text_search,Non-experimental_qualifiers,Sequence,Biocuration,faq
---

The manual curation process of UniProtKB/Swiss-Prot includes extensive literature curation, and the annotation items with experimental evidence can be used to construct positive data sets for predictors of post-translational modifications (PTM) and other events, e.g. [all human entries with experimentally determined signal sequences](https://www.uniprot.org/uniprotkb?query=organism%3A%22homo+sapiens%22+AND+annotation%3A%28type%3Asignal+evidence%3Aexperimental%29+reviewed%3Atrue).

However, the absence of annotation should not be used to build negative data sets: It is only in very rare cases that negative annotation is applied, e.g. entries which are known [not to be glycosylated](https://www.uniprot.org/uniprotkb?query=annotation%3A%28type%3Aptm%20%22not%20glycosylated%22%20evidence%3Aexperimental%29&columns=id%2Centry%20name%2Creviewed%2Cprotein%20names%2Cgenes%2Clength%2Ccomment%28POST-TRANSLATIONAL%20MODIFICATION%29), either the intact protein, or an isoform, or a cleavage product, under certain conditions.

Curating a negative data set requires about as much manual curation as building a positive data set. The absence of an annotation does not mean absence of a function (a true negative). Lack of annotation may simply be due to false negatives: incompleteness either in the state of experiment-derived knowledge of a particular protein's function, or incompleteness in representing that knowledge as annotations, i.e. an entry may not be up-to-date and therefore does not have the positive annotation (yet).

In order to obtain a reliable predictor, we recommend to be extremely conservative when trying to build your set, and in case of doubt contact us about the function or modification you are trying to predict.

# See also

- [Evidence attribution](https://www.uniprot.org/help/evidences)
- [Modified residue](https://www.uniprot.org/help/mod_res)
- [How do we manually annotate a UniProtKB entry?](https://www.uniprot.org/help/manual_curation)
- [How to retrieve sets of protein sequences?](https://www.uniprot.org/help/retrieve_sets)
- [Release cycle, synchronization issues and archival of previous releases](https://www.uniprot.org/help/synchronization)
