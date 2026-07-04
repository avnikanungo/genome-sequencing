# 📄 Paper 1: Deep learning: new computational modelling techniques for genomics
*   **Journal / Conference**: Nature Reviews Genetics (2019)
*   **DOI**: `10.1038/s41576-019-0122-6`
*   **Link**: [Nature Reviews Genetics](https://www.nature.com/articles/s41576-019-0122-6)

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | _Genomics data sets are too large and complex to be analyzed using traditional algorithms that rely on hard-coded assumptions or manually specified handcrafted features. There is a critical need for highly expressive computational models capable of automatically extracting relevant features and discovering unanticipated biological patterns from exponentially growing genomic data._ |
| **Methodology & Approach** <br>*(2-3 lines)* | _The researchers review the application of diverse deep neural network architectures—including fully connected, convolutional, recurrent, and graph convolutional networks—to supervised machine learning tasks within genomics. The study also examines strategies for integrating multiple data modalities, leveraging transfer learning for limited data sets, and employing unsupervised deep learning methods like autoencoders and GANs._ |
| **Key Results & Findings** <br>*(2-3 lines)* | _Deep learning architectures, particularly CNNs, have established new performance benchmarks for predicting molecular phenotypes, such as chromatin features and transcription factor binding—directly from raw DNA sequences. Additionally, these deep learning models have been successfully utilized as in silico perturbation tools to predict the specific impacts of non-coding genetic variants and have improved technical bioinformatics tasks like data denoising._ |
| **Limitations Identified** <br>*(1-2 lines)* | _Limitations of the paper thus identified are as follows: (i) Deep neural networks often function as "black boxes," making their internal parameters inherently difficult to interpret due to high redundancy and complex nonlinear relationships. (ii) Training multitask models presents significant challenges, as the network is forced to simultaneously optimize and balance multiple loss functions. (iii) Multitask neural networks can struggle when there are severe class imbalances across the different predictive tasks, sometimes ignoring difficult tasks altogether._ |
| **Future Scope** <br>*(2-3 lines)* | _The integration of multimodal data is expected to expand, particularly for applications like spatial transcriptomics where single-cell RNA sequencing is jointly analyzed with cellular imaging. Researchers also anticipate the growing adoption of federated learning to train models without transferring sensitive data (addressing privacy concerns) and an increased focus on predicting causal effects for therapeutic applications._ |
| **Project Relevance** <br>*(1-2 lines)* | _Deep learning models provide highly accurate, data-driven refinements for fundamental genome sequencing pipelines, including automated base calling for novel sequencing technologies and robust variant calling. Moreover, these models are essential for taking newly sequenced genomes and effectively prioritizing or predicting the functional impacts of the discovered non-coding variants._ |
