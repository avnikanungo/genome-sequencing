# 📄 Paper 1: Deep learning: new computational modelling techniques for genomics
*   **Journal / Conference**: Nature Reviews Genetics (2019)
*   **DOI**: `10.1038/s41576-019-0122-6`
*   **Link**: [Nature Reviews Genetics](https://www.nature.com/articles/s41576-019-0122-6)

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | Traditional machine learning in genomics depends on manually handcrafted features, which can miss important biological patterns and limit accuracy. This paper reviews how deep learning solves this by learning features directly from raw genomic data through end-to-end learning. |
| **Methodology & Approach** <br>*(2-3 lines)* | It systematically categorizes deep learning architectures - fully connected networks, convolutional neural networks (CNNs), recurrent neural networks (RNNs), and graph convolutional networks (GCNs) - explaining how each works using illustrated genomics examples such as splice-site prediction and transcription factor binding. It also covers advanced strategies (multitask learning, multimodal learning, and transfer learning) and interpretability techniques, supporting its points with real published models as evidence. |
| **Key Results & Findings** <br>*(2-3 lines)* | CNNs emerged as the most successful architecture for DNA sequence tasks, with landmark models such as DeepSEA, Basset, and Basenji outperforming classical approaches like k-mer and SVM-based methods. Multitask and transfer learning consistently improved performance over single-task models, especially when training data was limited. Backpropagation-based interpretability methods, such as DeepLIFT, proved faster and more reliable than perturbation-based approaches. |
| **Limitations Identified** <br>*(1-2 lines)* | Deep learning models remain largely a "black box" and are difficult to interpret. There is a lack of systematic benchmarking between architectures (e.g., RNN vs. CNN) and between interpretability methods. Data privacy for sensitive genomic data also remains an unresolved challenge. |
| **Future Scope** <br>*(2-3 lines)* | The authors anticipate broader integration across omics data types, wider adoption of federated learning for privacy-preserving model training, and the use of generative models for synthetic data sharing. They also highlight causal modelling, spatial transcriptomics, and protein structure prediction (a direction later realized by AlphaFold) as promising future research areas. |
| **Project Relevance** <br>*(1-2 lines)* | This paper provides a strong conceptual foundation for choosing the right deep learning architecture (CNN/RNN/GCN) and training strategy (transfer/multitask learning) based on the type of genomic data used in the project. |
