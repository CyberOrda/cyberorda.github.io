---
hide:
  - feedback
tags:
  - ML
  - MlOps
  - Ml security
---
# **MlSecOps**

[![mm.png](https://i.postimg.cc/VL6C6tKF/mm.png)](https://postimg.cc/SjBs1nFX)

## **Open Source инструменты**

- [ModelScan](https://github.com/protectai/modelscan) - защита от атак на сериализацию ML-моделей.
- [NB Defense](https://nbdefense.ai) - Безопасные Jupyter Notebooks.
- [Garak](https://github.com/leondz/garak) - сканер уязвимостей LLM.
- [Adversarial Robustness Toolbox](https://github.com/IBM/adversarial-robustness-toolbox) - Библиотека методов защиты моделей машинного обучения от adversarial-атак.
- [MLSploit](https://github.com/mlsploit/) - MLsploit - облачный фреймворк для проведения интерактивных экспериментов с исследованиями в области адверсивного машинного обучения.
- [TensorFlow Privacy](https://github.com/tensorflow/privacy) - Библиотека алгоритмов и инструментов машинного обучения с защитой конфиденциальности.
- [Foolbox](https://github.com/bethgelab/foolbox) - инструментарий на языке Python для создания и оценки adversarial-атак и защитных средств.
- [Advertorch](https://github.com/BorealisAI/advertorch) - Инструментарий на Python для исследования стойкости атак. 
- [Artificial Intelligence Threat Matrix](https://collaborativeaicontrols.github.io/ATM/) - фреймворк для выявления и смягчения угроз для систем машинного обучения.
- [Adversarial ML Threat Matrix](https://github.com/mitre/advmlthreatmatrix) - Ландшафт угроз для систем искусственного интеллекта.
- [CleverHans](https://github.com/cleverhans-lab/cleverhans) - Библиотека adversarial примеров и средств защиты для моделей машинного обучения.
- [AdvBox](https://github.com/advboxes/AdvBox) - Advbox - это набор инструментов для создания adversarial примеров, которые обманывают нейронные сети в PaddlePaddle、PyTorch、Caffe2、MxNet、Keras、TensorFlow.
- [Audit AI](https://github.com/pymetrics/audit-ai) - Тестирование на предвзятость для машинного обучения.
- [Deep Pwning](https://github.com/cchio/deep-pwning) - Deep-pwning - это легкий фреймворк для экспериментов с моделями машинного обучения с целью оценки их устойчивости против мотивированного противника. 
- [Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) - Библиотека с открытым исходным кодом для аудита конфиденциальности данных в статистических алгоритмах и алгоритмах машинного обучения.
- [TensorFlow Model Analysis](https://github.com/tensorflow/model-analysis) - библиотека для анализа, проверки и мониторинга моделей машинного обучения в производстве.
- [PromptInject](https://github.com/agencyenterprise/PromptInject) - фреймворк, позволяющий компоновать агрессивные подсказки.
- [TextAttack](https://github.com/QData/TextAttack) - TextAttack - это фреймворк на Python для adversarial attacks, дополнения данных и обучения моделей в NLP.
- [OpenAttack](https://github.com/thunlp/OpenAttack) - Пакет с открытым исходным кодом для текстовых атак.
- [TextFooler](https://github.com/jind11/TextFooler) - Модель для атак на естественный язык для классификации и вывода текста.
- [Flawed Machine Learning Security](https://github.com/EthicalML/fml-security) - Практические примеры "Flawed Machine Learning Security" вместе с лучшими практиками ML Security на всех этапах жизненного цикла моделей машинного обучения - от обучения, упаковки до развертывания.
- [Adversarial Machine Learning CTF](https://github.com/arturmiller/adversarial_ml_ctf) - Это хранилище представляет собой CTF-задачу, демонстрирующую недостаток безопасности в большинстве (всех?) распространенных искусственных нейронных сетей. Они уязвимы для неблагоприятных изображений.
- [Damn Vulnerable LLM Project](https://github.com/harishsg993010/DamnVulnerableLLMProject) - Большая языковая модель, предназначенная для взлома.
- [Gandalf Lakera](https://gandalf.lakera.ai/) - CTF-игра Prompt Injection
- [Vigil](https://github.com/deadbits/vigil-llm) - LLM prompt injection и сканер безопасности.
- [PALLMs (Payloads for Attacking Large Language Models)](https://github.com/mik0w/pallms) - список различных полезных нагрузок для атак на LLM, собранных в одном месте
- [AI-exploits](https://github.com/protectai/ai-exploits) - эксплойты для MlOps-систем. 
- [Offensive ML Playbook](https://wiki.offsecml.com/Welcome+to+the+Offensive+ML+Playbook) - Offensive ML Playbook. Заметки об атаках на машинное обучение и пентестинге.
- [AnonLLM](https://github.com/fsndzomga/anonLLM) - анонимизация персонально идентифицируемой информации (PII) для API больших языковых моделей.
- [AI Goat](https://github.com/dhammon/ai-goat) - уязвимые задачи LLM CTF.
- [Pyrit](https://github.com/Azure/PyRIT) - инструмент идентификации рисков на Python для генеративного ИИ.
- [Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors](https://github.com/advmlphish/raze_to_the_ground_aisec23) - исходный код статьи "Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors", принятый на AISec '23

## **Безопасное написание кода для модели машинного обучения**

- [lintML](https://github.com/JosephTLucas/lintML) - линтер безопасности для ML, от Nvidia
- [HiddenLayer: Model as Code](https://hiddenlayer.com/research/models-are-code/) - исследование о некоторых векторах в библиотеках ml.
- [Copycat CNN](https://github.com/jeiks/Stealing_DL_Models) - доказательство того, как создать копию конволюционной нейронной сети, запросив ее как "черный ящик" со случайными данными, и использовать полученные результаты для обучения копии CNN, которая имитирует предсказательные паттерны целевой CNN.

## **101**

- [AI Security 101](https://www.nightfall.ai/ai-security-101)
- [Web LLM attacks](https://portswigger.net/web-security/llm-attacks)
- [Microsoft AI Red Team](https://learn.microsoft.com/en-us/security/ai-red-team/)
- [AI Risk Assessment for ML Engineers](https://learn.microsoft.com/en-us/security/ai-red-team/ai-risk-assessment)

## **Вектора атак**

- [Data Poisoning](https://github.com/ch-shin/awesome-data-poisoning)
- [Adversarial Prompt Exploits](https://research.nccgroup.com/2022/12/05/exploring-prompt-injection-attacks)
- [Evasion Attack](https://blogs.rstudio.com/ai/posts/2020-05-15-model-inversion-attacks/)
- [Membership Inference Exploits](https://arxiv.org/abs/2103.07853)

## **Блоги и публикации**

- [Red-Teaming Large Language Models](https://huggingface.co/blog/red-teaming)
- [Google's AI red-team](https://blog.google/technology/safety-security/googles-ai-red-team-the-ethical-hackers-making-ai-safer/)
- [The MLSecOps Top 10 vulnerabilities](https://ethical.institute/security.html)
- [Token Smuggling Jailbreak via Adversarial Prompt](https://www.piratewires.com/p/gpt4-token-smuggling)
- [Just How Toxic is Data Poisoning? A Unified Benchmark for Backdoor and
Data Poisoning Attacks](https://arxiv.org/pdf/2006.12557.pdf)
- [We need a new way to measure AI security](https://blog.trailofbits.com/2023/03/14/ai-security-safety-audit-assurance-heidy-khlaaf-odd/)
- [PrivacyRaven: Implementing a proof of concept for model inversion](https://blog.trailofbits.com/2021/11/09/privacyraven-implementing-a-proof-of-concept-for-model-inversion/)
- [Adversarial Prompts Engineering](https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/guides/prompts-adversarial.md)
- [TextAttack: A Framework for Adversarial Attacks, Data Augmentation, and Adversarial Training in NLP](https://arxiv.org/abs/2005.05909)
- [Trail Of Bits' audit of Hugging Face's safetensors library](https://github.com/trailofbits/publications/blob/master/reviews/2023-03-eleutherai-huggingface-safetensors-securityreview.pdf)
- [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/descriptions/)
- [LLM Security](https://llmsecurity.net/)
- [Is you MLOps infrastructure leaking secrets?](https://hackstery.com/2023/10/13/no-one-is-prefect-is-your-mlops-infrastructure-leaking-secrets/)
- [Embrace The Red, blog where show how u can hack LLM's.](https://embracethered.com/)
- [Audio-jacking: Using generative AI to distort live audio transactions](https://securityintelligence.com/posts/using-generative-ai-distort-live-audio-transactions/)
- [HADESS - Web LLM Attacks](https://hadess.io/web-llm-attacks/)

## **Инфраструктурные уязвимости MLOPS**

- [SILENT SABOTAGE](https://hiddenlayer.com/research/silent-sabotage/) - A study on bot compromise for converting Pickle to SafeTensors.
- [NOT SO CLEAR: HOW MLOPS SOLUTIONS CAN MUDDY THE WATERS OF YOUR SUPPLY CHAIN](https://hiddenlayer.com/research/not-so-clear-how-mlops-solutions-can-muddy-the-waters-of-your-supply-chain/) - This study examines vulnerabilities for the ClearML platform.
- [Uncovering Azure's Silent Threats: A Journey into Cloud Vulnerabilities](https://www.youtube.com/watch?v=tv8tei97Sv8) - This study shows the security issues of Azure MLAAS(Machine Learning As A Service).
- [The MlOps Security Landscape](https://hackstery.com/wp-content/uploads/2023/11/mlops_owasp_oslo_2023.pdf)
- [Confused Learning: Supply Chain Attacks through Machine Learning Models](https://blackhat.com/asia-24/briefings/schedule/#confused-learning-supply-chain-attacks-through-machine-learning-models-37794) - Released in April 2024.
- [Большой куш: баги в MLOps и моделях машинного обучения, которые приводят к тем самым последствиям](https://safecodeconf.ru/talks/4ca452e0bdd046b4a1df9ea70a55917d/?referer=/persons/673b871e46c34811866ee6a1c29756d0/)

## **Другие ресурсы, которые были опубликованы и разработаны сообществом.**

- [MLSecOps](https://mlsecops.com/)
- [MLSecOps Podcast](https://mlsecops.com/podcast)
- [MITRE ATLAS™ (Adversarial Threat Landscape for Artificial-Intelligence Systems)](https://atlas.mitre.org/)
- [OWASP Machine Learning Security Top Ten](https://owasp.org/www-project-machine-learning-security-top-10/)
- [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [Awesome LLM Security](https://github.com/corca-ai/awesome-llm-security)
- [Hackstery](https://hackstery.com/)
- [PWNAI](https://t.me/pwnai)
- [AiSec_X_Feed](https://t.me/aisecnews)
- [HUNTR Discord community](https://discord.com/invite/GBmmty82CM)
- [AIRSK](https://airisk.io)
- [AI Vulnerability Database](https://avidml.org/)
- [Incident AI Database](https://incidentdatabase.ai/)
- [Defcon AI Villiage CTF](https://www.kaggle.com/competitions/ai-village-ctf/overview)
- [Awesome AI Security](https://github.com/ottosulin/awesome-ai-security)
- [MLSecOps Reference Repository](https://github.com/disesdi/mlsecops_references)

## **Инфографики**

### **MlSecOps жизненный цикл**

[![MLSecOps_Lifecycle](https://github.com/RiccardoBiosas/awesome-MLSecOps/assets/65150720/236cd3f4-bce8-4659-b43f-8d4002df65a5)](https://www.conf42.com/DevSecOps_2022_Eugene_Neelou_ai_introducing_mlsecops_for_software_20)


### **Ai Security карта рынка**

[![Market Map](https://i.postimg.cc/15ZxH0q9/marketmap.png)](https://menlovc.com/perspective/security-for-ai-genai-risks-and-the-emerging-startup-landscape/)


