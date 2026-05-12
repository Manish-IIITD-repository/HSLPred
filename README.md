# HSLpred: SVM-based Method for Subcellular Localization of Human Proteins

Welcome to the official documentation for **HSLpred**, a computational tool developed for predicting the subcellular localization of human proteins. Accurate localization is essential for understanding the biological function of proteins and their roles in various human diseases. HSLpred utilizes Support Vector Machines (SVM) and integrates diverse protein features, including amino acid composition, dipeptide composition, and similarity-based information, to provide high-accuracy predictions.

**Web Server:** [http://www.imtech.res.in/raghava/hslpred/](http://www.imtech.res.in/raghava/hslpred/)(https://webs.iiitd.edu.in/raghava/hslpred)

---

## Citation

Garg, A., Bhasin, M., & Raghava, G. P. S. (2005). 
**Support Vector Machine-based method for subcellular localization of human proteins using amino acid compositions, their order, and similarity search.** *Journal of Biological Chemistry*, 280(15), 14427–14432. 
[https://doi.org/10.1074/jbc.M411789200](https://doi.org/10.1074/jbc.M411789200)

zenodo:-(https://doi.org/10.5281/zenodo.20140367)

---

## About the Platform

HSLpred is specifically optimized for the human proteome. While many general eukaryotic localization tools exist, HSLpred focuses on the unique characteristics of human proteins to classify them into four major subcellular compartments:
* **Cytoplasm**
* **Mitochondria**
* **Nucleus**
* **Plasma Membrane**

### Key Features
* **SVM Implementation**: Utilizes Support Vector Machines to provide robust and reliable classification.
* **Feature Diversity**: Incorporates traditional amino acid composition, dipeptide composition, and physicochemical properties.
* **Evolutionary Context**: Leverages PSI-BLAST for similarity searches against a non-redundant database of experimentally annotated proteins.
* **Hybrid Modules**: Combines composition-based data with similarity-based data to maximize prediction performance.

---

## Technical Overview

The method was developed and validated using a clean, non-redundant dataset of human proteins.

| Prediction Module | Accuracy (%) |
| :--- | :--- |
| **Amino Acid Composition** | 76.6% |
| **Dipeptide Composition** | 77.8% |
| **PSI-BLAST (Similarity)** | 73.3% |
| **Hybrid (SVM + PSI-BLAST)** | 84.4% |

---

## Model Functionality

HSLpred uses a systematic approach to capture different levels of protein information:

* **Compositional Analysis**: Analyzes the frequency of single amino acids and adjacent pairs (dipeptides) to capture global and local sequence patterns.
* **Similarity Search**: Queries are searched against a curated dataset; if a highly significant hit is found, the localization of the hit is used to guide the prediction.
* **Weighted Integration**: The hybrid module integrates scores from individual components to provide a final localized prediction with high confidence.

---

## Applications

* **Human Proteomics**: Annotating the localization of newly discovered or poorly characterized human proteins.
* **Biomedical Research**: Understanding how mislocalization of proteins contributes to human pathologies.
* **Drug Target Identification**: Identifying proteins in specific compartments (e.g., plasma membrane) that may be accessible for therapeutic intervention.

---

## Contact & Authors

**Prof. Gajendra P. S. Raghava**
Bioinformatics Centre, Institute of Microbial Technology, Sector 39A, Chandigarh, India.
**Email**: raghava@imtech.res.in

---

## License

This project is an open-access resource and is available for academic and research use provided the original work is properly credited.
