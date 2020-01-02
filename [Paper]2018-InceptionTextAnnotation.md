# The INCEpTION Platform: Machine-Assisted and Knowledge-Oriented Interactive Annotation

**Authors:** Jan-Christoph Klie, Michael Bugert, Beto Boullosa, Richard Eckart de Castilho, Iryna Gurevych

Ubiquitous Knowledge Processing Lab, Technische Universita ̈t Darmstadt, Germany

**Link:** https://www.aclweb.org/anthology/C18-2002.pdf

**Year:** Aug 2018, ACL, System Demonstration

**Overview**
- Annotation assistance
  - Reach high inter-annotator agreement
  - Active Learning: The goal of active learning (AL) is to quickly reach a good quality of annotation suggestions by soliciting feedback from the user that is expected to be most informative to the underlying machine learning algorithm. Using the uncertainty sampling strategy.
  - Recommenders to continuously monitor the users’ actions, to update/retrain the recommendation models, and to provide always up-to-date suggestions
- Knowledge management 
  - Supports RDF-bases
  - A flexible configuration mechanism is used to support different knowledge representations, such as Wikidata, DBPedia, OWL, CIDOC-CRM, SKOS,
  - Internal databases accessed via SPARQL
  - Knowledge driven annotations: annotating mentions of knowledge base entities in documents (entity linking) or creating new knowledge bases by annotating subjects, predicates and objects in text (fact linking)
  - Entity Linking: take into account the context of the entity mention in order to provide the user with a ranked list of potential candidates. The same approach is used to drive an entity linking recommender which displays high-ranking candidates as annotation suggestions
- Customisability and extensibility: data formats, knowledge resources, text

**Other Annotation Platforms**
Gate Teamware, WebAnno, AlvisAE, Knowtator, Prodi.gy
