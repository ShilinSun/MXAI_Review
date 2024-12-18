# Literature-MXAI-Review
This is the repository of A review of Multimodal Explainable Artificial
Intelligence: Past, Present and Future, a systematic survey of Multimodal Explainable Artificial
Intelligence (MXAI) studies in a historical perspective. For details, please refer to: 

A review of Multimodal Explainable Artificial Intelligence: Past, Present and Future [Paper]
## Contents

* [Related Surveys](#related-surveys)
* [The Era of Traditional Machine Learning (2000-2009)](#the-era-of-traditional-machine-learning-2000-2009)
* [The Era of Deep Learning (2010-2016)](#the-era-of-deep-learning-2010-2016)
* [The Era of Discriminative Foundation Models (2017-2021)](#the-era-of-discriminative-foundation-models-2017-2021)
* [The Era of Generative Large Language Models (2022-2024)](#the-era-of-generative-large-language-models-2022-2024)
* [Evaluation datasets and metrics](#evaluation-datasets-and-metrics)
### Related Surveys
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

### The Era of Traditional Machine Learning (2000-2009)

### The Era of Deep Learning (2010-2016)

### The Era of Discriminative Foundation Models (2017-2021)

### The Era of Generative Large Language Models (2022-2024)

### Evaluation datasets and metrics

