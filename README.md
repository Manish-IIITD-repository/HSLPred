# GPCRsclass: Classification of Amine-Type G-Protein-Coupled Receptors

Welcome to the official documentation for **GPCRsclass**, a computational tool developed to recognize and classify the amine subfamily of G-protein-coupled receptors (GPCRs). Amine-type receptors are major drug targets for treating nervous disorders and psychiatric diseases, making their accurate identification essential for pharmaceutical research.

**Web Server:** [http://www.imtech.res.in/raghava/gpcrsclass/](http://www.imtech.res.in/raghava/gpcrsclass/)

---

## Citation

Bhasin, M., & Raghava, G. P. S. (2005). 
**GPCRsclass: a web tool for the classification of amine type of G-protein-coupled receptors.** *Nucleic Acids Research*, 33(Web Server issue), W143-W147. 
[https://doi.org/10.1093/nar/gki351](https://doi.org/10.1093/nar/gki351)

---

## About the Platform

GPCRsclass utilizes Support Vector Machines (SVM) to classify amine-type receptors based on their primary sequence. The method builds upon the observation that different types of amine receptors have distinct amino acid compositions. It provides a multi-level classification scheme to categorize these receptors into specific subfamilies.

### Classification Hierarchy
The tool classifies receptors into the following subfamilies:
* **Acetylcholine**
* **Adrenoceptor**
* **Dopamine**
* **Histamine**
* **Serotonin**

---

## Key Features

### Prediction Modules
* **Amino Acid Composition**: Classifies receptors based on the frequency of the 20 natural amino acids.
* **Dipeptide Composition**: Utilizes the frequency of pairs of adjacent amino acids to capture local order information.
* **Hybrid Approach**: Combines various sequence-based features to achieve superior classification performance.

### Performance Highlights
* **High Accuracy**: The dipeptide-based SVM model achieved an overall accuracy of 99.4% for classifying the five amine subfamilies.
* **Robust Validation**: Models were rigorously evaluated using 5-fold cross-validation on a dataset of 167 amine-type GPCRs.
* **Low False Positives**: Designed to effectively discriminate amine-type receptors from other types of GPCRs and non-GPCR proteins.

---

## Technical Overview

GPCRsclass leverages the SVM-light package to handle high-dimensional sequence data.

| Feature Type | Number of Descriptors | Accuracy (%) |
| :--- | :--- | :--- |
| **Amino Acid Composition** | 20 | 89.8% |
| **Dipeptide Composition** | 400 | 99.4% |

---

## Model Functionality

* **Subfamily Recognition**: Accurately determines which specific amine ligand (e.g., dopamine vs. serotonin) a query GPCR is likely to bind.
* **Sequence Scanning**: Users can submit one or more protein sequences to identify potential amine-type GPCRs.
* **Detailed Reports**: Provides a probability or confidence score for each predicted subfamily classification.

---

## Applications

* **Drug Discovery**: Identifying novel amine receptors as potential targets for neurological and psychiatric drugs.
* **Genome Annotation**: Automatically classifying GPCR sequences identified in newly sequenced genomes.
* **Structural Biology**: Providing a basis for comparative modeling and docking studies of amine-type receptors.

---

## Contact & Authors

**Prof. Gajendra P. S. Raghava**
Bioinformatics Center, Institute of Microbial Technology, Sector 39A, Chandigarh, India.
**Email**: raghava@imtech.res.in

---

## License

This project is an open-access resource and is available for academic and research use provided the original work is properly credited.
