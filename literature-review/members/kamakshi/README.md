# 🧑‍🔬 Research Review Dossier: Kamakshi
*   **Role**: Research Member
*   **Repository Component**: Literature Review (9 Papers)

This directory houses the systematic literature reviews for Kamakshi. Follow the links below to view or edit the respective paper reviews.

---

## 🔬 Section 1: Assigned Papers (Shared Reviews)

1.  **[Paper 1: Deep learning: new computational modelling techniques for genomics](paper-1.md)**
    *   *Nature Reviews Genetics (2019)* | DOI: `10.1038/s41576-019-0122-6`
2.  **[Paper 2: A universal SNP and small-indel variant caller using deep neural networks](paper-2.md)**
    *   *Nature Biotechnology (2018)* | DOI: `10.1038/nbt.4235`
3.  **[Paper 3: An integrated encyclopedia of DNA elements in the human genome](paper-3.md)**
    *   *Nature (2012)* | DOI: `10.1038/nature11247`
4.  **[Paper 4: Cell2location maps fine-grained cell types in spatial transcriptomics](paper-4.md)**
    *   *Nature Biotechnology (2022)* | DOI: `10.1038/s41587-021-01139-4`

---

## 🔬 Section 2: Self-Selected Papers

5.  **[Paper 5: Accurate Proteome-Wide Missense Variant Effect Prediction with AlphaMissense](paper-5.md)**
    *   *Science (2023)* | DOI: `10.1126/science.adg7492`
6.  **[Paper 6: Artificial Intelligence Enables Comprehensive Genome Interpretation and Nomination of Candidate Diagnoses for Rare Genetic Diseases](paper-6.md)**
    *   *Genome Medicine (2021)* | DOI: `10.1186/s13073-021-00965-0`
7.  **[Paper 7: Artificial Intelligence in Variant Calling: A Review](paper-7.md)**
    *   *Journal of Big Data (2024)* | DOI: `10.1186/s40537-024-00947-8`
8.  **[Paper 8: NanoCaller: Accurate Detection of SNPs and Indels in Difficult-to-Map Regions from Long-Read Sequencing by Haplotype-Aware Deep Neural Networks](paper-8.md)**
    *   *Genome Biology (2021)* | DOI: `10.1186/s13059-020-02249-1`
9.  **[Paper 9: MVP Predicts the Pathogenicity of Missense Variants by Deep Learning](paper-9.md)**
    *   *Nature Communications (2021)* | DOI: `10.1038/s41467-020-20847-0`

---

## 🏁 Section 3: Synthesis Summary

## 🔍 Common Themes Across Reviewed Papers

* **Theme 1: Interpretation is the bottleneck, not sequencing.** Across all 9 papers, the core challenge shifts from *generating* genomic data to *making sense of it*. Whether it's calling variants (DeepVariant, NanoCaller, AI Variant Calling review), annotating functional elements (ENCODE), predicting pathogenicity (AlphaMissense, MVP), diagnosing rare disease (GEM), mapping cell types spatially (cell2location), or understanding deep learning's role broadly (Eraslan et al.) - the problem is always downstream of data generation.

* **Theme 2: Deep learning consistently outperforms classical statistical methods.** From CNNs in DeepVariant and NanoCaller, to ResNet in MVP, to Bayesian models in cell2location, to AlphaFold-derived architectures in AlphaMissense - every paper either uses or argues for neural networks over older tools like GATK, SIFT, or PolyPhen2. The Eraslan et al. review paper explicitly frames this as a field-wide shift.

* **Theme 3: Data bias and benchmark inflation are recurring problems.** AlphaMissense, MVP, the AI Variant Calling review, and ENCODE all flag that training or benchmarking on curated databases (ClinVar, HGMD, VariBench) introduces human bias, inflates reported performance, and limits generalizability. Multiple papers design their methodology specifically to avoid this.

* **Theme 4: Integration of multiple data modalities improves results.** NanoCaller integrates long-range haplotype context with local read data; cell2location integrates single-cell RNA-seq with spatial transcriptomics; ENCODE integrates transcription, chromatin, and histone modification data; GEM integrates patient phenotype (HPO terms) with genomic variants. No single data source is sufficient.

* **Theme 5: Everything ultimately points toward clinical utility and rare disease.** GEM, AlphaMissense, MVP, NanoCaller, and even ENCODE explicitly connect their findings to improving diagnosis of rare diseases, increasing diagnostic yield, or accelerating clinical interpretation of genomic data.

## 🛠️ Key Methods/Tools That Appear Repeatedly

* **Convolutional Neural Networks (CNNs) / Deep Residual Networks (ResNets):** Used in DeepVariant (Paper 2), NanoCaller (Paper 8), MVP (Paper 9), and discussed broadly in Eraslan et al. (Paper 1). CNNs have become the default architecture for sequence-level genomic prediction tasks.

* **Bayesian and probabilistic modeling:** Used in GEM (Paper 6) for variant-phenotype scoring, and in cell2location (Paper 4) for spatial deconvolution. Both cases involve handling uncertainty and borrowing statistical strength across multiple data sources.

* **Transfer learning / fine-tuning from foundation models:** AlphaMissense (Paper 5) fine-tunes AlphaFold; DeepVariant (Paper 2) and NanoCaller (Paper 8) adapt models across sequencing platforms. The idea of repurposing a large pretrained model for a downstream genomic task appears multiple times.

* **Population frequency data as weak supervision:** Both AlphaMissense and MVP use population-level variant frequency (gnomAD, ExAC) as a training signal to avoid direct reliance on biased clinical labels - an increasingly common strategy across variant interpretation methods.

## 🕳️ Gaps in Literature Relevant to Our Project

* **Gap 1: Tools are platform-specific and don't generalize well.** NanoCaller, DeepVariant, and the AI Variant Calling review all show significant performance drops when moving across sequencing platforms (e.g. Illumina → Nanopore). A truly platform-agnostic, end-to-end variant calling and interpretation pipeline does not yet exist.

* **Gap 2: No unified pipeline from raw sequencing to clinical diagnosis.** The 9 papers collectively cover separate stages - variant calling (Papers 2, 7, 8), functional annotation (Paper 3), pathogenicity prediction (Papers 5, 9), and diagnosis (Paper 6) - but these stages are not integrated. A gap exists in building a seamless, automated pipeline connecting all steps.

* **Gap 3: Spatial and single-cell genomic data is underutilized in variant interpretation.** cell2location (Paper 4) and ENCODE (Paper 3) show how tissue context and regulatory elements matter, but tools like AlphaMissense and MVP don't incorporate spatial or cell-type-specific expression context when predicting variant pathogenicity.

* **Gap 4: Interpretability of AI models remains unsolved.** The AI Variant Calling review and Eraslan et al. both flag that black-box deep learning models raise trust and regulatory concerns for clinical use. No paper fully solves the interpretability problem, meaning clinicians still can't always understand *why* a model made a prediction.


