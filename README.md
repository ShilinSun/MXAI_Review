# Literature-MXAI-Review
This is the repository of **A Review of Multimodal Explainable Artificial Intelligence: Past, Present and Future**, a systematic review of Multimodal Explainable Artificial
Intelligence (MXAI) studies in a historical perspective. For details, please refer to: 

**A Review of Multimodal Explainable Artificial Intelligence: Past, Present and Future** [Paper](https://arxiv.org/abs/2412.14056)
## 🔥News
- ☄️ [2024/12/26] We have revised the table of contents, and the remaining sections will be updated progressively.
## Introduction
Artificial intelligence (AI) has rapidly developed through advancements in computational power and the growth of massive datasets. However, this progress has also heightened challenges in interpreting the "black-box" nature of AI models. 

To address these concerns, eXplainable AI (XAI) has emerged with a focus on transparency and interpretability to enhance human understanding and trust in AI decision-making processes. In the context of multimodal data fusion and complex reasoning scenarios, the proposal of Multimodal eXplainable AI (MXAI) integrates multiple modalities for prediction and explanation tasks. Meanwhile, the advent of Large Language Models (LLMs) has led to remarkable breakthroughs in natural language processing, yet their complexity has further exacerbated the issue of MXAI. 

To gain key insights into the development of MXAI methods and provide crucial guidance for building more transparent, fair, and trustworthy AI systems, we review the MXAI methods from a historical perspective and categorize them across four eras: traditional machine learning, deep learning, discriminative foundation models, and generative LLMs. We also review evaluation metrics and datasets used in MXAI research, concluding with a discussion of future challenges and directions. 

**We truly appreciate any contributions through PRs, issues, emails, or other means.**
## Contents

- [Related Surveys](#related-surveys)
- [1. The Era of Traditional Machine Learning (2000-2009)](#1-the-era-of-traditional-machine-learning-2000-2009)
  - [1.1 Data explainability](#11-data-explainability)
    - [1.1.1 Feature selection methods](#111-feature-selection-methods)
      - [Filter](#filter)
      - [Wrapper](#wrapper)
      - [Embedded](#embedded)
    - [1.1.2 Feature extraction methods](#112-feature-extraction-methods)
  - [1.2 Model explainability](#12-model-explainability)
    - [1.2.1 Linear/logistic regression](#121-linearlogistic-regression)
    - [1.2.2 Decision Tree](#122-decision-tree)
    - [1.2.3 K-Nearest Neighbors](#123-k-nearest-neighbors)
    - [1.2.4 Rule-based learning](#124-rule-based-learning)
    - [1.2.5 Bayesian models](#125-bayesian-models)
  - [1.3 Post-hoc explainability](#13-post-hoc-explainability)
    - [1.3.1 Model-agnostic techniques](#131-model-agnostic-techniques)
      - [Causal Explanation](#causal-explanation)
      - [Causal Prediction](#causal-prediction)
      - [Causal Intervention](#causal-intervention)
    - [1.3.2 Model-specific techniques](#132-model-specific-techniques)
      - [Tree ensemble](#tree-ensemble)
      - [Support vector machines](#support-vector-machines)
- [2. The Era of Deep Learning (2011-2016)](#2-the-era-of-deep-learning-2011-2016)
  - [2.1 Data explainability](#21-data-explainability)
    - [2.1.1 Data quality analysis](#211-data-quality-analysis)
    - [2.1.2 Data interaction analysis](#212-data-interaction-analysis)
    - [2.1.3 Inherently interpretable models](#213-inherently-interpretable-models)
  - [2.2 Model explainability](#22-model-explainability)
    - [2.2.1 Deep neural network interpretability](#221-deep-neural-network-interpretability)
      - [Decomposability](#decomposability)
      - [Algorithmic transparency](#algorithmic-transparency)
    - [2.2.2 Explain the training process](#222-explain-the-training-process)
      - [Attention-based networks](#attention-based-networks)
      - [Disentangled representations](#disentangled-representations)
      - [Generate explanations](#generate-explanations)
  - [2.3 Post-hoc explainability](#23-post-hoc-explainability)
    - [2.3.1 Multi-layer neural networks](#231-multi-layer-neural-networks)
      - [Model simplification](#model-simplification)
      - [Feature-related explanations](#feature-related-explanations)
    - [2.3.2 Convolutional Neural Networks](#232-convolutional-neural-networks)
      - [Understand decision-making processes](#understand-decision-making-processes)
      - [Investigate module function](#investigate-module-function)
    - [2.3.3 Recurrent Neural Networks](#233-recurrent-neural-networks)
      - [Feature-related explanations](#feature-related-explanations)
      - [Local explanations](#local-explanations)
- [3. The Era of Discriminative Foundation Models (2017-2021)](#3-the-era-of-discriminative-foundation-models-2017-2021)
  - [3.1 Data explainability](#31-data-explainability)
    - [3.1.1 Analyse multimodal datasets](#311-analyse-multimodal-datasets)
    - [3.1.2 Structural relationship construction](#312-structural-relationship-construction)
  - [3.2 Model explainability](#32-model-explainability)
    - [3.2.1 Behavioral explanation](#321-behavioral-explanation)
      - [Architecture-independent](#architecture-independent) 
      - [Transformer-based](#transformer-based)
      - [CLIP-based](#clip-based)
    - [3.2.2 Structural transparency](#322-structural-transparency)
      - [GNN-based](#gnn-based)
      - [Knowledge Graph-based](#knowledge-graph-based)
      - [Causal-based](#causal-based)
      - [Others](#others)
  - [3.3 Post-hoc explainability](#33-post-hoc-explainability)
    - [3.3.1 Counterfactual-based](#331-counterfactual-based)
    - [3.3.2 Bias mitigation](#332-bias-mitigation)
    - [3.3.3 Multimodal learning process explanation](#333-multimodal-learning-process-explanation)
      - [Multimodal representation](#multimodal-representation)
      - [Multimodal reasoning](#multimodal-reasoning)
      - [Visualization](#visualization)
- [4. The Era of Generative Large Language Models (2022-2024)](#4-the-era-of-generative-large-language-models-2022-2024)
  - [4.1 Data explainability](#41-data-explainability)
    - [4.1.1 explain datasets](#411-explain-datasets)
    - [4.1.2 Data selection](#412-data-selection)
    - [4.1.3 Graph modeling](#413-graph-modeling)
  - [4.2 Model explainability](#42-model-explainability)
    - [4.2.1 Process explanation](#421-process-explanation)
      - [Explain multimodal-ICL](#explain-multimodal-icl)
      - [Explain multimodal-CoT](#explain-multimodal-cot)
      - [Robustness enhancement](#robustness-enhancement)
    - [4.2.2 Explainable data augmentation](#422-explainable-data-augmentation)
      - [Small models training](#small-models-training)
    - [4.2.3 Inherent interpretability](#423-inherent-interpretability)
      - [Image-Text understanding](#image-text-understanding)
      - [Video-Text understanding](#video-text-understanding)
      - [Audio-Text understanding](#audio-text-understanding)
      - [Multimodal-Text understanding](#multimodal-text-understanding)
      - [Classifier-based](#classifier-based)
  - [4.3 Post-hoc explainability](#43-post-hoc-explainability)
    - [4.3.1 Probing-based explanation](#431-probing-based-explanation)
      - [Parameter-free](#parameter-free)
      - [Modular design-based](#modular-design-based)
    - [4.3.2 Reasoning-based explanation](#432-reasoning-based-explanation)
      - [External world knowledge-based](#external-world-knowledge-based)
      - [Feedback-based](#feedback-based)
    - [4.3.3 Example-based explanation](#433-example-based-explanation)
      - [Counterfactual examples](#counterfactual-examples)
      - [Adversarial examples](#adversarial-examples)
- [5. Evaluation datasets and metrics](#5-evaluation-datasets-and-metrics)
## Related Surveys
<details>
<summary>Click to expand the XAI Survey Comparison Table</summary>
  
| Ref. | Published Year | Literature coverage range | Existing surveys are analyzed | MXAI | Transformer explainability | LLMs explainability | Historical perspective | Data explainability | Model explainability | Post-hoc explainability | Evaluation methods | Main theme |
|------|----------------|--------------------------|--------------------------------|------|----------------------------|---------------------|------------------------|--------------------|----------------------|------------------------|-------------------|------------|
| Ours | 2024           | 2000-2024                | ✓                              | ✓    | ✓                          | ✓                   | ✓                      | ✓                  | ✓                    | ✓                      | ✓                 | Historical perspective MXAI |
| [Explainable Generative AI (GenXAI): A Survey, Conceptualization, and Research Agenda](https://arxiv.org/abs/2404.09554) | 2024 | 2016-2024 | × | × | ✓ | ✓ | × | × | × | ✓ | × | Explainable Generative AI |
| [Usable XAI: 10 strategies towards exploiting explainability in the LLM era](https://arxiv.org/abs/2403.08946) | 2024 | 2017-2024 | × | × | ✓ | ✓ | × | × | × | ✓ | ✓ | LLM explainability strategies |
| [Explainability for large language models: A survey](https://dl.acm.org/doi/full/10.1145/3639372) | 2024 | 2017-2024 | × | × | ✓ | ✓ | × | × | × | ✓ | ✓ | LLMs explainability |
| [Rethinking Interpretability in the Era of Large Language Models](https://arxiv.org/abs/2402.01761) | 2024 | 2017-2024 | × | × | × | ✓ | × | ✓ | × | ✓ | ✓ | LLMs explainability |
| [From Understanding to Utilization: A Survey on Explainability for Large Language Models](https://arxiv.org/abs/2401.12874) | 2024 | 2016-2023 | × | × | × | ✓ | × | × | × | ✓ | ✓ | LLMs explainability |
| [Multimodal Explainable Artificial Intelligence: A Comprehensive Review of Methodological Advances and Future Research Directions](https://arxiv.org/abs/2306.05731) | 2023 | 2016-2023 | × | ✓ | × | × | × | × | ✓ | ✓ | ✓ | MXAI |
| [Explainable Artificial Intelligence (XAI) from a user perspective: A synthesis of prior literature and problematizing avenues for future research](https://www.sciencedirect.com/science/article/pii/S0040162522006412) | 2023 | 2008-2022 | ✓ | ✓ | × | × | × | × | × | ✓ | ✓ | User and their concerns |
| [A systematic review of Explainable Artificial Intelligence models and applications: Recent developments and future trends](https://www.sciencedirect.com/science/article/pii/S277266222300070X) | 2023 | 2018-2022 | × | × | × | × | × | × | ✓ | ✓ | × | XAI applications |
|[Explainability of Vision Transformers: A Comprehensive Review and New Perspectives](https://arxiv.org/abs/2311.06786) | 2023 | 2016-2023 | × | × | ✓ | × | × | × | ✓ | ✓ | ✓ | Vision Transformer explainability |
| [Explainability and Evaluation of Vision Transformers: An In-Depth Experimental Study](https://www.mdpi.com/2079-9292/13/1/175) | 2023 | 2016-2023 | × | × | ✓ | × | × | × | ✓ | ✓ | ✓ | Vision Transformer explainability |
| [Towards human-centered explainable ai: A survey of user studies for model explanations](https://ieeexplore.ieee.org/abstract/document/10316181)| 2023 | 2018-2022 | ✓ | × | × | × | × | × | ✓ | ✓ | ✓ | Human-centered XAI |
|[Explainable AI (XAI): A systematic meta-survey of current challenges and future opportunities](https://www.sciencedirect.com/science/article/pii/S0950705123000230) | 2023 | 2017-2021 | ✓ | × | × | × | × | × | ✓ | ✓ | ✓ | Challenges and trends in XAI |
| [Explainable Artificial Intelligence (XAI): What we know and what is left to attain Trustworthy Artificial Intelligence](https://www.sciencedirect.com/science/article/pii/S1566253523001148) | 2022 | 2016-2022 | ✓ | × | × | × | × | ✓ | ✓ | ✓ | ✓ | Model’s trustworthiness |
| [A survey on XAI and natural language explanations](https://www.sciencedirect.com/science/article/abs/pii/S0306457322002126) | 2022 | 2006-2021 | × | × | × | × | × | × | ✓ | ✓ | × | Natural Language Explanations |
| [Knowledge graphs as tools for explainable machine learning: A survey](https://www.sciencedirect.com/science/article/pii/S0004370221001788) | 2022 | 2015-2020 | × | × | × | × | × | × | × | × | × | Knowledge based XAI |
| [Explainable AI methods-a brief overview](https://link.springer.com/chapter/10.1007/978-3-031-04083-2_2?utm_medium=referral&utm_source=slink&utm_content=RM&utm_term=null&utm_campaign=HSCR_BOOKS_AWA1_GL_MPAS_005KU_LNCS50-AA) | 2022 | 2016-2021 | × | × | × | × | × | × | ✓ | ✓ | × | Introduction to XAI |
| [Counterfactual explanations and how to find them: literature review and benchmarking](https://link.springer.com/article/10.1007/s10618-022-00831-6) | 2022 | 2017-2022 | ✓ | × | × | × | × | × | × | ✓ | ✓ | Counterfactual explanations |
| [Explainable AI for time series classification: a review, taxonomy and research directions](https://ieeexplore.ieee.org/abstract/document/9895252) | 2022 | 2018-2022 | ✓ | × | × | × | × | × | × | ✓ | ✓ | XAI for time series |
| [Unbox the black-box for the medical explainable AI via multi-modal and multi-centre data fusion: A mini-review, two showcases and beyond](https://www.sciencedirect.com/science/article/pii/S1566253521001597) | 2022 | 2018-2021 | ✓ | ✓ | × | × | × | × | × | ✓ | × | XAI in healthcare |
| [A survey of contrastive and counterfactual explanation generation methods for explainable artificial intelligence](https://ieeexplore.ieee.org/abstract/document/9321372) | 2021 | 1991-2020 | ✓ | × | × | × | × | × | ✓ | ✓ | ✓ | Contrastive and Counterfactual XAI |
| [Notions of explainability and evaluation approaches for explainable artificial intelligence](https://www.sciencedirect.com/science/article/pii/S1566253521001093) | 2021 | 2015-2020 | ✓ | × | × | × | × | × | × | × | ✓ | Evaluation approaches of XAI |
| [Explainable artificial intelligence: objectives, stakeholders, and future research opportunities](https://www.tandfonline.com/doi/full/10.1080/10580530.2020.1849465) | 2021 | 2017-2020 | × | × | × | × | × | × | × | × | × | Black-box issue |
| [Explainable ai: A review of machine learning interpretability methods](https://www.mdpi.com/1099-4300/23/1/18) | 2021 | 2016-2020 | × | × | × | × | × | × | ✓ | × | × | ML interpretability methods |
| [Explainable artificial intelligence approaches: A survey](https://arxiv.org/abs/2101.09429) | 2021 | 2016-2020 | ✓ | × | × | × | × | × | × | ✓ | × | XAI methods classification |
| [Argumentation and explainable artificial intelligence: a survey](https://www.cambridge.org/core/journals/knowledge-engineering-review/article/argumentation-and-explainable-artificial-intelligence-a-survey/DC6841ED8C7A80DC9EFADF87E4558A1F) | 2021 | 2014-2020 | ✓ | × | × | × | × | × | × | × | × | Argumentation enabling XAI |
| [A Survey on the Explainability of Supervised Machine Learning](https://www.jair.org/index.php/jair/article/view/12228) | 2021 | 2015-2020 | × | × | × | × | × | ✓ | × | ✓ | ✓ | XAI methods classification |
| [Reviewing the need for Explainable Artificial Intelligence (XAI)](https://arxiv.org/abs/2012.01007) | 2021 | 2016-2020 | × | × | × | × | × | × | × | × | × | Necessity of explainability |
| [Explainable Artificial Intelligence (XAI): An Engineering Perspective](https://arxiv.org/abs/2101.03613) | 2021 | 2017-2020 | × | × | × | × | × | × | × | × | × | User and their concerns |
| [What do we want from Explainable Artificial Intelligence (XAI)? – A stakeholder perspective on XAI and a conceptual model guiding interdisciplinary XAI research](https://www.sciencedirect.com/science/article/abs/pii/S0004370221000242) | 2021 | 2016-2021 | × | × | × | × | × | × | × | × | × | User and their concerns |
| [Interpretable deep learning: Interpretation, interpretability, trustworthiness, and beyond](https://link.springer.com/article/10.1007/s10115-022-01756-8) | 2021 | 2016-2020 | × | × | × | × | × | × | ✓ | ✓ | ✓ | XAI methods classification |

</details>

## 1. The Era of Traditional Machine Learning (2000-2009)
### 1.1 Data explainability
#### 1.1.1 Feature selection methods
##### Filter
##### Wrapper 
##### Embedded
#### 1.1.2 Feature extraction methods
### 1.2 Model explainability
#### 1.2.1 Linear/logistic regression
#### 1.2.2 Decision Tree
#### 1.2.3 K-Nearest Neighbors
#### 1.2.4 Rule-based learning
#### 1.2.5 Bayesian models
### 1.3 Post-hoc explainability
#### 1.3.1 Model-agnostic techniques
##### Causal Explanation
##### Causal Prediction
##### Causal Intervention
#### 1.3.2 Model-specific techniques
##### Tree ensemble
##### Support vector machines
## 2. The Era of Deep Learning (2011-2016)

### 2.1 Data explainability

#### 2.1.1 Data quality analysis

#### 2.1.2 Data interaction analysis

#### 2.1.3 Inherently interpretable models

### 2.2 Model explainability

#### 2.2.1 Deep neural network interpretability

##### Decomposability

##### Algorithmic transparency

#### 2.2.2 Explain the training process

##### Attention-based networks

##### Disentangled representations

##### Generate explanations

### 2.3 Post-hoc explainability

#### 2.3.1 Multi-layer neural networks

##### Model simplification

##### Feature-related explanations

#### 2.3.2 Convolutional Neural Networks

##### Understand decision-making processes

##### Investigate module function

#### 2.3.3 Recurrent Neural Networks

##### Feature-related explanations

##### Local explanations


## 3. The Era of Discriminative Foundation Models (2017-2021)

### 3.1 Data explainability

#### 3.1.1 Analyse multimodal datasets

#### 3.1.2 Structural relationship construction

### 3.2 Model explainability

#### 3.2.1 Behavioral explanation

##### Architecture-independent 

##### Transformer-based

##### CLIP-based

#### 3.2.2 Structural transparency

##### GNN-based

##### Knowledge Graph-based

##### Causal-based

##### Others
### 3.3 Post-hoc explainability

#### 3.3.1 Counterfactual-based

#### 3.3.2 Bias mitigation

#### 3.3.3 Multimodal learning process explanation

##### Multimodal representation

##### Multimodal reasoning

##### Visualization

## 4. The Era of Generative Large Language Models (2022-2024)

### 4.1 Data explainability
#### 4.1.1 Explain datasets


#### 4.1.2 Data selection


#### 4.1.3 Graph modeling


### 4.2 Model explainability
#### 4.2.1 Process explanation
##### Process explanation
##### Explain multimodal-ICL
##### Explain multimodal-CoT
##### Robustness enhancement

#### 4.2.2 Explainable data augmentation
##### Explainable data augmentation
##### Small models training

#### 4.2.3 Inherent interpretability
##### Inherent interpretability
##### Image-Text understanding
##### Video-Text understanding
##### Audio-Text understanding
##### Multimodal-Text understanding
##### Classifier-based

### 4.3 Post-hoc explainability
#### 4.3.1 Probing-based explanation
##### Probing-based explanation
##### Parameter-free
##### Modular design-based

#### 4.3.2 Reasoning-based explanation
##### Reasoning-based explanation
##### External world knowledge-based
##### Feedback-based

#### 4.3.3 Example-based explanation
##### Example-based explanation
##### Counterfactual examples
##### Adversarial examples


## 5. Evaluation datasets and metrics

## Citation
If you find this repository useful, please cite our paper:

```
@article{sun2024review,
  title={A Review of Multimodal Explainable Artificial Intelligence: Past, Present and Future},
  author={Sun, Shilin and An, Wenbin and Tian, Feng and Nan, Fang and Liu, Qidong and Liu, Jun and Shah, Nazaraf and Chen, Ping},
  journal={arXiv preprint arXiv:2412.14056},
  year={2024}
}
```
