---
hide:
  - feedback
tags:
  - ML
  - MlOps
  - Ml security
---
# Впечатляющий MLSecOps 🛡️🤖

[![mm.png](img/mm.png)](img/mm.png)

## Table of Contents
- [Инструменты с открытым исходным кодом](#инструменты-с-открытым-исходным-кодом)
- [Коммерческие инструменты](#коммерческие-инструменты)
- [Данные](#данные)
- [ML Code Security](#безопасность-кода-ml)
- [101](#101-resources)
- [Моделирование угроз](#моделирование-угроз)
- [Фреймворки по безопасности ML(Россия)](#фреймворки-по-безопасности-mlроссия)
- [Векторы атак](#векторы-атак)
- [Блоги и публикаци](#блоги-и-публикации)
- [Инфраструктурные уязвимости MLOps](#инфраструктурные-уязвимости-mlops)
- [MLSecOps pipeline](#mlsecops-pipeline)
- [Academic Po(C)ker FACE](#academic-pocker-face)
- [LLM Defense](#решения-для-защиты-llm)
- [Ресурсы сообщества](#ресурсы-сообщества)
- [Книги и курсы](#книги-и-курсы)
- [Инфографики](#инфографики)
- [Законодательство и постановления](#законодательство-и-постановления)



## Инструменты с открытым исходным кодом

**В этом разделе мы с вами можем рассмотреть, какие opensource решения и PoC существуют для выполнения задачи по защите ML. Конечно, некоторые из них являются не поддерживаемыми или будут возникать трудности с запуском, однако не сказать о них - большое преступление.**


| Инструмент | Описание |
|------------|----------|
| [ModelScan(sast)](https://github.com/protectai/modelscan) | Защита от атак сериализации ML-моделей |
| [NB Defense(sast)](https://protectai.com/nbdefense) | Безопасность Jupyter Notebooks |
| [Garak(dast)](https://github.com/leondz/garak) | Сканер уязвимостей LLM |
| [Adversarial Robustness Toolbox](https://github.com/IBM/adversarial-robustness-toolbox) | Библиотека методов защиты ML-моделей от состязательных атак |
| [MLSploit](https://github.com/mlsploit/) | Облачная платформа для интерактивных экспериментов с исследованиями состязательного машинного обучения |
| [TensorFlow Privacy](https://github.com/tensorflow/privacy) | Библиотека алгоритмов и инструментов машинного обучения с сохранением конфиденциальности |
| [Foolbox](https://github.com/bethgelab/foolbox) | Python-инструментарий для создания и оценки состязательных атак и защит |
| [Advertorch](https://github.com/BorealisAI/advertorch) | Python-инструментарий для исследований состязательной устойчивости |
| [Artificial Intelligence Threat Matrix](https://collaborativeaicontrols.github.io/ATM/) | Фреймворк для выявления и снижения угроз системам машинного обучения |
| [Adversarial ML Threat Matrix](https://github.com/mitre/advmlthreatmatrix) | Карта состязательных угроз для AI-систем |
| [CleverHans](https://github.com/cleverhans-lab/cleverhans) | Библиотека состязательных примеров и защит для моделей машинного обучения |
| [AdvBox](https://github.com/advboxes/AdvBox) | Инструментарий для генерации состязательных примеров, обманывающих нейронные сети в PaddlePaddle, PyTorch, Caffe2, MxNet, Keras, TensorFlow |
| [Audit AI](https://github.com/pymetrics/audit-ai) | Тестирование предвзятости для обобщенных приложений машинного обучения |
| [Deep Pwning](https://github.com/cchio/deep-pwning) | Легковесный фреймворк для экспериментов с моделями машинного обучения с целью оценки их устойчивости против мотивированного противника |
| [Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) | Библиотека с открытым исходным кодом для аудита конфиденциальности данных в статистических алгоритмах и алгоритмах машинного обучения |
| [TensorFlow Model Analysis](https://github.com/tensorflow/model-analysis) | Библиотека для анализа, валидации и мониторинга моделей машинного обучения в продакшене |
| [PromptInject](https://github.com/agencyenterprise/PromptInject) | Фреймворк для составления состязательных промптов |
| [TextAttack](https://github.com/QData/TextAttack) | Python-фреймворк для состязательных атак, аугментации данных и обучения моделей в NLP |
| [OpenAttack](https://github.com/thunlp/OpenAttack) | Пакет с открытым исходным кодом для текстовых состязательных атак |
| [TextFooler](https://github.com/jind11/TextFooler) | Модель для атак на естественный язык в задачах классификации текста и логического вывода |
| [Flawed Machine Learning Security](https://github.com/EthicalML/fml-security) | Практические примеры "Ошибочной безопасности машинного обучения" вместе с лучшими практиками безопасности ML на всех этапах жизненного цикла модели машинного обучения от обучения до упаковки и развертывания |
| [Adversarial Machine Learning CTF](https://github.com/arturmiller/adversarial_ml_ctf) | Задание CTF, демонстрирующее уязвимость большинства (всех?) обычных искусственных нейронных сетей к состязательным изображениям |
| [Damn Vulnerable LLM Project](https://github.com/harishsg993010/DamnVulnerableLLMProject) | Большая языковая модель, разработанная для взлома |
| [Gandalf Lakera](https://gandalf.lakera.ai/) | Площадка для CTF с инъекцией промптов |
| [Prompt Airlines](https://promptairlines.com) | CTF, котоаря похоже на Gandalf|
| [Vigil(dast)](https://github.com/deadbits/vigil-llm) | Сканер инъекций промптов и безопасности LLM |
| [PALLMs (Payloads for Attacking Large Language Models)](https://github.com/mik0w/pallms) | Список различных полезных нагрузок для атак на LLM, собранных в одном месте |
| [AI-exploits](https://github.com/protectai/ai-exploits) | Эксплойты для систем MLOps. Тут не только prompt injections. |
| [Offensive ML Playbook](https://wiki.offsecml.com/Welcome+to+the+Offensive+ML+Playbook) | Руководство по наступательному ML. Заметки об атаках на машинное обучение и тестировании на проникновение |
| [AnonLLM](https://github.com/fsndzomga/anonLLM) | Анонимизация персональной идентифицируемой информации (PII) для API больших языковых моделей |
| [AI Goat](https://github.com/dhammon/ai-goat) | Ещё один CTF для LLM |
| [Pyrit(dast*)](https://github.com/Azure/PyRIT) | Инструмент идентификации рисков на Python для генеративного ИИ |
| [Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors](https://github.com/advmlphish/raze_to_the_ground_aisec23) | Исходный код статьи "Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors", принятой на AISec '23 |
| [Giskard](https://github.com/Giskard-AI/giskard) | Инструмент тестирования с открытым исходным кодом для приложений LLM |
| [Safetensors](https://github.com/huggingface/safetensors) | Конвертация pickle в безопасный вариант сериализации |
| [Citadel Lens](https://www.citadel.co.jp/en/products/lens/) | Тестирование качества моделей в соответствии с отраслевыми стандартами |
| [Model-Inversion-Attack-ToolBox](https://github.com/ffhibnese/Model-Inversion-Attack-ToolBox) | Фреймворк для реализации атак инверсии модели |
| [NeMo-Guardials](https://github.com/NVIDIA/NeMo-Guardrails) | NeMo Guardrails позволяет разработчикам, создающим приложения на основе LLM, легко добавлять программируемые ограничения между кодом приложения и LLM |
| [AugLy](https://github.com/facebookresearch/AugLy) | Инструмент для генерации состязательных атак |
| [Knockoffnets](https://github.com/tribhuvanesh/knockoffnets) | PoC для реализации атак по краже данных модели методом черного ящика |
| [Robust Intelligence Continous Validation](https://www.robustintelligence.com/platform/continuous-validation) | Инструмент для непрерывной валидации модели на соответствие стандартам |
| [VGER](https://github.com/JosephTLucas/vger) | Фреймворк атак для Jupyter |
| [AIShield Watchtower](https://github.com/bosch-aisecurity-aishield/watchtower) | Инструмент с открытым исходным кодом от AIShield для изучения AI-моделей и сканирования уязвимостей |
| [PS-fuzz](https://github.com/prompt-security/ps-fuzz) | Инструмент для сканирования уязвимостей LLM |
| [Mindgard-cli(dast)](https://github.com/Mindgard/cli/) | Проверка безопасности вашего AI через CLI |
| [PurpleLLama3](https://meta-llama.github.io/PurpleLlama/) | Проверка безопасности LLM с помощью бенчмарка Meta LLM |
| [Model transparency](https://github.com/sigstore/model-transparency) | Генерация подписи модели |
| [ARTkit](https://github.com/BCG-X-Official/artkit) | Автоматизированное тестирование и оценка приложений генеративного ИИ на основе промптов |
| [LangBiTe](https://github.com/SOM-Research/LangBiTe) | Фреймворк для тестирования предвзятости LLM |
| [OpenDP](https://github.com/opendp/opendp) | Основная библиотека алгоритмов дифференциальной приватности, лежащая в основе проекта OpenDP |
| [TF-encrypted](https://tf-encrypted.io/) | Шифрование для TensorFlow |



## Коммерческие инструменты

| Инструмент | Описание |
|------------|----------|
| [Databricks Platform, Azure Databricks](https://azure.microsoft.com/ru-ru/products/databricks) | Инструмент управления и внедрения данных в data-lake |
| [Hidden Layer AI Detection Response](https://hiddenlayer.com/aidr/) | Инструмент для обнаружения инцидентов и реагирования на них |
| [Guardian(sast)](https://protectai.com/guardian) | Защита модели в CI/CD |

## ДАННЫЕ

| Инструмент | Описание |
|------------|----------|
| [ARX - Data Anonymization Tool](https://arx.deidentifier.org/) | Инструмент для анонимизации наборов данных |
| [Data-Veil](https://veil.ai/) | Инструмент для маскирования и анонимизации данных |
| [Tool for IMG anonymization](https://github.com/PacktPublishing/Adversarial-AI---Attacks-Mitigations-and-Defense-Strategies/blob/main/ch10/notebooks/Image%20Anonymization.ipynb) | Анонимизация изображений |
| [Tool for DATA anonymization](https://github.com/PacktPublishing/Adversarial-AI---Attacks-Mitigations-and-Defense-Strategies/blob/main/ch10/notebooks/Data%20Anonymization.ipynb) | Анонимизация данных |
| [BMW-Anonymization-Api](https://github.com/BMW-InnovationLab/BMW-Anonymization-API?referral=top-free-anonymization-tools-apis-and-open-source-models) | Этот репозиторий позволяет анонимизировать конфиденциальную информацию на изображениях/видео. Решение полностью совместимо с решениями для обучения/вывода на основе DL |
| [DeepPrivacy2](https://github.com/hukkelas/deep_privacy2) | Инструментарий для реалистичной анонимизации изображений |
| [PPAP](https://github.com/tgisaturday/PPAP) | Анонимизация изображений на уровне латентного пространства с использованием сетей защиты от состязательных атак |

## Безопасность кода ML

| Инструмент | Описание |
|------------|----------|
| [lintML(sast)](https://github.com/JosephTLucas/lintML) | Линтер безопасности для ML от Nvidia |
| [HiddenLayer: Model as Code](https://hiddenlayer.com/research/models-are-code/) | Исследование некоторых векторов в библиотеках ML |
| [Copycat CNN](https://github.com/jeiks/Stealing_DL_Models) | Proof-of-concept о том, как создать копию сверточной нейронной сети |
| [differential-privacy-library](https://github.com/IBM/differential-privacy-library) | Библиотека, предназначенная для дифференциальной приватности и машинного обучения |



## 101 Resources

**Вы можете найти тут перечень ресурсов, которые помогут войти в тему безопасности ИИ: разобраться с тем, какие атаки существуют и как они могут быть использованы злоумышленником.**

- [AI Security 101](https://www.nightfall.ai/ai-security-101)
- [Web LLM attacks](https://portswigger.net/web-security/llm-attacks)
- [Microsoft AI Red Team](https://learn.microsoft.com/en-us/security/ai-red-team/)
- [AI Risk Assessment for ML Engineers](https://learn.microsoft.com/en-us/security/ai-red-team/ai-risk-assessment)
- [Microsoft - Generative AI Security for beginners](https://github.com/microsoft/generative-ai-for-beginners/blob/main/13-securing-ai-applications/README.md?WT.mc_id=academic-105485-koreyst)

#### AI Security Study Map

[![AI Security Study Map](https://i.postimg.cc/G2QdqnK6/map.png)](https://postimg.cc/sQvkg8tJ)

**[Полноразмерная карта с кликабельными ссылками](https://github.com/wearetyomsmnv/AI-LLM-ML_security_study_map)**

## Моделирование угроз

- [AI Villiage: LLM threat modeling](https://aivillage.org/large%20language%20models/threat-modeling-llm/)

- [JSOTIRO/ThreatModels](https://github.com/jsotiro/ThreatModels/tree/main)

![image](https://github.com/user-attachments/assets/367a50da-c93d-4c91-a69f-9a6de8d48f91)

![image](https://github.com/user-attachments/assets/eae84861-945b-4a2e-8037-f5ccfc92e5d0)

![image](https://github.com/user-attachments/assets/9f366c92-3e5a-4375-b967-ac35801151c1)

![image](https://github.com/user-attachments/assets/db78c3e7-8e41-4097-8f71-30b69eb70e55)

![image](https://github.com/user-attachments/assets/2cc30071-7ec2-4f09-bf80-29d6b1a008ba)


больше в книге **Adversarial AI Attacks, Mitigations, and Defense Strategies: A cybersecurity professional's guide to AI attacks, threat modeling, and securing AI with MLSecOps**


## Фреймворки по безопасности ML(Россия)
- [MlSecOps Process Framework](https://cyberorda.com/mlsecops_framework_pt/)
- [MlSecOps Framework: How to build the MLSecOps in IT-organization](https://github.com/d0ntbe/MLSecOps)

## Векторы атак

**Тут мы приводим полезный список ресурсов, которые посвящены конкретному вектору атаки.**

- [Data Poisoning](https://github.com/ch-shin/awesome-data-poisoning)
- [Adversarial Prompt Exploits](https://research.nccgroup.com/2022/12/05/exploring-prompt-injection-attacks)
- [Evasion Attack](https://blogs.rstudio.com/ai/posts/2020-05-15-model-inversion-attacks/)
- [Membership Inference Exploits](https://arxiv.org/abs/2103.07853)
  
![Классификация атак на модели машинного обучения](https://github.com/user-attachments/assets/434c0ee3-d8c9-44fe-a842-e31f8b51f2c7)

**[Полноразмерная классификация тут](https://t.me/purple_team_diary/35)**


## Блоги и публикации

**🌱 Сообщество в сфере ИИ-безопасности растёт. Появляются новые блоги и исследования. В этом разделе вы можете найти и ознакомиться с примерами блогов в даннойобласти, но это лишь малая часть, их намного больше.**

- 🛡️ [Red-Teaming Large Language Models](https://huggingface.co/blog/red-teaming)
- 🔍 [Google's AI red-team](https://blog.google/technology/safety-security/googles-ai-red-team-the-ethical-hackers-making-ai-safer/)
- 🔒 [The MLSecOps Top 10 vulnerabilities](https://ethical.institute/security.html)
- 🏴‍☠️ [Token Smuggling Jailbreak via Adversarial Prompt](https://www.piratewires.com/p/gpt4-token-smuggling)
- ☣️ [Just How Toxic is Data Poisoning? A Unified Benchmark for Backdoor and
Data Poisoning Attacks](https://arxiv.org/pdf/2006.12557.pdf)
- 📊 [We need a new way to measure AI security](https://blog.trailofbits.com/2023/03/14/ai-security-safety-audit-assurance-heidy-khlaaf-odd/)
- 🕵️ [PrivacyRaven: Implementing a proof of concept for model inversion](https://blog.trailofbits.com/2021/11/09/privacyraven-implementing-a-proof-of-concept-for-model-inversion/)
- 🧠 [Adversarial Prompts Engineering](https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/guides/prompts-adversarial.md)
- 🔫 [TextAttack: A Framework for Adversarial Attacks, Data Augmentation, and Adversarial Training in NLP](https://arxiv.org/abs/2005.05909)
- 📋 [Trail Of Bits' audit of Hugging Face's safetensors library](https://github.com/trailofbits/publications/blob/master/reviews/2023-03-eleutherai-huggingface-safetensors-securityreview.pdf)
- 🔝 [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/descriptions/)
- 🔐 [LLM Security](https://llmsecurity.net/)
- 🔑 [Is you MLOps infrastructure leaking secrets?](https://hackstery.com/2023/10/13/no-one-is-prefect-is-your-mlops-infrastructure-leaking-secrets/)
- 🚩 [Embrace The Red, blog where show how u can hack LLM's.](https://embracethered.com/)
- 🎙️ [Audio-jacking: Using generative AI to distort live audio transactions](https://securityintelligence.com/posts/using-generative-ai-distort-live-audio-transactions/)
- 🌐 [HADESS - Web LLM Attacks](https://hadess.io/web-llm-attacks/)
- 🧰 [WTF-blog - MlSecOps frameworks ... Which ones are available and what is the difference?](https://blog.wearetyomsmnv.wtf/articles/mlsecops-frameworks-...-which-ones-are-available-and-what-is-the-difference)
- 📚 [DreadNode Paper Stack](https://dreadnode.notion.site/2582fe5306274c60b85a5e37cf99da7e?v=74ab79ed1452441dab8a1fa02099fed)
- 


## Инфраструктурные уязвимости MLOps

**Очень интересные статьи по уязвимостям MlOps инфраструктуры. В некоторых можно найти даже готовые эксплоиты.**

- [SILENT SABOTAGE](https://hiddenlayer.com/research/silent-sabotage/) - Study on bot compromise for converting Pickle to SafeTensors
- [NOT SO CLEAR: HOW MLOPS SOLUTIONS CAN MUDDY THE WATERS OF YOUR SUPPLY CHAIN](https://hiddenlayer.com/research/not-so-clear-how-mlops-solutions-can-muddy-the-waters-of-your-supply-chain/) - Study on vulnerabilities for the ClearML platform
- [Uncovering Azure's Silent Threats: A Journey into Cloud Vulnerabilities](https://www.youtube.com/watch?v=tv8tei97Sv8) - Study on security issues of Azure MLAAS
- [The MLOps Security Landscape](https://hackstery.com/wp-content/uploads/2023/11/mlops_owasp_oslo_2023.pdf)
- [Confused Learning: Supply Chain Attacks through Machine Learning Models](https://blackhat.com/asia-24/briefings/schedule/#confused-learning-supply-chain-attacks-through-machine-learning-models-37794) 

## MlSecOps pipeline

![image](https://github.com/user-attachments/assets/8ce8400b-804b-4ce0-9241-30ad5b42b55f)



# Academic Po(C)ker FACE

## Репозитории

**Тут мы не стали переводить описания, так как могут возникнуть проблемы с пониманием.**

| PoC | Описание |
|------------|----------|
| [AgentPoison](https://github.com/BillChan226/AgentPoison)| Official implementation of "AgentPoison: Red-teaming LLM Agents via Memory or Knowledge Base Backdoor Poisoning". This project explores methods of data poisoning and backdoor insertion in LLM agents to assess their resilience against such attacks.|
| [DeepPayload](https://github.com/yuanchun-li/DeepPayload)| Research on methods of embedding malicious payloads into deep neural networks.|
| [backdoor](https://github.com/bolunwang/backdoor)| Investigation of backdoor attacks on deep learning models, focusing on creating undetectable vulnerabilities within models.|
| [Stealing_DL_Models](https://github.com/jeiks/Stealing_DL_Models)| Techniques for stealing deep learning models through various attack vectors, enabling adversaries to replicate or access models.|
| [datafree-model-extraction](https://github.com/cake-lab/datafree-model-extraction)| Model extraction without using data, allowing for the recovery of models without access to the original data.|
| [LLMmap](https://github.com/pasquini-dario/LLMmap)| Tool for mapping and analyzing large language models (LLMs), exploring the structure and behavior of various LLMs.|
| [GoogleCloud-Federated-ML-Pipeline](https://github.com/raj200501/GoogleCloud-Federated-ML-Pipeline)| Federated learning pipeline using Google Cloud infrastructure, enabling model training on distributed data.|
| [Class_Activation_Mapping_Ensemble_Attack](https://github.com/DreamyRainforest/Class_Activation_Mapping_Ensemble_Attack)| Attack using ensemble class activation maps to introduce errors in models by manipulating activation maps.|
| [COLD-Attack](https://github.com/Yu-Fangxu/COLD-Attack)| Methods for attacking deep models under various conditions and constraints, focusing on creating more resilient attacks.|
| [pal](https://github.com/chawins/pal)| Research on adaptive attacks on machine learning models, enabling the creation of attacks that can adapt to model defenses.|
| [ZeroShotKnowledgeTransfer](https://github.com/polo5/ZeroShotKnowledgeTransfer)| Knowledge transfer in zero-shot scenarios, exploring methods to transfer knowledge between models without prior training on target data.|
| [GMI-Attack](https://github.com/AI-secure/GMI-Attack)| Attack for generating informative labels, aimed at covertly extracting data from trained models.|
| [Knowledge-Enriched-DMI](https://github.com/SCccc21/Knowledge-Enriched-DMI)| Enhancing DMI (Data Mining and Integration) methods using additional knowledge to improve accuracy and efficiency.
| [vmi](https://github.com/wangkua1/vmi)| Research on methods for visualizing and interpreting machine learning models, providing insights into model workings.|
| [Plug-and-Play-Attacks](https://github.com/LukasStruppek/Plug-and-Play-Attacks)| Attacks that can be "plugged and played" without needing model modifications, offering flexible and universal attack methods.|
| [snap-sp23](https://github.com/johnmath/snap-sp23)| Tool for analyzing and processing snapshot data, enabling efficient handling of data snapshots.|
| [privacy-vs-robustness](https://github.com/inspire-group/privacy-vs-robustness)| Research on the trade-offs between privacy and robustness in models, aiming to balance these two aspects in machine learning.|
| [ML-Leaks](https://github.com/AhmedSalem2/ML-Leaks)| Methods for data leakage from trained models, exploring ways to extract private information from machine learning models.|
| [BlindMI](https://github.com/hyhmia/BlindMI)| Research on blind information extraction attacks, enabling data retrieval without access to the model's internal structure.|
| [python-DP-DL](https://github.com/NNToan-apcs/python-DP-DL)| Differential privacy methods for deep learning, ensuring data privacy during model training.|
| [MMD-mixup-Defense](https://github.com/colaalex111/MMD-mixup-Defense)| Defense methods using MMD-mixup, aimed at improving model robustness against attacks.|
| [MemGuard](https://github.com/jinyuan-jia/MemGuard)| Tools for protecting memory from attacks, exploring ways to prevent data leaks from model memory.|
| [unsplit](https://github.com/ege-erdogan/unsplit)| Methods for merging and splitting data to improve training, optimizing the use of heterogeneous data in models.|
| [face_attribute_attack](https://github.com/koushiksrivats/face_attribute_attack)| Attacks on face recognition models using attributes, exploring ways to manipulate facial attributes to induce errors.|
| [FVB](https://github.com/Sanjana-Sarda/FVB)| Attacks on face verification models, aimed at disrupting authentication systems based on face recognition.|
| [Malware-GAN](https://github.com/yanminglai/Malware-GAN)| Using GANs to create malware, exploring methods for generating malicious code with generative models.|
| [Generative_Adversarial_Perturbations](https://github.com/OmidPoursaeed/Generative_Adversarial_Perturbations)| Methods for generating adversarial perturbations using generative models, aimed at introducing errors in deep models.|
| [Adversarial-Attacks-with-Relativistic-AdvGAN](https://github.com/GiorgosKarantonis/Adversarial-Attacks-with-Relativistic-AdvGAN)| Adversarial attacks using Relativistic AdvGAN, exploring methods for creating more realistic and effective attacks.|
| [llm-attacks](https://github.com/llm-attacks/llm-attacks)| Attacks on large language models, exploring vulnerabilities and protection methods for LLMs.|
| [LLMs-Finetuning-Safety](https://github.com/LLM-Tuning-Safety/LLMs-Finetuning-Safety)| Safe fine-tuning of large language models, aiming to prevent data leaks and ensure security during LLM tuning.|
| [DecodingTrust](https://github.com/AI-secure/DecodingTrust)| Methods for evaluating trust in models, exploring ways to determine the reliability and safety of machine learning models.|
| [promptbench](https://github.com/microsoft/promptbench)| Benchmark for evaluating prompts, providing tools for testing and optimizing queries to large language models.|
| [rome](https://github.com/kmeng01/rome)| Tool for analyzing and evaluating models based on ROM codes, exploring various aspects of model performance and resilience.|
| [llmprivacy](https://github.com/eth-sri/llmprivacy)| Research on privacy in large language models, aiming to protect data and prevent leaks from LLMs.|

## Решения для защиты LLM

| Название | Возможности безопасности LLM | URL |
|----------|------------------------------|-----|
| CalypsoAI Moderator | Фокусируется на предотвращении утечки данных, полной возможности аудита и обнаружении вредоносного кода. | [https://calypsoai.com/](https://calypsoai.com/) |
| Giskard | Система управления качеством ИИ для ML-моделей, которая фокусируется на уязвимостях, таких как предвзятость производительности, галлюцинации и инъекции промптов. | (https://www.giskard.ai/)[https://www.giskard.ai/] |
| Lakera | Lakera Guard повышает безопасность приложений LLM и противодействует широкому спектру кибер-угроз ИИ. | [https://www.lakera.ai/](https://www.lakera.ai/) |
| Lasso Security | Фокусируется на LLM, предлагая оценку безопасности, продвинутое моделирование угроз и специализированные программы обучения. | [https://www.lasso.security/](https://www.lasso.security/) |
| LLM Guard | Разработан для укрепления безопасности LLM, предлагает санитизацию, обнаружение вредоносного языка, предотвращение утечки данных и устойчивость к инъекциям промптов. | [https://llm-guard.com](https://llm-guard.com) или [https://github.com/laiyerai/llm-guard](https://github.com/laiyerai/llm-guard) |
| LLM Fuzzer | Фреймворк с открытым исходным кодом для фаззинга, специально разработанный для LLM, который фокусируется на интеграции в приложения через API LLM. | [https://github.com/llmfuzzer](https://github.com/llmfuzzer) |
| Prompt Security | Предоставляет подход к обеспечению безопасности, конфиденциальности данных и безопасности во всех аспектах генеративного ИИ, не зависящий от конкретной LLM. | [https://prompt.security](https://prompt.security) |
| Rebuff | Самоукрепляющийся детектор инъекций промптов для AI-приложений, использующий многоуровневый механизм защиты. | [https://github.com/rebuff](https://github.com/rebuff) |
| Robust Intelligence | Предоставляет AI-файрвол и непрерывное тестирование и оценку. Создатели базы данных airisk.io пожертвовали это MITRE. | [https://www.robustintelligence.com/](https://www.robustintelligence.com/) |
| WhyLabs | Защищает LLM от угроз безопасности, фокусируясь на предотвращении утечки данных, мониторинге инъекций промптов и предотвращении дезинформации. | [https://www.whylabs.ai/](https://www.whylabs.ai/)

## Ресурсы сообщества

- [MLSecOps](https://mlsecops.com/)
- [MLSecOps Podcast](https://mlsecops.com/podcast)
- [MITRE ATLAS™](https://atlas.mitre.org/) and [SLACK COMMUNITY](https://join.slack.com/t/mitreatlas/shared_invite/zt-10i6ka9xw-~dc70mXWrlbN9dfFNKyyzQ)
- [MlSecOps comuntiy](https://mlsceops.com) and [SLACK COMMUNITY](https://mlsecops.slack.com/)
- [OWASP Machine Learning Security Top Ten](https://owasp.org/www-project-machine-learning-security-top-10/)
- [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [OWASP LLMSVS](https://owasp.org/www-project-llm-verification-standard/)
- [OWASP Periodic Table of AI Security](https://owaspai.org/goto/periodictable/)
- [OWASP SLACK](https://owasp.org/slack/invite)    
Следующие каналы:
    - #project-top10-for-llm
    - #ml-risk-top5
    - #project-ai-community
    - #project-mlsec-top10
    - #team-llm_ai-secgov
    - #team-llm-redteam
    - #team-llm-v2-brainstorm
    
- [Awesome LLM Security](https://github.com/corca-ai/awesome-llm-security)
- [Hackstery](https://hackstery.com/)
- [PWNAI](https://t.me/pwnai)
- [AiSec_X_Feed](https://t.me/aisecnews)
- [HUNTR Discord community](https://discord.com/invite/GBmmty82CM)
- [AIRSK](https://airisk.io)
- [AI Vulnerability Database](https://avidml.org/)
- [Incident AI Database](https://incidentdatabase.ai/)
- [Defcon AI Village CTF](https://www.kaggle.com/competitions/ai-village-ctf/overview)
- [Awesome AI Security](https://github.com/ottosulin/awesome-ai-security)
- [MLSecOps Reference Repository](https://github.com/disesdi/mlsecops_references)
- [Awesome LVLM Attack](https://github.com/liudaizong/Awesome-LVLM-Attack)
- [Awesome MLLM Safety](https://github.com/isXinLiu/Awesome-MLLM-Safety)
- [Телеграм папка](https://t.me/addlist/40D9BRf6rDoxNzg6)


## Книги и курсы

- [Protect AI: Introduction to mlsecops](https://www.linkedin.com/learning/introduction-to-mlsecops)
- [Adversarial AI Attacks, Mitigations, and Defense Strategies: A cybersecurity professional's guide to AI attacks, threat modeling, and securing AI with MLSecOps](https://www.amazon.com/Adversarial-Attacks-Mitigations-Defense-Strategies/dp/1835087981)
- [Privacy-Preserving Machine Learning](https://www.ebooks.com/en-cg/book/211334202/privacy-preserving-machine-learning/srinivasa-rao-aravilli/)
- [Generative AI Security: Theories and Practices (Future of Business and Finance) ](https://www.amazon.com/Generative-AI-Security-Theories-Practices/dp/3031542517)
- [Lakera: Introduction to AI Security (10 days email course)](https://www.lakera.ai/ai-security-guides/introduction-to-ai-security)
- [The Developer's Playbook for Large Language Model Security](https://www.amazon.com/Developers-Playbook-Large-Language-Security/dp/109816220X)


## Инфографики

### MLSecOps Lifecycle
[![MLSecOps Lifecycle](https://github.com/RiccardoBiosas/awesome-MLSecOps/assets/65150720/236cd3f4-bce8-4659-b43f-8d4002df65a5)](https://www.conf42.com/DevSecOps_2022_Eugene_Neelou_ai_introducing_mlsecops_for_software_20)

### AI Security Market Map
![image](https://github.com/user-attachments/assets/c929bab0-ece4-43cc-b63b-a0b2c387b633)

## Законодательство и постановления


| Страна | Название документа | Краткое описание | Основные направления | Ссылка |
|--------|---------------------|-------------------|----------------------|--------|
| Россия | ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ. ТЕХНИЧЕСКАЯ СТРУКТУРА ФЕДЕРАТИВНОЙ СИСТЕМЫ МАШИННОГО ОБУЧЕНИЯ | | | [Ссылка](https://protect.gost.ru/v.aspx?control=8&baseC=6&page=0&month=12&year=-1&search=&RegNum=1&DocOnPageCount=15&id=245476) |
| Россия | ПНСТ 848-2023 Искусственный интеллект. Большие данные. Обзор и требования по обеспечению сохранности данных. | | | [Ссылка](https://docs.cntd.ru/document/1304365959) |
| Россия | ПНСТ 847-2023 Искусственный интеллект. Большие данные. Функциональные требования в отношении происхождения данных | | | [Ссылка](https://protect.gost.ru/document1.aspx?control=31&baseC=6&page=2&month=9&year=-1&search=&id=256915) |
| Россия | Оценка качества систем искусственного интеллекта. Общие положения. ГОСТ Р 59898-2021 | | | |
| Россия | Информационные технологии. Интеллект искусственный. Оценка робастности нейронных сетей. Часть 1. Обзор. ГОСТ Р 70462.1-2022/ISO/IEC TR 24029-1-2021 | | | |
| Россия | Системы искусственного интеллекта. Способы обеспечения доверия. Общие положения. ГОСТ Р 59276-2020 | | | |
| США | Biden's AI executive order | Указ устанавливает новые стандарты безопасности ИИ, требуя от разработчиков мощных систем делиться результатами испытаний с правительством. | Министру торговли поручено разработать руководство и лучшие практики по безопасности ИИ в течение 270 дней. Подчеркивается важность безопасности и беспристрастности систем ИИ для национальной обороны и критической инфраструктуры. | [Ссылка](https://www.whitehouse.gov/briefing-room/statements-releases/2023/10/30/fact-sheet-president-biden-issues-executive-order-on-safe-secure-and-trustworthy-artificial-intelligence/) |
| США | FTC: Keep your AI claims in check | | | [Ссылка](https://www.ftc.gov/business-guidance/blog/2023/02/keep-your-ai-claims-check) |
| США | FAA - Unmanned Aircraft Vehicles | | | [Ссылка](https://www.faa.gov/regulations_policies/rulemaking/committees/documents/index.cfm/committee/browse/committeeID/837) |
| США | NHTSA - Automated Vehicle safety | | | [Ссылка](https://www.nhtsa.gov/vehicle-safety/automated-vehicles-safety) |
| США | AI Bill of Rights | | | [Ссылка](https://www.whitehouse.gov/ostp/ai-bill-of-rights/) |
| Япония | Relaxing copyright for AI training | Economic growth takes priority over regulation | | [Ссылка](https://www.privacyworld.blog/2024/03/japans-new-draft-guidelines-on-ai-and-copyright-is-it-really-ok-to-train-ai-using-pirated-materials/) |
| Великобритания | AI white paper | Principle-based approach, decentralized governance | | [Ссылка](https://commission.europa.eu/system/files/2020-02/commission-white-paper-artificial-intelligence-feb2020_en.pdf) |
| Китай | Rules for GenAI services | Extraterritorial scope, content monitoring | | [Ссылка](https://www.insideglobaltech.com/2023/08/30/labeling-of-ai-generated-content-new-guidelines-released-in-china/) |
| Сингапур | Voluntary AI Verify system | Self-assessment against principles, global alignment | | |
| Австралия | AI ethics framework | Voluntary principles, considering stricter laws | | [Ссылка](https://ethics-of-ai.mooc.fi/chapter-1/4-a-framework-for-ai-ethics/) |
| Евросоюз | AI Act | Risk-based framework, banned uses, standards for high-risk AI | | [Ссылка](https://artificialintelligenceact.eu/) |
| Международный | ISO/IEC 42001 Artificial intelligence — Management system | | | [Ссылка](https://www.iso.org/standard/81230.html) |
| Международный | ISO/IEC 22989 — Artificial intelligence — Concepts and terminology | | | [Ссылка](https://www.iso.org/standard/74296.html) |
| Международный | ISO/IEC 38507 — Governance of IT — Governance implications of the use of artificial intelligence by organizations | | | [Ссылка](https://www.iso.org/standard/56641.html) |
| Международный | ISO/IEC 23894 — Artificial Intelligence — Guidance on Risk Management | | | [Ссылка](https://www.iso.org/standard/77304.html) |
| Международный | ANSI/UL 4600 Standard for Safety for the Evaluation of Autonomous Products | Addresses fully autonomous systems that move such as self-driving cars, and other vehicles including lightweight unmanned aerial vehicles (UAVs). | Includes safety case construction, risk analysis, design process, verification and validation, tool qualification, data integrity, human-machine interaction, metrics and conformance assessment. | [Ссылка](https://users.ece.cmu.edu/~koopman/ul4600/index.html) |




