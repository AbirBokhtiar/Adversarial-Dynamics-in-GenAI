# Systematic Review Methodology

## Overview

This document describes the methodology used for conducting the systematic review on "Adversarial Dynamics in Generative AI". The review follows established systematic review protocols adapted for the rapidly evolving field of AI security.

## Research Questions

### Primary Research Questions

**RQ1**: What are the primary adversarial attack methods targeting generative AI systems (LLMs, VLMs, diffusion models)?

**RQ2**: What defense mechanisms and safety measures have been proposed to protect generative AI systems?

**RQ3**: How effective are current defenses against various attack strategies, and what are their limitations?

**RQ4**: What are the unique security challenges in multi-modal and large-scale generative models?

### Secondary Research Questions

**RQ5**: How do adversarial attacks transfer across different models, architectures, and modalities?

**RQ6**: What evaluation frameworks and benchmarks exist for assessing generative AI security?

**RQ7**: What are the privacy implications of generative AI systems (data extraction, membership inference)?

**RQ8**: What are the emerging trends and future directions in generative AI security?

## Search Strategy

### Information Sources

The systematic search was conducted across multiple academic databases and repositories:

**Primary Sources**:
- arXiv.org (cs.AI, cs.CL, cs.CR, cs.CV, cs.LG)
- Google Scholar
- Semantic Scholar
- Papers with Code

**Conference Proceedings**:
- NeurIPS (Neural Information Processing Systems)
- ICML (International Conference on Machine Learning)
- ICLR (International Conference on Learning Representations)
- ACL (Association for Computational Linguistics)
- EMNLP (Empirical Methods in Natural Language Processing)
- CVPR (Computer Vision and Pattern Recognition)
- USENIX Security Symposium
- IEEE Security & Privacy
- ACM CCS (Computer and Communications Security)

**Journals**:
- Nature Machine Intelligence
- IEEE Transactions on Knowledge and Data Engineering
- Journal of Machine Learning Research
- Nature Communications

### Search Terms

#### Core Concepts
- "adversarial attacks" AND "generative AI"
- "jailbreaking" AND ("LLM" OR "large language model")
- "prompt injection" AND "language model"
- "adversarial examples" AND ("vision-language" OR "multimodal")
- "safety" AND "alignment" AND "language model"

#### Attack-Specific Terms
- "universal adversarial attack"
- "transferable adversarial"
- "jailbreak prompts"
- "backdoor attacks" AND "diffusion models"
- "data poisoning" AND "LLM"
- "prompt injection"
- "visual jailbreak"

#### Defense-Specific Terms
- "adversarial training" AND "LLM"
- "robust optimization" AND "language model"
- "certified defense" AND "neural network"
- "RLHF" OR "reinforcement learning from human feedback"
- "constitutional AI"
- "watermarking" AND ("LLM" OR "diffusion")

#### Application Areas
- "trustworthy AI"
- "AI safety"
- "red teaming"
- "AI security"

### Time Period

- **Primary Period**: 2021-2025 (focus on generative AI era)
- **Foundational Work**: Selected seminal papers from 2017-2020
- **Last Search Date**: February 2026

## Inclusion Criteria

Studies were included if they met ALL of the following criteria:

1. **Relevance**: 
   - Directly addresses security, safety, or adversarial aspects of generative AI systems
   - Covers LLMs, VLMs, diffusion models, or related generative architectures

2. **Scope**:
   - Presents novel attack methods, defense mechanisms, or evaluation frameworks
   - Provides empirical evaluation or theoretical analysis
   - Addresses security implications of generative AI

3. **Quality**:
   - Published in peer-reviewed venues or high-quality preprints
   - Presents clear methodology and reproducible results
   - Makes significant contribution to the field

4. **Accessibility**:
   - Full text available
   - Written in English

5. **Currency**:
   - Published within the review period OR
   - Foundational work frequently cited in recent papers

## Exclusion Criteria

Studies were excluded if they met ANY of the following:

1. **Out of Scope**:
   - Not related to generative AI security
   - Focus solely on traditional ML (non-generative models)
   - Application papers without security analysis

2. **Quality Issues**:
   - Insufficient methodological detail
   - No empirical validation
   - Clear methodological flaws
   - Duplicate publications

3. **Accessibility**:
   - Full text not available
   - Non-English publications
   - Paywalled without institutional access

4. **Type**:
   - Editorials, opinion pieces, or blog posts
   - Workshop abstracts without full papers
   - Patents or technical reports without peer review

## Study Selection Process

### Phase 1: Database Search
1. Executed search queries across all information sources
2. Retrieved approximately 500+ candidate papers
3. Removed duplicates (same paper in multiple databases)
4. Result: ~400 unique papers for screening

### Phase 2: Title and Abstract Screening
1. Two independent reviewers screened titles and abstracts
2. Applied inclusion/exclusion criteria
3. Resolved disagreements through discussion
4. Result: ~150 papers selected for full-text review

### Phase 3: Full-Text Assessment
1. Retrieved and reviewed full texts
2. Applied detailed inclusion/exclusion criteria
3. Assessed quality and relevance
4. Result: 90 papers included in final review

