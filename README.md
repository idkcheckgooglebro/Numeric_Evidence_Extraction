# Numerical Evidence Extraction Benchmark
This repository accompanies the paper:
**Numerical Evidence Extraction from Scientific PDFs: A Systematic Review and Empirical Evaluation**

## Overview

Scientific evidence synthesis increasingly relies on extracting numerical information from tables, figures, and full-text PDF documents. Although numerous extraction tools exist, there is currently no lightweight benchmark that evaluates both numerical extraction performance and context preservation across different document types.

This repository provides the benchmark dataset used in our empirical evaluation, together with ground-truth annotations and evaluation resources.

The benchmark is intended to support reproducible research in:

- Table extraction
- Chart and figure digitization
- Scientific PDF processing
- Numerical evidence extraction
- Context preservation
- Document understanding
- Information extraction
## Repository Structure

```
benchmark/
│
├── dataset/
│   ├── tables/
│   ├── figures/
│   └── full_pdfs/
│
├── ground_truth/
│   ├── tables/
│   ├── figures/
│   └── full_pdfs/
│
├── outputs/
│   ├── Camelot/
│   ├── Docling/
│   ├── Marker/
│   ├── PaddleOCR/
│   ├── DePlot/
│   ├── Unstructured/
│   └── olmOCR2/
│
├── evaluation/
│   ├── evaluate.py
│   ├── metrics.py
│   └── README.md
│
└── README.md
```

---

## Dataset

The benchmark consists of manually curated scientific materials collected from publicly available research articles.

| Category | Samples |
|----------|--------:|
| Tables | 10 |
| Charts/Figures | 6 |
| Full Scientific PDFs | 5 |

The selected documents include simple and complex layouts representative of real-world scientific publications.

---

## Ground Truth

Each benchmark sample is accompanied by manually verified annotations describing the expected numerical extraction results.

Annotations include, where applicable:

- Numerical values
- Variable names
- Units
- Headers
- Captions
- Labels
- Provenance information

Ground-truth files are provided in JSON format.

---

## Evaluation

The benchmark is designed to evaluate multiple aspects of numerical evidence extraction.

Current evaluation includes:

- Numerical extraction accuracy
- Structural reconstruction
- Context preservation
- Document-level completeness
- Qualitative error analysis

Researchers may use their own evaluation metrics or extend the provided scripts.

---

## Evaluated Tools

The benchmark was used to evaluate representative tools including:

- Camelot
- Docling
- Marker
- PaddleOCR
- Unstructured.io
- DePlot
- olmOCR2

Additional tools can easily be evaluated using the same benchmark.

---

## Citation

If you use this benchmark, please cite:

```bibtex
@inproceedings{rajendran2026numerical,
  title={Numerical Evidence Extraction from Scientific PDFs: A Systematic Review and Empirical Evaluation},
  author={Rajendran, Athira Asalatha and Yousef, Tariq and Kotta, Jonne},
  booktitle={Proceedings of KONVENS 2026},
  year={2026}
}
```


## Acknowledgements

This work was carried out as part of research on AI-assisted numerical evidence extraction for scientific literature, with applications to evidence synthesis and Cumulative Impact Assessment (CIA).

---

## Contact

For questions regarding the benchmark, please contact:

Athira Asalatha Rajendran

Email: *your-email*

TalTech – Tallinn University of Technology
