<a id="top"></a>

# CRATER · Supplementary tables

***Cybersecurity Risk Assessment and Optimal Treatment Framework for AI-based Systems***

Aikaterini Psychogyiou | Aristeidis Farao | Apostolis Zarras | Vaios Bolgouras | Christos Xenakis

[Explore foundations ↓](#foundations) · [View case study ↓](#case-study) · [Code repository ↗](https://github.com/UniPiSSL/CRATER-Cybersecurity-Risk-Assessment-and-Optimal-Treatment-Framework-for-AI-based-Systems)

**Contents**

- [S1 — Asset taxonomy](#s1)
- [S2 — Threat taxonomy](#s2)
- [S3 — Asset–threat correlation](#s3)
- [S4 — Risk-scoring model](#s4)
- [S5 — Control catalogue](#s5)
- [S6 — Control–threat mapping](#s6)
- [S7 — Case-study threat scores](#s7)
- [S8 — Case-study countermeasures](#s8)

**At a glance**

- **36** Component assets — Across 6 categories
- **63** Identified threat types — Across 8 categories
- **52** Reference controls — With applicability mappings

---

<a id="foundations"></a>

## 01 · Foundations

*Reusable reference material: the asset and threat taxonomies, their associations, the risk-scoring definitions, and the full control pool.*

<a id="s1"></a>

### Table S1. Main assets of an AI system

*Six asset categories and their 36 component assets, as defined in the CRATER manuscript.*

| Asset ID | Asset | Asset Description |
|---|---|---|
| <a id="a1"></a>**A1** | **Data** | **Any form of data used in the lifecycle of AI systems, including their training process, deployment, and retraining** |
| <a id="a1-1"></a>A1.1 | Raw data | Unprocessed data collected from various sources before any cleaning or transformation |
| <a id="a1-2"></a>A1.2 | Public data sets | Openly available datasets that can be used for training and testing AI models |
| <a id="a1-3"></a>A1.3 | Training data | Data specifically used to train AI models, helping them learn patterns and make predictions |
| <a id="a1-4"></a>A1.4 | Testing and Validation data | Data used to evaluate the performance of AI models to ensure accuracy and generalisation |
| <a id="a1-5"></a>A1.5 | Log data | Records of AI system operations, including errors, predictions, and performance metrics |
| <a id="a1-6"></a>A1.6 | Metadata | Information describing data attributes, structure, and context, aiding in data management |
| <a id="a2"></a>**A2** | **Models** | **AI models and their components that define how data is processed and interpreted** |
| <a id="a2-1"></a>A2.1 | Algorithms | Mathematical rules and logic used to process and analyse data in AI systems |
| <a id="a2-2"></a>A2.2 | Models | Trained AI structures that make predictions or decisions based on input data |
| <a id="a2-3"></a>A2.3 | Model parameters | Learnt numerical values within an AI model that influence its predictions |
| <a id="a2-4"></a>A2.4 | Hyperparameters | Configurable settings that control the training process and affect model performance |
| <a id="a2-5"></a>A2.5 | Pre-trained models | Models that have been trained on large datasets and can be fine-tuned for specific tasks |
| <a id="a2-6"></a>A2.6 | Model architectures | Structural design of models, such as CNNs for image recognition or Transformers for NLP |
| <a id="a3"></a>**A3** | **Artefacts** | **Supporting components and governance structures essential for AI model management** |
| <a id="a3-1"></a>A3.1 | Data governance policies | Guidelines and protocols for managing data quality, security, and compliance |
| <a id="a3-2"></a>A3.2 | Descriptive statistical parameters | Summary statistics used to analyse data distribution and characteristics |
| <a id="a3-3"></a>A3.3 | Model frameworks | Predefined libraries and architectures that help develop AI models efficiently |
| <a id="a4"></a>**A4** | **Actors/Stakeholders** | **Key individuals or groups involved in the AI development lifecycle** |
| <a id="a4-1"></a>A4.1 | Data owners | Individuals or organisations responsible for data access and management |
| <a id="a4-2"></a>A4.2 | Data scientists | Professionals who design and implement AI models using statistical and machine-learning techniques |
| <a id="a4-3"></a>A4.3 | Data engineers | Experts responsible for processing and managing large-scale datasets |
| <a id="a4-4"></a>A4.4 | Model providers | Organisations or teams that develop and supply AI models for different applications |
| <a id="a4-5"></a>A4.5 | MLOps Engineers | Professionals who manage AI model deployment, monitoring, and maintenance in production |
| <a id="a4-6"></a>A4.6 | Ethics & Compliance Officers | Experts ensuring AI models adhere to ethical standards and legal regulations |
| <a id="a5"></a>**A5** | **Processes** | **Critical workflows involved in AI system development and maintenance** |
| <a id="a5-1"></a>A5.1 | Data ingestion | The process of collecting and importing data from various sources |
| <a id="a5-2"></a>A5.2 | Data Pre-processing | Cleaning and transforming raw data into a usable format |
| <a id="a5-3"></a>A5.3 | Data collection | Gathering data from multiple sources for model training and evaluation |
| <a id="a5-4"></a>A5.4 | Data augmentation | Techniques used to artificially expand datasets to improve model performance |
| <a id="a5-5"></a>A5.5 | Feature selection | Identifying relevant variables that contribute to a model's accuracy |
| <a id="a5-6"></a>A5.6 | Training | The process of teaching an AI model using training datasets |
| <a id="a5-7"></a>A5.7 | Tuning | Adjusting model parameters and hyperparameters to optimise performance |
| <a id="a5-8"></a>A5.8 | Model monitoring | Continuous tracking of AI model performance in production to detect drift |
| <a id="a5-9"></a>A5.9 | Model retraining | Updating models periodically to adapt to new data and maintain accuracy |
| <a id="a6"></a>**A6** | **Environment/Tools** | **Software and platforms that support AI model development and deployment** |
| <a id="a6-1"></a>A6.1 | Algorithm libraries | Prebuilt collections of algorithms used for AI and machine learning |
| <a id="a6-2"></a>A6.2 | ML platforms | Cloud-based or local environments for training and deploying AI models |
| <a id="a6-3"></a>A6.3 | Optimisation techniques | Methods used to enhance AI model performance and efficiency |
| <a id="a6-4"></a>A6.4 | Integrated development environments | Software tools that provide a workspace for coding, debugging, and testing AI applications |
| <a id="a6-5"></a>A6.5 | Edge AI devices | Hardware that enables AI models to run locally on IoT devices or mobile phones |
| <a id="a6-6"></a>A6.6 | Inference engines | Specialised frameworks for running trained AI models efficiently in production |

<sub>[Back to top ↑](#top)</sub>

<a id="s2"></a>

### Table S2. Threat pool

*The complete threat pool: 63 threat types across eight categories.*

| Threat ID | Threat | Threat Description |
|---|---|---|
| <a id="t1"></a>**T1** | **Data risks** | **Threats related to the management and use of data in AI systems.** |
| <a id="t1-1"></a>T1.1 | Input manipulation | Altering the input data provided to AI systems to intentionally mislead or skew outputs. |
| <a id="t1-2"></a>T1.2 | Introducing malicious samples into training data | Deliberate insertion of harmful or misleading data into training datasets, resulting in biased or compromised models. |
| <a id="t1-3"></a>T1.3 | Data integrity breaches | Unauthorised modifications to the data, leading to corrupted training or inaccurate model predictions. |
| <a id="t1-4"></a>T1.4 | Quality of the database | Poor quality datasets (e.g., incomplete, noisy, or outdated data) reducing the reliability and robustness of AI models. |
| <a id="t1-5"></a>T1.5 | Data drift due to external factors such as reward hacking | Changes in real-world patterns or behaviours that render the model's learnt rules less effective, causing AI systems to exploit unintended behaviours in their objectives. |
| <a id="t1-6"></a>T1.6 | Data drift due to seasonal changes | Periodic variations in data (e.g., e-commerce patterns) that reduce model accuracy over time. |
| <a id="t1-7"></a>T1.7 | Data drift due to changes in processes | Organisational or operational changes altering the underlying data distribution, making the AI system less accurate. |
| <a id="t1-8"></a>T1.8 | Concept drift | When the relationship between input data and output labels changes over time, degrading the model's predictive power. |
| <a id="t1-9"></a>T1.9 | Small dataset size | Training AI with insufficient data leads to biased, unreliable, or non-generalisable models. |
| <a id="t2"></a>**T2** | **Attacks** | **Threats arising from malicious attacks on AI systems.** |
| <a id="t2-1"></a>T2.1 | Adversarial attacks | Small, imperceptible perturbations to input data that mislead AI systems. |
| <a id="t2-2"></a>T2.2 | Poisoning attacks | Contaminating training data with malicious samples to degrade model performance or achieve specific outcomes. |
| <a id="t2-3"></a>T2.3 | Inference attacks | Extracting sensitive information about the training dataset by observing the AI model's outputs. |
| <a id="t2-4"></a>T2.4 | Evasion attacks | Crafting inputs to avoid detection or bypass security mechanisms in AI-based systems. |
| <a id="t2-5"></a>T2.5 | Extraction attacks | Reverse-engineering AI models to reconstruct sensitive data or proprietary algorithms. |
| <a id="t2-6"></a>T2.6 | Membership Inference attacks | Identifying whether specific data points were part of the training dataset, potentially breaching privacy. |
| <a id="t2-7"></a>T2.7 | Physical attacks | Manipulating the physical environment (e.g., stickers on stop signs) to deceive AI systems. |
| <a id="t3"></a>**T3** | **Algorithm risks** | **Risks related to AI model algorithms.** |
| <a id="t3-1"></a>T3.1 | Exploiting Generative AI | Using generative models to produce harmful outputs, such as deepfakes or malicious content. |
| <a id="t3-2"></a>T3.2 | Model theft | Unauthorised duplication of proprietary AI models, leading to intellectual property loss and competitive disadvantages. |
| <a id="t3-3"></a>T3.3 | Zero-day vulnerabilities | Exploiting unknown or unpatched weaknesses in AI algorithms or their implementations. |
| <a id="t4"></a>**T4** | **Operational risks** | **Risks from AI system functioning and maintenance.** |
| <a id="t4-1"></a>T4.1 | Compromise of reliability and safety of an AI system due to complex environments | Unpredictable interactions with dynamic environments, causing failures. |
| <a id="t4-2"></a>T4.2 | Responsiveness of the AI | Delays in AI system outputs during critical operations, affecting usability or safety. |
| <a id="t4-3"></a>T4.3 | Loss of expressiveness of models | Models becoming overly simplified and unable to capture complex relationships. |
| <a id="t4-4"></a>T4.4 | Specific failure cases | Unexpected failures under edge-case scenarios. |
| <a id="t4-5"></a>T4.5 | Non-continuous risk monitoring | Lack of real-time or ongoing risk evaluation, leading to undetected vulnerabilities or performance degradation. |
| <a id="t4-6"></a>T4.6 | Inadequate maintenance | Lack of updates or adjustments causing models to degrade over time. |
| <a id="t4-7"></a>T4.7 | Systems with continuous learning | AI systems that learn and adapt over time may incorporate unintended biases, security vulnerabilities, or errors due to a lack of oversight. |
| <a id="t5"></a>**T5** | **Legal/Privacy/ Ethical risks** | **Legal, privacy, and ethical concerns in AI.** |
| <a id="t5-1"></a>T5.1 | Fairness | Models that unintentionally or intentionally reinforce biases, leading to unequal treatment or outcomes. |
| <a id="t5-2"></a>T5.2 | Privacy | Compromises of sensitive user data, either during data collection, processing, or sharing. |
| <a id="t5-3"></a>T5.3 | Degree of automation and control | Excessive automation reducing human oversight, leading to unintended consequences or loss of accountability. |
| <a id="t5-4"></a>T5.4 | Lack of transparency | Opaque decision-making processes, making AI actions hard to understand. |
| <a id="t5-5"></a>T5.5 | Lack of traceability | Challenges in tracking data and processes used in training and deploying AI systems. |
| <a id="t5-6"></a>T5.6 | Lack of explainability | Limited ability to explain how or why an AI model arrived at a specific decision. |
| <a id="t5-7"></a>T5.7 | Lack of reproducibility | Difficulty replicating AI results due to inconsistencies in data, algorithms, or environments. |
| <a id="t5-8"></a>T5.8 | High degree of transparency | Over-disclosure of model details or data potentially exposing sensitive or proprietary information. |
| <a id="t5-9"></a>T5.9 | Data collection and surveillance | Excessive or unethical collection of personal data for AI training. |
| <a id="t5-10"></a>T5.10 | Data misuse and unauthorised access | Exploiting or mishandling data, leading to legal and ethical breaches. |
| <a id="t5-11"></a>T5.11 | Inference and Re-Identification risks | Deriving personally identifiable information from supposedly anonymised datasets. |
| <a id="t5-12"></a>T5.12 | Bias-Discrimination | Systematic unfairness due to flawed training data or biased algorithms. |
| <a id="t5-13"></a>T5.13 | Lack of informed consent | Data subjects not being fully aware or agreeing to how their data is collected or used. |
| <a id="t5-14"></a>T5.14 | Data sharing and Third-Party risks | Vulnerabilities introduced through external data sharing or partnerships. |
| <a id="t5-15"></a>T5.15 | Deepfakes and synthetic data | Misuse of AI-generated content to deceive, manipulate, or harm. |
| <a id="t5-16"></a>T5.16 | Autonomy and behavioural manipulation | Exploiting AI systems to unduly influence user behaviour or decision-making. |
| <a id="t5-17"></a>T5.17 | Limited information communication to stakeholders | Inadequate reporting or disclosure of AI risks, limitations, or decisions to business leaders, policymakers, or regulators. |
| <a id="t5-18"></a>T5.18 | Limited information communication to end users | Users are not provided sufficient explanations about how AI decisions are made, leading to trust and usability concerns. |
| <a id="t6"></a>**T6** | **Technical risks** | **Technical deficiencies and hardware-related issues.** |
| <a id="t6-1"></a>T6.1 | Technical deficiencies | General inadequacies in AI models, such as incorrect assumptions, flawed architectures, or suboptimal implementations that reduce system reliability. |
| <a id="t6-2"></a>T6.2 | Weaknesses in the system hardware / Hardware faults | Hardware components may fail, degrade, or be insufficiently robust, affecting AI model performance. |
| <a id="t6-3"></a>T6.3 | Hardware failures capable of causing a non-negligible shift in model output | Failures or faults in computing hardware (e.g., memory, processors) may alter AI computations, leading to noticeable changes in model behaviour or predictions. |
| <a id="t6-4"></a>T6.4 | System noise can cause a non-negligible shift in model output | Variability in system processes may introduce randomness that affects AI model outputs, potentially leading to inconsistent or inaccurate results. |
| <a id="t6-5"></a>T6.5 | Random hardware failures | Unpredictable faults in hardware components (e.g., bit flips, transient errors) that can disrupt AI computations and lead to incorrect or unstable model outputs. |
| <a id="t6-6"></a>T6.6 | Common cause failures | Failures that stem from a single underlying issue and simultaneously affect multiple components of the AI system. |
| <a id="t6-7"></a>T6.7 | Systematic failures | Consistent and repeatable errors in AI systems due to flaws in design, implementation, or training methodologies. |
| <a id="t6-8"></a>T6.8 | Time-related program errors (race conditions, deadlocks, heisenbugs) | Bugs such as race conditions, deadlocks, or heisenbugs that occur due to timing or concurrency issues, potentially causing unpredictable or incorrect AI system behaviour. |
| <a id="t6-9"></a>T6.9 | Use of technologies with a lower level of maturity | Adoption of AI systems that rely on emerging or unproven technologies, leading to unexpected failures or security risks. |
| <a id="t7"></a>**T7** | **Human variables** | **Risks from human factors in AI systems.** |
| <a id="t7-1"></a>T7.1 | Absence of a critic | The lack of human oversight or critique, which could otherwise identify and correct flaws. |
| <a id="t7-2"></a>T7.2 | Presence of a critic | Reliance on human oversight to detect, interpret, and correct errors or misbehaviours in the AI system. |
| <a id="t7-3"></a>T7.3 | Reaction times | Delayed human responses in critical AI failure scenarios. |
| <a id="t7-4"></a>T7.4 | Understanding | Insufficient understanding of AI systems by users or developers leading to misuse or poor decision-making. |
| <a id="t7-5"></a>T7.5 | Lack of experience | Inexperienced personnel causing errors in deploying or managing AI systems. |
| <a id="t8"></a>**T8** | **Regulatory risks** | **Compliance and regulatory issues.** |
| <a id="t8-1"></a>T8.1 | Non-compliance with data privacy laws | Violations of laws such as GDPR, CCPA, or similar regulations. |
| <a id="t8-2"></a>T8.2 | Non-compliance with AI-specific regulations such as the AI Act | Failure to meet legal requirements designed for AI deployment. |
| <a id="t8-3"></a>T8.3 | Infringements of Intellectual Property and Copyright | Use of copyrighted material in training datasets or unauthorised duplication of AI models. |
| <a id="t8-4"></a>T8.4 | Ethics and Human Rights violations | Breaches of ethical standards or human rights protections in AI applications. |
| <a id="t8-5"></a>T8.5 | Lack of responsible AI governance | Inadequate mechanisms for AI oversight, regulation, or accountability. |

<sub>[Back to top ↑](#top)</sub>

<a id="s3"></a>

### Table S3. Correlation between asset categories and threat categories of AI systems

*Category-level associations between the asset taxonomy and the threat pool.*

| Asset category | [T1](#t1) | [T2](#t2) | [T3](#t3) | [T4](#t4) | [T5](#t5) | [T6](#t6) | [T7](#t7) | [T8](#t8) |
|---|---|---|---|---|---|---|---|---|
| [A1](#a1) — Data | ● | ● | — | — | ● | — | — | ● |
| [A2](#a2) — Models | ● | ● | ● | ● | ● | ● | ● | ● |
| [A3](#a3) — Artefacts | — | — | — | — | ● | — | — | ● |
| [A4](#a4) — Actors/Stakeholders | ● | — | — | — | — | ● | — | ● |
| [A5](#a5) — Processes | ● | — | — | ● | ● | ● | ● | ● |
| [A6](#a6) — Environment/Tools | ● | ● | ● | ● | ● | ● | — | ● |

> ● = association marked in the source. — = blank in the source, not a claim that the threat is impossible. This is an association matrix, not a statistical correlation coefficient matrix.

**Key:** [T1](#t1) Data risks · [T2](#t2) Attacks · [T3](#t3) Algorithm risks · [T4](#t4) Operational risks · [T5](#t5) Legal/Privacy/ Ethical risks · [T6](#t6) Technical risks · [T7](#t7) Human variables · [T8](#t8) Regulatory risks

<sub>[Back to top ↑](#top)</sub>

<a id="s4"></a>

### Table S4. CRATER risk score

*The probability–impact matrix and organisation-level classification, using consistent risk bands and explicit interval boundaries.*

#### How to read the scores

The baseline contribution of each threat–asset pair is I<sub>a,t</sub> × P<sub>a,t</sub>. <br>The manuscript’s ordinal formulation uses scores in {1, 2, 3, 4}: Very Low, Low, High, and Critical for occurrence probability; Negligible, Manageable, High, and Critical for impact. These are ordinal risk scores, not monetary losses or calibrated probabilities.

> L<sub>𝒪</sub> = ∑<sub>a ∈ 𝒜</sub> L<sub>a</sub> = ∑<sub>t ∈ 𝒯, a ∈ 𝒜</sub> (I<sub>a,t</sub> × P<sub>a,t</sub>)

| Probability ↓ / Impact → | Negligible | Manageable | High | Critical |
|---|---|---|---|---|
| Very Low | Minimal | Minimal | Minimal | Minimal |
| Low | Minimal | Minimal | Limited | Limited |
| High | Minimal | Limited | High | Critical |
| Critical | Minimal | Limited | Critical | Critical |

> Single-pair scores are classified as **Minimal (1–4)**, **Limited (5–8)**, **High (9–11)**, and **Critical (12–16)**. The Low probability (2) × Critical impact (4) cell is **Limited** because its score is 8; all other matrix cells are unchanged.

<a id="eq-risk-range"></a>

#### Organisation-level risk classification

Let n ≥ 1 be the number of assessed threat–asset pairs included in the baseline sum L<sub>𝒪</sub>. The qualitative level is determined by the mean score per assessed pair, L<sub>𝒪</sub> / n, using [1, 5), [5, 9), [9, 12), and [12, 16]. Equivalently:

| RiskLevel(L<sub>𝒪</sub>) = | Condition |
|---|---|
| Minimal Risk | n ≤ L<sub>𝒪</sub> < 5n |
| Limited Risk | 5n ≤ L<sub>𝒪</sub> < 9n |
| High Risk | 9n ≤ L<sub>𝒪</sub> < 12n |
| Critical Risk | 12n ≤ L<sub>𝒪</sub> ≤ 16n |

Each lower endpoint is included; each upper endpoint is excluded except the maximum 16n. Thus, a score exactly at 5n, 9n, or 12n belongs to Limited, High, or Critical, respectively. For n = 1, this reproduces the single-pair integer bands. The numeric aggregate remains the sum of the individual contributions; division by n is used only to assign its qualitative level.

For the case study, n = 11: **Minimal** [11, 55); **Limited** [55, 99); **High** [99, 132); and **Critical** [132, 176]. The baseline total L<sub>𝒪</sub> = 120 remains **High**, with a mean score of 120 / 11 ≈ 10.91.

These bounds classify the baseline (uncontrolled) score. The residual-risk formula below is unchanged.

#### Control efficacy and residual risk

The manuscript defines efficacy e<sub>t,a</sub> ∈ [0,1] and a residual multiplier S<sub>t,a</sub> = 1 − e<sub>t,a</sub>. With no control, e = 0 and S = 1. Greater efficacy leaves a smaller residual contribution.

> L<sub>a,t</sub><sup>res</sup> = I<sub>a,t</sub> × P<sub>a,t</sub> × S<sub>t,a</sub>

<sub>[Back to top ↑](#top)</sub>

<a id="s5"></a>

### Table S5. Categorisation of controls and correlation with assets

*The full control pool.*

<details>
<summary><b>Control-pool provenance as described in the manuscript</b></summary>

The paper attributes C1–C24 to MITRE ATLAS, describes C25–C33 as CRATER controls defined on top of CIS Controls Version 8, selects C34–C45 from NIST AI 600-1, and identifies C46–C52 as controls created by the authors. <br>This is the manuscript’s attribution, not an independent verification of those mappings.

**Control types:** **Preventive** measures prevent risks or reduce incident likelihood. **Detective** measures identify incidents or breaches. **Corrective** measures respond to and correct incidents after detection.

</details>

| ID | Control | Control Type | Asset Type correlation |
|---|---|---|---|
| <a id="c1"></a>C1 | Limit Public Release of Information | Preventive | Data, Environment/Tools |
| <a id="c2"></a>C2 | Limit Model Artefact Release | Preventive | Models, Artefacts |
| <a id="c3"></a>C3 | Passive ML Output Obfuscation | Preventive | Models |
| <a id="c4"></a>C4 | Model Hardening | Preventive/ Corrective | Models |
| <a id="c5"></a>C5 | Restrict Number of ML Model Queries | Preventive | Processes |
| <a id="c6"></a>C6 | Control Access to ML Models and Data at Rest | Preventive | Data, Models |
| <a id="c7"></a>C7 | Use Ensemble Methods | Preventive | Models |
| <a id="c8"></a>C8 | Sanitise Training Data | Preventive/ Corrective | Data |
| <a id="c9"></a>C9 | Validate ML Model | Detective/ Corrective | Models |
| <a id="c10"></a>C10 | Use Multi-Modal Sensors | Preventive/ Corrective | Environment/Tools |
| <a id="c11"></a>C11 | Input Restoration | Preventive/ Corrective | Models, Processes |
| <a id="c12"></a>C12 | Restrict Library Loading | Preventive/ Corrective | Environment/Tools |
| <a id="c13"></a>C13 | Encrypt Sensitive Information | Preventive | Data, Models |
| <a id="c14"></a>C14 | Code Signing | Preventive | Artefacts, Environment/Tools |
| <a id="c15"></a>C15 | Verify ML Artefacts | Preventive | Artefacts, Models |
| <a id="c16"></a>C16 | Adversarial Input Detection | Preventive/ Detective | Processes, Models |
| <a id="c17"></a>C17 | Vulnerability Scanning | Detective | Processes, Environment/Tools |
| <a id="c18"></a>C18 | Model Distribution Methods | Preventive/ Corrective | Models, Environment/Tools |
| <a id="c19"></a>C19 | User Training | Preventive | Actors/Stakeholders |
| <a id="c20"></a>C20 | Control Access to ML Models and Data in Production | Preventive | Data, Models |
| <a id="c21"></a>C21 | Generative AI Guardrails | Preventive | Artefacts, Processes |
| <a id="c22"></a>C22 | Generative AI Guidelines | Preventive | Artefacts, Processes |
| <a id="c23"></a>C23 | Generative AI Model Alignment | Preventive | Models, Processes |
| <a id="c24"></a>C24 | AI Telemetry Logging | Preventive/ Detective | Processes, Environment/Tools |
| <a id="c25"></a>C25 | Maintain AI Dataset Provenance | Preventive | Data, Artefacts |
| <a id="c26"></a>C26 | Establish and Maintain an AI Vulnerability Management Process | Preventive/ Corrective | Processes |
| <a id="c27"></a>C27 | Perform Automated Security Updates for AI Models and Pipelines | Preventive/ Corrective | Processes, Models |
| <a id="c28"></a>C28 | Perform Automated Vulnerability Scans of Internal AI Assets | Detective | Processes, Environment/Tools |
| <a id="c29"></a>C29 | Establish and Maintain an AI Security Awareness Programme | Preventive | Actors/Stakeholders |
| <a id="c30"></a>C30 | AI Security and Data Handling Training | Preventive | Actors/Stakeholders, Data |
| <a id="c31"></a>C31 | Establish and Maintain a Secure AI Development and Design | Preventive/ Corrective | Processes |
| <a id="c32"></a>C32 | Conduct AI Penetration Testing | Preventive/ Corrective | Processes, Environment/Tools |
| <a id="c33"></a>C33 | Conduct AI Threat Modelling | Preventive | Processes, Environment/Tools |
| <a id="c34"></a>C34 | Risk Measurement | Preventive/ Corrective | Data/Models |
| <a id="c35"></a>C35 | Team Training | Preventive | Actors/Stakeholders |
| <a id="c36"></a>C36 | Crisis Handling Plan | Corrective | Processes/Environment/Tools |
| <a id="c37"></a>C37 | Role Clarity | Preventive | Actors/Stakeholders |
| <a id="c38"></a>C38 | AI Awareness Training | Preventive | Environment/Tools |
| <a id="c39"></a>C39 | AI Training Programmes | Preventive/ Corrective | Processes |
| <a id="c40"></a>C40 | Oversight Mechanisms | Corrective | Artefacts, Tools |
| <a id="c41"></a>C41 | Privacy Compliance | Preventive | Data |
| <a id="c42"></a>C42 | Regulatory Alignment | Preventive | Data, Models, Processes, Actors/Stakeholders |
| <a id="c43"></a>C43 | IP Protection | Preventive | Models |
| <a id="c44"></a>C44 | Vendor Due Diligence | Preventive/ Corrective | Environment/Tools |
| <a id="c45"></a>C45 | Ethical AI Policies | Preventive | Artefacts |
| <a id="c46"></a>C46 | Data Quality Assurance | Detective | Data, Processes |
| <a id="c47"></a>C47 | Continuous Model Monitoring | Detective | Models, Stakeholders, Processes |
| <a id="c48"></a>C48 | Secure Input Validation | Detective | Data, Environment/Tools |
| <a id="c49"></a>C49 | Bias Detection and Mitigation | Detective | Data, Stakeholders, Processes |
| <a id="c50"></a>C50 | Model Watermarking | Detective/ Preventive | Models, Artefacts |
| <a id="c51"></a>C51 | Model Encryption | Detective/ Preventive | Models |
| <a id="c52"></a>C52 | Secure AI Infrastructure | Detective/ Preventive | Artefacts, Environment/Tools |

<sub>[Back to top ↑](#top)</sub>

<a id="s6"></a>

### Table S6. Application of the newly created controls pool to pre-identified risks

*The complete applicability mapping between the 52 controls and the identified threats.*

| ID | Control | Applies to Risk ID |
|---|---|---|
| <a id="mapping-c1"></a>[C1](#c1) | Limit Public Release of Information | [T2.3](#t2-3) (Inference attacks),<br>[T2.5](#t2-5) (Extraction attacks),<br>[T6.1](#t6-1) (Technical deficiencies) |
| <a id="mapping-c2"></a>[C2](#c2) | Limit Model Artefact Release | [T2.3](#t2-3) (Inference attacks),<br>[T2.5](#t2-5) (Extraction attacks),<br>[T2.6](#t2-6) (Membership Inference attacks),<br>[T3.2](#t3-2) (Model theft) |
| <a id="mapping-c3"></a>[C3](#c3) | Passive ML Output Obfuscation | [T2.3](#t2-3) (Inference attacks) |
| <a id="mapping-c4"></a>[C4](#c4) | Model Hardening | [T2.1](#t2-1) (Adversarial attacks),<br>[T2.4](#t2-4) (Evasion attacks),<br>[T2.7](#t2-7) (Physical attacks) |
| <a id="mapping-c5"></a>[C5](#c5) | Restrict Number of ML Model Queries | [T2.3](#t2-3) (Inference attacks),<br>[T2.5](#t2-5) (Extraction attacks),<br>[T2.6](#t2-6) (Membership Inference attacks) |
| <a id="mapping-c6"></a>[C6](#c6) | Control Access to ML Models and Data at Rest | [T1.3](#t1-3) (Data integrity breaches) |
| <a id="mapping-c7"></a>[C7](#c7) | Use Ensemble Methods | [T1.1](#t1-1) (Input manipulation),<br>[T1.7](#t1-7) (Data drift due to changes in processes),<br>[T1.8](#t1-8) (Concept drift),<br>[T1.9](#t1-9) (Small dataset size),<br>[T2.1](#t2-1) (Adversarial attacks),<br>[T2.4](#t2-4) (Evasion attacks),<br>[T3.1](#t3-1) (Exploiting Generative AI) |
| <a id="mapping-c8"></a>[C8](#c8) | Sanitise Training Data | [T1.2](#t1-2) (Introducing malicious samples),<br>[T1.4](#t1-4) (Quality of the database),<br>[T1.9](#t1-9) (Small dataset size),<br>[T2.2](#t2-2) (Poisoning attacks) |
| <a id="mapping-c9"></a>[C9](#c9) | Validate ML Model | [T1.2](#t1-2) (Introducing malicious samples),<br>[T1.5](#t1-5)-[T1.8](#t1-8) (Data drift due to various factors),<br>[T2.2](#t2-2) (Poisoning attacks),<br>[T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c10"></a>[C10](#c10) | Use Multi-Modal Sensors | [T2.1](#t2-1) (Adversarial attacks),<br>[T2.7](#t2-7) (Physical attacks),<br>[T4.1](#t4-1) (Compromise of reliability and safety),<br>[T6.2](#t6-2)-[T6.6](#t6-6) (Hardware/System risks) |
| <a id="mapping-c11"></a>[C11](#c11) | Input Restoration | [T1.1](#t1-1) (Input manipulation),<br>[T2.7](#t2-7) (Physical attacks) |
| <a id="mapping-c12"></a>[C12](#c12) | Restrict Library Loading | [T6.1](#t6-1)-[T6.9](#t6-9) (Technical risks) |
| <a id="mapping-c13"></a>[C13](#c13) | Encrypt Sensitive Information | [T1.4](#t1-4) (Quality of the database) |
| <a id="mapping-c14"></a>[C14](#c14) | Code Signing | [T3.2](#t3-2) (Model theft),<br>[T6.1](#t6-1)-[T6.9](#t6-9) (Technical risks) |
| <a id="mapping-c15"></a>[C15](#c15) | Verify ML Artefacts | [T1.4](#t1-4) (Quality of the database) |
| <a id="mapping-c16"></a>[C16](#c16) | Adversarial Input Detection | [T1.1](#t1-1) (Input manipulation),<br>[T2.1](#t2-1) (Adversarial attacks),<br>[T2.4](#t2-4) (Evasion attacks) |
| <a id="mapping-c17"></a>[C17](#c17) | Vulnerability Scanning | [T3.3](#t3-3) (Zero day vulnerabilities),<br>[T6.1](#t6-1)-[T6.9](#t6-9) (Technical risks) |
| <a id="mapping-c18"></a>[C18](#c18) | Model Distribution Methods | [T3.2](#t3-2) (Model theft) |
| <a id="mapping-c19"></a>[C19](#c19) | User Training | [T5.1](#t5-1)-[T5.3](#t5-3) (Fairness, Privacy, Automation control),<br>[T7.1](#t7-1)-[T7.5](#t7-5) (Human Variables) |
| <a id="mapping-c20"></a>[C20](#c20) | Control Access to ML Models and Data in Production | [T2.5](#t2-5) (Extraction attacks),<br>[T5.10](#t5-10) Data Misuse and Unauthorised Access |
| <a id="mapping-c21"></a>[C21](#c21) | Generative AI Guardrails | [T3.1](#t3-1) (Exploiting Generative AI) |
| <a id="mapping-c22"></a>[C22](#c22) | Generative AI Guidelines | [T3.1](#t3-1) (Exploiting Generative AI) |
| <a id="mapping-c23"></a>[C23](#c23) | Generative AI Model Alignment | [T3.1](#t3-1) (Exploiting Generative AI) |
| <a id="mapping-c24"></a>[C24](#c24) | AI Telemetry Logging | [T1.5](#t1-5)-[T1.8](#t1-8) (Data drift),<br>[T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c25"></a>[C25](#c25) | Maintain AI Dataset Provenance | [T1.2](#t1-2) (Introducing malicious samples),<br>[T1.4](#t1-4) (Quality of the database),<br>[T2.2](#t2-2) (Poisoning attacks),<br>[T5.14](#t5-14) (Data sharing and Third-Party risks) |
| <a id="mapping-c26"></a>[C26](#c26) | Establish and Maintain an AI Vulnerability Management Process | [T3.3](#t3-3) (Zero day vulnerabilities) |
| <a id="mapping-c27"></a>[C27](#c27) | Perform Automated Security Updates for AI Models and Pipelines | [T1.5](#t1-5)-[T1.8](#t1-8) (Data drift),<br>[T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c28"></a>[C28](#c28) | Perform Automated Vulnerability Scans of Internal AI Assets | [T3.3](#t3-3) (Zero day vulnerabilities) |
| <a id="mapping-c29"></a>[C29](#c29) | Establish and Maintain an AI Security Awareness Programme | [T7.1](#t7-1)-[T7.5](#t7-5) (Human Variables) |
| <a id="mapping-c30"></a>[C30](#c30) | AI Security and Data Handling Training | [T5.2](#t5-2) (Privacy) |
| <a id="mapping-c31"></a>[C31](#c31) | Establish and Maintain a Secure AI Development and Design | [T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c32"></a>[C32](#c32) | Conduct AI Penetration Testing | [T1.1](#t1-1) (Input manipulation),<br>[T2.1](#t2-1) (Adversarial attacks),<br>[T2.4](#t2-4) (Evasion attacks) |
| <a id="mapping-c33"></a>[C33](#c33) | Conduct AI Threat Modelling | [T1.2](#t1-2) (Introducing malicious samples),<br>[T1.9](#t1-9) (Small dataset size),<br>[T2.2](#t2-2) (Poisoning attacks) |
| <a id="mapping-c34"></a>[C34](#c34) | Risk Measurement | [T1.4](#t1-4)-[T1.8](#t1-8) (Quality of the database, Data drift),<br>[T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c35"></a>[C35](#c35) | Team Training | [T7.1](#t7-1)-[T7.5](#t7-5) (Human Variables) |
| <a id="mapping-c36"></a>[C36](#c36) | Crisis Handling Plan | [T4.4](#t4-4) (Specific failure cases) |
| <a id="mapping-c37"></a>[C37](#c37) | Role Clarity | [T7.1](#t7-1)-[T7.5](#t7-5) (Human Variables) |
| <a id="mapping-c38"></a>[C38](#c38) | AI Awareness Training | [T7.1](#t7-1)-[T7.5](#t7-5) (Human Variables) |
| <a id="mapping-c39"></a>[C39](#c39) | AI Training Programmes | [T7.5](#t7-5) (Lack of experience) |
| <a id="mapping-c40"></a>[C40](#c40) | Oversight Mechanisms | [T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c41"></a>[C41](#c41) | Privacy Compliance | [T2.3](#t2-3) (Inference attacks) |
| <a id="mapping-c42"></a>[C42](#c42) | Regulatory Alignment | [T1.3](#t1-3) (Data integrity breaches),<br>[T5.1](#t5-1)-[T5.3](#t5-3) (Fairness, Privacy, Automation control) |
| <a id="mapping-c43"></a>[C43](#c43) | IP Protection | [T1.3](#t1-3) (Data integrity breaches),<br>[T2.3](#t2-3) (Inference attacks),<br>[T2.5](#t2-5) (Extraction attacks),<br>[T3.2](#t3-2) (Model theft) |
| <a id="mapping-c44"></a>[C44](#c44) | Vendor Due Diligence | [T5.7](#t5-7)-[T5.18](#t5-18) (Regulatory risks) |
| <a id="mapping-c45"></a>[C45](#c45) | Ethical AI Policies | [T5.1](#t5-1)-[T5.18](#t5-18) (Legal - Privacy - Ethical risks),<br>[T7.1](#t7-1)-[T7.5](#t7-5) (Human Variables) |
| <a id="mapping-c46"></a>[C46](#c46) | Data Quality Assurance | [T1.2](#t1-2) (Introducing malicious samples),<br>[T1.4](#t1-4) (Quality of the database),<br>[T1.9](#t1-9) (Small dataset size) |
| <a id="mapping-c47"></a>[C47](#c47) | Continuous Model Monitoring | [T1.5](#t1-5)-[T1.8](#t1-8) (Data drift),<br>[T4.1](#t4-1)-[T4.7](#t4-7) (Operational risks) |
| <a id="mapping-c48"></a>[C48](#c48) | Secure Input Validation | [T1.1](#t1-1) (Input manipulation),<br>[T2.1](#t2-1) (Adversarial attacks) |
| <a id="mapping-c49"></a>[C49](#c49) | Bias Detection and Mitigation | [T5.1](#t5-1)-[T5.3](#t5-3) (Fairness, Privacy, Automation control),<br>[T7.1](#t7-1) (Absence of a critic) |
| <a id="mapping-c50"></a>[C50](#c50) | Model Watermarking | [T3.2](#t3-2) (Model theft) |
| <a id="mapping-c51"></a>[C51](#c51) | Model Encryption | [T2.5](#t2-5) (Extraction attacks),<br>[T3.2](#t3-2) (Model theft) |
| <a id="mapping-c52"></a>[C52](#c52) | Secure AI Infrastructure | [T6.1](#t6-1)-[T6.9](#t6-9) (Technical risks) |

> Select a threat identifier to view its definition in [S2](#s2), or a control identifier to view its type and asset associations in [S5](#s5).

<sub>[Back to top ↑](#top)</sub>

---

<a id="case-study"></a>

## 02 · Applied case study

*An illustrative AI-system assessment, with 11 identified threats and eight candidate control applications drawn from the control pool.*

#### Study setting

The manuscript evaluates an illustrative YOLOv5 real-time object-detection pipeline using indoor cafeteria cameras. Periodic retraining incorporates field images and publicly available datasets. The modelled adversary pursues a poisoning objective ([T2.2](#t2-2)) through three paths.

- **11** Assessed threat–asset pairs
- **120** Baseline risk score
- **100 m.u.** Experimental budget

> Control costs, efficacies, and transition probabilities are illustrative inputs, not empirically calibrated estimates. “m.u.” denotes monetary units; no specific currency is assigned.

<a id="modelled-paths"></a><details>
<summary><b>Modelled attack paths and node meanings</b></summary>

The case study represents threat progression as a directed graph. Each path is an alternative route from **Start**, the initial state, to **F**, the shared poisoning objective ([T2.2](#t2-2)). Intermediate nodes represent threats or weaknesses, and the arrows show the direction of progression in the model.

Labels such as **A**, **t₁** and **p₁** identify graph nodes, not asset categories or threat IDs. For example, node **t₁** represents threat [T5.14](#t5-14), not threat category T1. The plain-text labels `t1` and `p1` in [S7](#s7) denote the same nodes as t₁ and p₁ below.

##### Path 1 — Human Negligence and Organisational Drift

**Start → A → B → C → D → F**

This route begins with insufficient human oversight. Unchecked process changes alter the data received by the system; subsequent retraining can allow misleading patterns to become embedded in the model. Gaps in continuous monitoring allow this deterioration to go unnoticed, creating an opportunity for poisoning.

- **A** — Absence of a critic — [T7.1](#t7-1)
- **B** — Process drift: data drift due to changes in processes — [T1.7](#t1-7)
- **C** — Concept drift — [T1.8](#t1-8)
- **D** — Non-continuous risk monitoring — [T4.5](#t4-5)

##### Path 2 — Data Supply Chain Exploitation via Partnerships

**Start → t₁ → t₂ → t₃ → F**

This route concerns data obtained or processed through external partners. Weaknesses in those partnerships allow malicious samples to enter the training-data supply chain. If verification and quality checks fail, the contaminated data are retained and incorporated into retraining, leading towards the poisoning objective.

- **t₁** — Data sharing and third-party risks — [T5.14](#t5-14)
- **t₂** — Introduction of malicious samples into training data — [T1.2](#t1-2)
- **t₃** — Quality of the database: poor-quality training data — [T1.4](#t1-4)

##### Path 3 — Technical Weakness and Model Sensitivity

**Start → p₁ → p₂ → p₃ → F**

This route focuses on technical limitations in the retraining pipeline. Small training datasets make the model more sensitive to individual samples. Manipulated inputs can therefore exert a disproportionate influence during retraining, contributing to the poisoning objective.

- **p₁** — Technical deficiencies — [T6.1](#t6-1)
- **p₂** — Small dataset size — [T1.9](#t1-9)
- **p₃** — Input manipulation — [T1.1](#t1-1)

##### How the paths relate to the tables

[Table S7](#s7) assigns a baseline risk score to each threat represented by a node, including the common final node **F — Poisoning attacks ([T2.2](#t2-2))**. [Table S8](#s8) shows where candidate controls act along the paths. For example, [C11](#c11) is assigned to **p₂ → p₃** to address input manipulation. The two [C7](#c7) entries refer to separate applications on **A → B** and **B → C**.

##### Which version of Path 3 is used in the payoff calculation?

The reported payoff calculation uses the direct chain **Start → p₁ → p₂ → p₃ → F**. The manuscript also specifies a cross-path link, **p₂ → t₃**, with transition probability **0.13**. This connects the small-dataset node on Path 3 to the poor-data-quality node on Path 2, but it is **excluded from that payoff calculation**. Consequently, 0.13 is not included in the product used to calculate success along the direct Path 3.

In the game model, a path’s success probability is the product of its edge transition probabilities and any control residual multipliers. These transition probabilities are distinct from the **ordinal 1–4 occurrence scores** in S7.

</details>

<a id="s7"></a>

### Table S7. Risk caused per identified threat

*Threats assessed in the illustrative case study, with their graph nodes, ordinal impact and occurrence scores, and baseline risk contributions.*

| Threat <i>t</i> | Node | Threat ID | Impact <i>I</i><sub>a,t</sub> | Occurrence Probability <i>P</i><sub>t,a</sub> | Risk <i>L</i><sub>a,t</sub> |
|---|---|---|---|---|---|
| Absence of a Critic | A | [T7.1](#t7-1) | High-3 | High-3 | High-9 |
| Process Drift | B | [T1.7](#t1-7) | High-3 | High-3 | High-9 |
| Concept Drift | C | [T1.8](#t1-8) | High-3 | High-3 | High-9 |
| Non-Continuous Risk Monitoring | D | [T4.5](#t4-5) | Critical-4 | Critical-4 | Critical-16 |
| Data Sharing and Third-Party Risks | t1 | [T5.14](#t5-14) | Manageable-2 | High-3 | Limited-6 |
| Introduction of Malicious Samples into Training Data | t2 | [T1.2](#t1-2) | Critical-4 | Critical-4 | Critical-16 |
| Quality of the Database | t3 | [T1.4](#t1-4) | High-3 | Critical-4 | Critical-12 |
| Technical Deficiencies | p1 | [T6.1](#t6-1) | High-3 | High-3 | High-9 |
| Small Dataset Size | p2 | [T1.9](#t1-9) | Negligible-1 | Low-2 | Minimal-2 |
| Input Manipulation | p3 | [T1.1](#t1-1) | Critical-4 | Critical-4 | Critical-16 |
| Poisoning Attacks | F | [T2.2](#t2-2) | Critical-4 | Critical-4 | Critical-16 |

> The 11 assessed threat–asset pairs contribute a baseline total of **120**, classified as **High** under the revised interval 99 ≤ L<sub>𝒪</sub> < 132. <br>
> The mean score per pair is 120 / 11 ≈ 10.91. <br>
> This table reports baseline risk, not post-control results. The complete classification rule appears in [S4](#s4).

<sub>[Back to top ↑](#top)</sub>

<a id="s8"></a>

### Table S8. Proposed countermeasures for detected threats

*Candidate control applications for the case-study graph, with their costs, efficacy, residual values, and application steps.*

| Threats | Control ID | Control | Cost | Efficacy (<i>e</i>) | Security Provided (𝒮=1-e) | Step |
|---|---|---|---|---|---|---|
| [T7.1](#t7-1) | [C49](#c49) | Bias Detection | 25 | 0.5 | 0.50 | Start → A |
| [T1.7](#t1-7) | [C7](#c7) | Use Ensemble Methods | 50 | 0.75 | 0.25 | A → B |
| [T1.8](#t1-8) | [C7](#c7) | Use Ensemble Methods | 40 | 0.63 | 0.37 | B → C |
| [T4.5](#t4-5) | [C24](#c24) | AI Telemetry Logging | 30 | 0.43 | 0.57 | C → D |
| [T5.14](#t5-14) | [C25](#c25) | Maintain AI Dataset Provenance | 50 | 0.45 | 0.55 | Start → <i>t</i><sub>1</sub> |
| [T6.1](#t6-1) | [C1](#c1) | Limit Public Release of Information | 35 | 0.63 | 0.37 | Start → <i>p</i><sub>1</sub> |
| [T1.9](#t1-9) | [C46](#c46) | Data Quality Assurance | 60 | 0.30 | 0.70 | <i>p</i><sub>1</sub> → <i>p</i><sub>2</sub> |
| [T1.1](#t1-1) | [C11](#c11) | Input Restoration | 80 | 0.31 | 0.69 | <i>p</i><sub>2</sub> → <i>p</i><sub>3</sub> |

> **Cost:** monetary units, with experimental budget B = 100. <br>
> **Notation:** the manuscript defines S = 1 − e as a residual multiplier, so smaller values leave less residual risk. <br>
> Repeated C7 entries describe separate edge-specific applications. Edges without an assigned control retain S<sub>e</sub> = 1.

<sub>[Back to top ↑](#top)</sub>

---

<sub>CRATER | Supplementary research material.</sub>
