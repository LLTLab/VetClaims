# VetClaims
This repository contains annotated decisions of the Board of Veterans' Appeals (BVA), an administrative appellate tribunal within the U.S. Department of Veterans Affairs. They are XMI files, conforming to the Apache UIMA Standard.

The annotations were created using Eclipse with a UIMA plugin. The repository also contains the UIMA type system file ("sentenceRoleTypeSystem.xml") needed to view the annotations on Eclipse, within a UIMA Ruta project that contains the Basic Type System. Add an import of this type system to the mainTypeSystem in order to view the annotations.

The decision documents themselves were downloaded from the BVA website. The BVA has fact-finding authority, and the decisions collected here are decisions about veterans' claims for compensation for service-related disability. More information about the BVA, its decisions, and the process for adjudicating disability claims can be found in: Vern R. Walker, Ji Hae Han, Xiang Ni and Kaneyasu Yoseda, "Semantic Types for Computational Legal Reasoning: Propositional Connectives and Sentence Roles in the Veterans’ Claims Dataset," In Proceedings of ICAIL ’17, London, United Kingdom, June 12-16, 2017 (ACM, 10 pages). (A pre-publication version of this paper is also included in this repository.)

The following annotations are about the logical or inferential roles of sentences in adjudicatory decisions, and are designed to facilitate argument mining (the identification and extraction of the elements of argument or reasoning). The LLT Lab employs 10 semantic types of sentence, based on reasoning roles. Details about these types are contained in the above paper. The following is a list and brief description of each sentence type. At the present time, only the first five sentence types, those with a double asterisk ( ** ), are annotated in the documents in this repository. Moreover, only the portions of the decisions dealing with PTSD and related psychological claims are fully annotated for findings of fact, relevant evidence, and evidence-based reasoning.

For any questions or comments on this dataset, please contact us at <LLTLab@Hofstra.edu>.

1. Citation Sentence**. A citation sentence is a sentence whose primary function is to reference legal authorities or other materials, and which usually contains standard notation that encodes useful information about the cited source.

2. Legal-Rule Sentence**. A legal-rule sentence is a sentence that primarily states one or more legal rules in the abstract, without stating whether the conditions of the rule(s) are satisfied in the case being decided.

3. Evidence-Based Finding Sentence**. An evidence-based finding sentence (or simply "finding sentence") is a sentence that primarily states an authoritative finding, conclusion or determination of the trier of fact – a decision made “as a matter of fact” instead of “as a matter of law.”

4. Evidence Sentence**. An evidence sentence is a sentence that primarily states the content of the testimony of a witness, states the content of documents introduced into evidence, or describes other evidence.

5. Evidence-Based Reasoning Sentence**. An evidence-based reasoning sentence is a sentence that primarily reports the trier of fact’s reasoning, based on the evidence, in making the findings of fact. 

6. Legal-Policy Sentence. A legal-policy sentence is a sentence that primarily states one or more legal policies, principles or objectives in the abstract, without reasoning about whether the policy is being applied correctly in the decided case.

7. Policy-Based Reasoning Sentence. A policy-based reasoning sentence is a sentence that primarily applies legal policies to decide legal issues – often to decide whether to adopt or reject a legal rule, but occasionally to decide a finding of fact.

8. Ruling or Holding Sentence. A sentence that states a ruling or holding is a sentence that primarily states, “as a matter of law,” whether some particular legal rule is satisfied in the case, and applies the rule to the specifics of the case.

9. Rule-Based Reasoning Sentence. A sentence that states rule-based reasoning is a sentence that reasons from a foundation of legal rules and facts to a ruling or holding as a matter of law (i.e., a conclusion of law).

10. Procedural-Fact Sentence. A procedural-fact sentence is a sentence that primarily states one or more procedural facts about the specific case, such as what motions were filed or the disposition of the case at the trial level.
