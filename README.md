# Adversarial Dynamics in Generative AI

This repository contains a comprehensive systematic review of adversarial dynamics in Generative AI systems, covering attack methods, defense mechanisms, and evaluation frameworks from 2013 to 2024.

## Overview

Adversarial dynamics in Generative AI encompasses the interplay between attack techniques that attempt to compromise AI systems and defense mechanisms designed to protect them. This systematic review examines:

- **Adversarial Attacks**: From traditional gradient-based attacks on image classifiers to modern LLM jailbreaking techniques
- **Defense Mechanisms**: Including adversarial training, certified defenses, input purification, and alignment methods
- **Evaluation Frameworks**: Benchmarks, metrics, and methodologies for assessing adversarial robustness
- **Multi-modal Security**: Unique challenges in securing vision-language and other multi-modal models

## Systematic Review Resources

### 📚 Bibliography

The complete bibliographic list of included studies is available in BibTeX format:

- **File**: [`systematic_review/bibliography.bib`](systematic_review/bibliography.bib)
- **Format**: BibTeX
- **Studies**: 49 carefully selected papers from 2013-2024
- **Coverage**: Computer vision, NLP, multi-modal systems, and LLM security

### 📊 Data Extraction Form

A comprehensive data extraction form containing detailed information about each study:

- **File**: [`systematic_review/data_extraction_form.csv`](systematic_review/data_extraction_form.csv)
- **Format**: CSV (Excel-compatible)
- **Fields**: 27 data points per study including:
  - Bibliographic information (authors, year, venue, DOI)
  - Study characteristics (design, objectives, domain)
  - Technical details (attack/defense methods, success rates, datasets)
  - Analysis (key findings, limitations, quality scores)

### 📖 Methodology Document

Detailed documentation of the systematic review methodology:

- **File**: [`systematic_review/METHODOLOGY.md`](systematic_review/METHODOLOGY.md)
- **Contents**:
  - Research questions and objectives
  - Search strategy and databases
  - Inclusion/exclusion criteria
  - Quality assessment rubric
  - Data extraction process
  - Classification frameworks (attack/defense taxonomies)
  - Limitations and future directions

## Key Findings

### Evolution of Attacks

1. **2013-2017**: Foundation of adversarial ML
   - Discovery of adversarial examples (Szegedy et al., 2014)
   - FGSM and gradient-based attacks (Goodfellow et al., 2014)
   - Physical adversarial examples (Brown et al., 2017)

2. **2017-2020**: Sophisticated attack methods
   - Strong optimization attacks (C&W, Carlini et al., 2017)
   - Universal perturbations (Moosavi-Dezfooli et al., 2017)
   - Transferability and black-box attacks (Papernot et al., 2017)

3. **2020-2024**: LLM and multi-modal attacks
   - Prompt injection and jailbreaking (Zou et al., 2023)
   - Multi-modal adversarial attacks (Qi et al., 2023)
   - Automated red teaming (Perez et al., 2022)

### Defense Mechanisms

1. **Adversarial Training**: Gold standard but computationally expensive (Madry et al., 2018)
2. **Certified Defenses**: Provable guarantees but limited scalability (Raghunathan et al., 2018)
3. **Generative Defenses**: Input purification using GANs (Samangouei et al., 2018)
4. **Alignment Methods**: RLHF and Constitutional AI for LLMs (Bai et al., 2022)
5. **Novel Approaches**: Circuit breakers, instruction hierarchy (Zou et al., 2024)

### Current Challenges

- **Arms Race**: Defenses are often bypassed by stronger attacks
- **Multi-modal Security**: Vision-language models face unique vulnerabilities
- **Scalability**: Many robust training methods don't scale to large models
- **Real-world Gap**: Academic benchmarks may not reflect real-world threats
- **Trade-offs**: Robustness often comes at the cost of accuracy or efficiency

## Using This Repository

### For Researchers

1. **Literature Review**: Use the bibliography as a starting point for research on adversarial AI
2. **Data Analysis**: Import the CSV file for meta-analysis or trend analysis
3. **Methodology Reference**: Adapt our systematic review methodology for your domain
4. **Citation**: Cite relevant papers from our curated list

### For Practitioners

1. **Threat Assessment**: Understand attack vectors relevant to your AI systems
2. **Defense Selection**: Identify appropriate defense mechanisms for your use case
3. **Best Practices**: Learn from the findings and recommendations
4. **Risk Management**: Use quality scores and effectiveness data for risk assessment

### For Educators

1. **Course Material**: Use the taxonomy and classification frameworks for teaching
2. **Reading List**: Assign papers from the bibliography organized by topic/difficulty
3. **Lab Exercises**: Reference methods and datasets for hands-on exercises
4. **Discussion Topics**: Use research questions and limitations for classroom discussions

## Citation

If you use this systematic review in your research, please cite this repository:

```bibtex
@misc{adversarial-dynamics-genai-2024,
  title={Adversarial Dynamics in Generative AI: A Systematic Review},
  author={Repository Contributors},
  year={2024},
  publisher={GitHub},
  url={https://github.com/AbirBokhtiar/Adversarial-Dynamics-in-GenAI}
}
```

## Contributing

We welcome contributions to keep this systematic review up-to-date:

- **New Papers**: Suggest recently published papers that meet our inclusion criteria
- **Corrections**: Report errors in the extracted data or bibliography
- **Extensions**: Propose additional data fields or analysis dimensions
- **Tools**: Contribute scripts for data analysis or visualization

Please open an issue or pull request to contribute.

## License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This systematic review builds upon the foundational work of researchers in adversarial machine learning, AI safety, and machine learning security. We thank all authors of the included studies for their contributions to the field.

---

**Last Updated**: February 8, 2026  
**Status**: Version 1.0 - Covering papers from 2013-2024