### Phase 4: Forward/Backward Citation Tracking
1. Examined references of included papers (backward)
2. Checked papers citing included studies (forward)
3. Identified additional relevant papers
4. Applied same inclusion/exclusion criteria

## Data Extraction

For each included study, the following information was extracted:

### Bibliographic Information
- Authors and affiliations
- Title and publication year
- Venue (conference/journal)
- DOI and URLs
- Citation count

### Study Characteristics
- Research type (empirical, theoretical, survey, benchmark)
- Primary objective
- Target system (LLM, VLM, diffusion model, etc.)
- Domain of application

### Technical Details

#### For Attack Studies
- Attack category (jailbreaking, backdoor, poisoning, extraction, etc.)
- Attack method and algorithm
- Threat model (white-box, black-box, query-based)
- Success metrics
- Target models tested
- Attack transferability
- Computational requirements

#### For Defense Studies
- Defense category (training-time, inference-time, architectural)
- Defense mechanism
- Effectiveness metrics
- Robustness evaluation
- Computational overhead
- Practical deployment considerations

#### For Evaluation Studies
- Benchmark/framework name
- Evaluation metrics
- Dataset characteristics
- Models evaluated
- Coverage of threat landscape

### Findings
- Key contributions
- Main results
- Limitations acknowledged
- Future work suggested
- Practical implications

## Data Synthesis

### Quantitative Analysis
- Distribution of studies by year
- Distribution by attack/defense category
- Success rates across different methods
- Comparison of defense effectiveness
- Model architecture vulnerabilities

### Qualitative Analysis
- Thematic analysis of attack strategies
- Categorization of defense mechanisms
- Identification of research gaps
- Evolution of research focus
- Emerging trends and patterns

### Classification Framework

#### Attack Taxonomy
1. **Target-based**:
   - Text-to-Text (LLMs)
   - Text-to-Image (Diffusion models)
   - Multi-modal (VLMs)

2. **Stage-based**:
   - Pre-training attacks (poisoning, backdoors)
   - Fine-tuning attacks (instruction hijacking)
   - Inference attacks (jailbreaking, prompt injection)

3. **Method-based**:
   - Optimization-based
   - Prompt engineering
   - Multi-turn strategies
   - Visual attacks
   - Cross-lingual/code-switching

#### Defense Taxonomy
1. **Timing**:
   - Training-time (adversarial training, data filtering)
   - Inference-time (input validation, output filtering)
   - Post-hoc (detection, watermarking)

2. **Approach**:
   - Alignment-based (RLHF, DPO, Constitutional AI)
   - Robustness-based (certified defenses, smoothing)
   - Detection-based (input/output monitors)
   - Architectural (safety layers, instruction hierarchy)

## Quality Assessment

Each paper was assessed on:

1. **Methodological Rigor** (1-5):
   - Clarity of methodology
   - Experimental design
   - Statistical validity

2. **Reproducibility** (1-5):
   - Code availability
   - Dataset availability
   - Implementation details

3. **Impact** (1-5):
   - Citation count
   - Novelty of contribution
   - Influence on subsequent work

4. **Practical Relevance** (1-5):
   - Real-world applicability
   - Scalability considerations
   - Deployment feasibility

## Limitations

### Limitations of This Review

1. **Rapid Evolution**: Field changes faster than review publication cycle
2. **Publication Bias**: Negative results may be underrepresented
3. **Preprint Inclusion**: Some studies not yet peer-reviewed
4. **Language**: Only English-language papers included
5. **Access**: Some papers behind paywalls may have been missed

### Limitations of Included Studies

1. **Evaluation Inconsistency**: Different benchmarks and metrics across studies
2. **Limited Real-World Testing**: Most evaluations on research datasets
3. **Reproducibility**: Not all studies provide code or complete details
4. **Arms Race**: Defenses often bypassed by subsequent attacks
5. **Narrow Scope**: Many studies focus on specific models or settings

## Implications

### For Researchers
- Need for standardized evaluation protocols
- Importance of adaptive attack evaluation
- Value of cross-modal security analysis
- Opportunity for certified defense mechanisms

### For Practitioners
- Multiple defense layers recommended (defense in depth)
- Regular security testing essential
- Monitor for emerging attack techniques
- Balance security with utility and cost

### For Policymakers
- AI safety standards needed for high-risk applications
- Disclosure frameworks for AI vulnerabilities
- Support for AI security research
- International coordination on AI safety

## Future Research Directions

1. **Scalable Certified Defenses**: Provable guarantees for large models
2. **Multi-Modal Security**: Unified frameworks across modalities
3. **Real-World Evaluation**: Beyond academic benchmarks
4. **Adaptive Defenses**: Self-updating security mechanisms
5. **Human-AI Collaboration**: Combining automated and human red teaming
6. **Privacy-Robustness Trade-offs**: Simultaneous privacy and security
7. **Regulatory Compliance**: Technical solutions for policy requirements
8. **Open-Source Tools**: Accessible security evaluation frameworks

## References

See `ref.bib` for the complete bibliography of 90 included studies.

---

**Document Version**: 1.0  
**Last Updated**: February 2026  
**Review Period**: 2021-2025 (with selected foundational work from 2017-2020)
