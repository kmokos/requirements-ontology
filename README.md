# Requirements Ontology
Our unified requirements ontology architecture allows covering multiple heterogeneous system domains. To this end, it provides a core glossary, in the form of an upper ontology, that contains the necessary terms and associated object descriptions to define various system-specific domain ontologies. Architecture was designed as a modular collection of six ontology categories equiped with classes for specifying requirements at different levels of specification including system, function and interface requirements:

- The System and Attributes Ontology (SAO) contains the core glossary and concepts used as elements of requirement specifications (e.g. system, function, interface, connection, flow, item, state). It plays the role of upper ontology supporting a broad semantic interoperability among a large number of domain-specific ontologies, i.e. it provides a common starting point, for the formulation of definitions.

- The Requirement Boilerplate Ontology (RBO), encodes the elements of requirement specifications in a boilerplate form. More specifically, it provides semantic definitions for the used boilerplates and their placeholders (e.g. main, prefix, suffix). RBO imposes structural constraints in assembling a requirement, thus promoting a formal syntax of well-formed specifications and consequently reducing specification errors. RBO classes are related to classes of the SAO.

- The Domain Specific Ontologies (DSOs) contain domain-specific classes for the system under design. DSOs import all SAO classes and further specialize them.

- The Lexicographic Ontology (LO) contains synonym and antonym semantic definitions for the used boilerplates. It allows using paraphrases inside a boilerplate and contributes to the consistency analysis of requirements.

- The Requirements Definition Ontology (RDO), is the top-level ontology, which defines the mappings and subclassof relationships between different ontologies, while preserving their semantics, and resolving any conflicts and ambiguities. RDO is used as a repository for all requirements and uses elements from the LO and DSO ontologies, following the semantic definitions of RBO. Therefore, RDO imports the RBO, LO and DSO ontologies, and transitively imports (through the DSO ontology) the SAO ontology. Finally, the analysis and classification of all requirements is performed within RDO.

**Ontology architecture is presented in detail in the following publications:**
- K. Mokos, T. Nestoridis, P. Katsaros and N. Bassiliades, "Semantic Modeling and Analysis of Natural Language System Requirements," in IEEE Access, vol. 10, pp. 84094-84119, 2022, doi: 10.1109/ACCESS.2022.3197281, https://ieeexplore.ieee.org/document/9852230.
