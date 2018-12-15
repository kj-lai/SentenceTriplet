# SentenceTriplet
Python implementation on extracting triplet, which consists of subject, predicate and object from a sentence. Currently, there are two models being implemented. 

The first model is based on [1], which extracts the first noun subject, last verb as predicate, and the first noun or adjective as subject to form the triplet of a sentence.

The second model is based on [2], which can be considered as an improvement of the first model because it extracts all the subjects, predicates. With this, the model can determine more relations in the sentence.

## Requirements
1. Python 3.6
2. Stanford CoreNLP which can be downloaded from [here](https://stanfordnlp.github.io/CoreNLP/)

## Methodology
1. A sentence is parsed using Stanford CoreNLP Parser as part of the preprocessing stage.
2. Extract all the subjects, predicates and objects from the sentence.
3. Determine relations with the triplets obtained based on the different models.

## References
[[1]](https://www.researchgate.net/publication/228905420_Triplet_extraction_from_sentences) Delia Rusu, Lorand Dali, Blaz Fortuna, Marko Grobelnik, DunjaMladenic, “Triplet extraction from sentences” in Artificial Intelligence Laboratory, Jožef Stefan Institute, Slovenia, Nov. 7, 2008. http://ailab.ijs.si/dunja/SiKDD2007/Papers/Rusu_Trippels.pdf

[[2]](https://www.researchgate.net/publication/215498892_The_Multi-Liaison_Algorithm) The Multi-Liaison algorithm by Ms. Anjali Ganesh Jivani, Ms.AmishaHetalShingala, Dr. Paresh. V. Virparia published in International Journal of Advanced Computer Science and Applications Vol. 2, No. 5, 2011. http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.625.507&rep=rep1&type=pdf
