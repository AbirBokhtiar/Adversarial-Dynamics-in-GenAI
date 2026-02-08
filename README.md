# Adversarial Dynamics in Generative AI: A Systematic Review

This repository contains the complete materials for a systematic review on adversarial dynamics in Generative AI systems, covering attack methods, defense mechanisms, and security considerations for modern AI systems.

## Overview

Adversarial dynamics in Generative AI encompasses the complex interplay between:
- **Attack Techniques**: Methods that attempt to compromise or manipulate AI systems
- **Defense Mechanisms**: Strategies designed to protect and secure AI systems
- **Evaluation Frameworks**: Benchmarks and methodologies for assessing AI security

This systematic review examines the state-of-the-art in securing generative AI systems, including Large Language Models (LLMs), Vision-Language Models (VLMs), and diffusion models.

## Repository Contents

### 📚 Bibliographic References

**File**: [`systematic_review/ref.bib`](systematic_review/ref.bib)

- **Format**: BibTeX
- **Number of Studies**: 90 carefully selected papers
- **Coverage**: 
  - Adversarial attacks on LLMs and VLMs
  - Jailbreaking techniques and prompt injection
  - Defense mechanisms and safety training
  - Backdoor attacks and poisoning
  - Privacy and watermarking
  - Evaluation frameworks and benchmarks
- **Time Period**: Recent advances in generative AI security (2021-2025)

### 📊 Data Extraction Form

**File**: [`systematic_review/secure_genai_review_master2.xlsx`](systematic_review/secure_genai_review_master2.xlsx)

- **Format**: Microsoft Excel (.xlsx)
- **Contents**: Comprehensive data extraction covering:
  - Study metadata (authors, year, venue, citations)
  - Research objectives and methodology
  - Attack/defense techniques and characteristics
  - Experimental setup and results
  - Key findings and contributions
  - Limitations and future work

### 📄 Review Paper

**File**: [`systematic_review/ReviewPaper.pdf`](systematic_review/ReviewPaper.pdf)

- **Format**: PDF
- **Contents**: Complete systematic review manuscript including:
  - Introduction and background
  - Methodology and search strategy
  - Results and synthesis
  - Discussion and implications
  - Conclusions and future directions

## Key Research Areas Covered

### 1. **Adversarial Attacks on LLMs**
- Jailbreaking techniques (universal prompts, optimization-based attacks)
- Prompt injection and indirect attacks
- Multi-turn and accumulative attacks
- Cipher-based and encoding attacks (ASCII art, code-switching)

### 2. **Multi-Modal Attacks**
- Vision-language model vulnerabilities
- Image hijacks and visual adversarial examples
- Cross-modal jailbreaking
- Compositional adversarial attacks

### 3. **Defense Mechanisms**
- Adversarial training and robust optimization
- Input preprocessing and detection
- Self-reminder and instruction hierarchy
- Certified defenses and safety constraints
- RLHF and preference alignment

### 4. **Data Security**
- Training data extraction and privacy leakage
- Backdoor attacks and trojans
- Poisoning attacks (pre-training, instruction tuning, RAG)
- Model stealing and membership inference

### 5. **Content Protection**
- Watermarking for LLMs and diffusion models
- Style protection for artists (Glaze, adversarial examples)
- Concept erasure and unlearning
- Detection of AI-generated content

### 6. **Evaluation and Benchmarks**
- Red teaming frameworks
- Safety evaluation suites (HarmBench, XSTest)
- Trustworthiness assessments (DecodingTrust, TrustLLM)
- Automated adversarial testing

## Using This Repository

### For Researchers

1. **Literature Review**: Use the BibTeX file to quickly access and cite relevant papers
2. **Data Analysis**: Open the Excel file to explore extracted data and identify research trends
3. **Gap Analysis**: Identify underexplored areas by reviewing the systematic classification
4. **Reproducibility**: Reference the methodology in the review paper for your own systematic reviews

### For Practitioners

1. **Threat Assessment**: Understand current attack vectors and their severity
2. **Defense Selection**: Identify appropriate countermeasures for your specific use case
3. **Best Practices**: Learn from empirical findings across multiple studies
4. **Risk Management**: Use the comprehensive overview to inform security decisions

### For Educators

1. **Course Material**: Use the taxonomy and classification as teaching frameworks
2. **Reading Lists**: Assign papers organized by topic and difficulty level
3. **Discussion Topics**: Leverage research questions and open problems for classroom discussions
4. **Lab Exercises**: Reference attack/defense methods for hands-on security exercises

## Citation

If you use this systematic review in your research, please cite:

```bibtex
@misc{adversarial-dynamics-genai-2024,
  title={Adversarial Dynamics in Generative AI: A Systematic Review},
  author={[Author Names]},
  year={2024},
  publisher={GitHub},
  url={https://github.com/AbirBokhtiar/Adversarial-Dynamics-in-GenAI}
}
```

For citing individual papers from the bibliography, please use the references in `systematic_review/ref.bib`.

## Key Findings Summary

### Current Challenges

1. **Arms Race Dynamics**: Continuous cycle where new defenses are bypassed by stronger attacks
2. **Multi-Modal Vulnerabilities**: Vision-language models face unique security challenges
3. **Alignment Limitations**: Safety training can be circumvented through various techniques
4. **Trade-offs**: Balancing security, utility, and computational efficiency
5. **Evaluation Gaps**: Limited standardization in benchmarks and metrics

### Emerging Trends

1. **Automated Red Teaming**: AI-powered systems for discovering vulnerabilities
2. **Certified Defenses**: Moving towards provable security guarantees
3. **Holistic Safety**: Integration of multiple defense layers
4. **Mechanistic Interpretability**: Understanding internal model representations for security
5. **Regulatory Frameworks**: Development of AI safety standards and guidelines

## Contributing

We welcome contributions to keep this systematic review up-to-date:

- **New Papers**: Suggest recently published papers that fit the scope
- **Data Updates**: Report errors or suggest improvements to the data extraction
- **Discussion**: Share insights and perspectives on the findings
- **Extensions**: Propose additional analysis or visualization

Please open an issue or pull request to contribute.

## License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This systematic review builds upon the pioneering work of researchers in:
- Adversarial machine learning
- AI safety and alignment
- Machine learning security
- Trustworthy AI

We thank all authors of the included studies for their contributions to advancing the field of secure and trustworthy generative AI.

---

**Repository Structure**:
```
.
├── README.md                                    # This file
├── LICENSE                                       # MIT License
└── systematic_review/
    ├── ref.bib                                  # BibTeX bibliography (90 papers)
    ├── secure_genai_review_master2.xlsx         # Data extraction form
    └── ReviewPaper.pdf                          # Complete review manuscript
```

**Last Updated**: February 2026  
**Status**: Active - Covering recent advances in generative AI security