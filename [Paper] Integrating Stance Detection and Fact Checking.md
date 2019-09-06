# Integrating Stance Detection and Fact Checking in a Unified Corpus 

**Authors:** Ramy Baly, Mitra Mohtarami, James Glass, Llu ́ıs Ma`rquez , Alessandro Moschitti, Preslav Nakov

**Link:** https://www.aclweb.org/anthology/N18-2004

**Year:** 2018

**Overview**

•	Created an Arabic corpus similar to the Fake News Challenge (FNC), where it is labelled for factuality (true vs false) and stance (agree, disagree, discuss, unrelated). Maybe should ask for the corpus?
•	Performed machine learning models to label the corpus, using the FNC as a baseline. Most models perform similarity, but all models show the best input would be best sentence + rationale, confirming the utility of including the rationale in fact checking

**Corpus Construction**

•	Claim Extraction: Used VERIFY project to extract false claims from corpus, especially those that cannot be verified using textual and NLP techniques; and corrected claims to their original false form. Extract headlines of news documents through manually selected keywords to extract news claims with same topics as those extracted from VERIFY
•	Evidence Extraction: Used Google custom search API for document retrieval. Transformed each claim into subqueries by Named Entity Extraction with the highest TFDF score to use as input into the search API, retrieving first 20 returned links. Then calculated tri-gram containment and cosine distance between average word embedding of links’ content and claims.
•	Stance Annotation: Used CrowdFlower to recruit Arabic speakers to annotate claim-document pair; using 3-5 annotators per pair. 

**Experiments**
•	Experimented with the corpus by first preprocessing it with ATB-style segmentation using: FNC Baseline System, Athene, UCL, Memory Network. 
•	Document content used: full document, best sentence, best sentence + rationale, full document + rationale. Best sentence is measure as most similar to claim by cosine of their average word embeddings. 

**Assumptions**
•	Identifying stance towards claims can help predict their veracity. Hence, the authors associate each claim with supporting and opposing pieces of textual evidence
•	Evidence extracted in Evidence Extraction step were sufficient to the claim
•	Annotators in Stance Annotation step were randomly selected and do not have a bias to Middle Eastern issues. 
