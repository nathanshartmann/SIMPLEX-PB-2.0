# SIMPLEX-PB-2.0

This repository contains the results obtained in a paper to be presented in [PROPOR 2020](https://propor.di.uevora.pt).

```
Hartmann, N. S., Paetzold, G. H. and Aluísio, S. M. (2020). A Dataset for the Evaluation of
Lexical Simplification in Portuguese for Children.
International Conference on the Computational Processing of Portuguese (PROPOR 2020).
Evora, Portugal.
```

This paper presents an improved version of SIMPLEX-PB, called SIMPLEX-PB 2.0, a public benchmark dataset for LS that was subject to multiple rounds of manual annotation in order for it to accurately capture the simplification needs of children studying in underprivileged public institutions. It addresses all limitations of the old original SIMPLEX-PB: incorrectly generated synonyms for complex words, low coverage of synonyms, and the absence of reliable simplicity rankings for synonyms.

The dataset was subjected to an enhancement on the number of synonyms for its target complex words (7,31 synonyms on average), and the simplicity rankings introduced were manually provided by the target audience itself – children between 10 and 14 years of age studying in underprivileged public institutions.

The corpora compiled in this work is are available in two formats as follows:

* [SIMPLEX 2.0.json](https://drive.google.com/open?id=16wucBik0Qk3LBdLSc7lzrjVTfmbCMKlE)
* [SIMPLEX 2.0.xlsx](https://drive.google.com/open?id=1SMbj7zkD4rfTtcY-M7PSgoylD4IeN2-p)

Each line in the SIMPLEX-PB 2.0 follows the following format:

> <instance> <sentence> <difficult_word> <POS> <annotated_synonyms> <#annotators> <ranked_synonyms> <ranking_score> <top1_agreement> <top2_agreement> <top3_agreement> <spearman>
  
where,

* **\<instance\>** (label "instância") is the instance id.
* **\<sentence\>** (label "sentença") is the sentence containing a difficult word for children.
* **\<difficult_word\>** (label "palavra_difícil") is the difficult word for children.
* **\<POS\>** (label "pos_tag") is the part-of-speech tag for the difficuld word.
* **\<annotated_synonyms\>** (label "sinônimos_anotados") is the list of synonyms annotated for the difficult word in the given context.
* **\<#annotators\>** (label "nro_de_crianças_que_analisaram") is the amount of children who read the given sentence.
* **\<ranked_synonyms\>** (label "sinônimos_ranqueados") is the list os synonyms ranked by simplicity based on children annotation.
* **\<ranking_score\>** (label "score_do_ranqueamento") is the synonyms ranking gave by the average annotated ranking.
* **\<top1_agreement\>** (label "concordância_top1") is the ranking agreement of the best ranked synonym.
* **\<top2_agreement\>** (label "concordância_top2") is the ranking agreement of the 1st and 2nd best ranked synonym.
* **\<top3_agreement\>** (label "concordância_top3") is the ranking agreement of the 3-best ranked synonym.
* **\<spearman\>** (label "spearman") is the spearman correlation for the synonyms ranking task.
