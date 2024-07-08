---
hide:
  - feedback
tags:
  - ML
  - MlOps
  - Ml security
---
# **Впечатляющий MlSecOps**

Курируемый на русском языке список ресурсов, которые относятся к MlSecOps(ну и немножко про атаки на AI).

[![mm.png](img/mm.png)](img/mm.png)

## Содержание
- [Инструменты с открытым исходным кодом](#инструменты-с-открытым-исходным-кодом)
- [Защита кода моделей](#защита-кода-моделей)
- [101](#101)
- [Векторы атак](#векторы-атак)
- [Блоги и публикации](#блоги-и-публикации)
- [Уязвимости MlOps инфраструктуры](#уязвимости-mlops-инфраструктуры)
- [Ресурсы сообщества](#ресурсы-сообщества)
- [Инфографики](#инфографики)


## Инструменты с открытым исходным кодом

В этом разделе мы с вами можем рассмотреть, какие opensource решения и PoC, существуют для выполнения задачи по защите ML. Конечно, некоторые из них являются не поддерживаемыми или будут возникать трудности с запуском. Однако, не сказать о них - большое преступление.


- [ModelScan](https://github.com/protectai/modelscan) - Защита от атак на сериализацию ML-моделей.
- [NB Defense](https://nbdefense.ai) - решение для защиты Jupyter Notebook.
- [Garak](https://github.com/leondz/garak) -  сканер уязвимостей для LLM.
- [Adversarial Robustness Toolbox](https://github.com/IBM/adversarial-robustness-toolbox) - Библиотека методов защиты моделей машинного обучения от adversarial атак.
- [MLSploit](https://github.com/mlsploit/) - MLsploit - это облачный фреймворк для интерактивных экспериментов по изучению adversarial machine learning.
- [TensorFlow Privacy](https://github.com/tensorflow/privacy) - Библиотека алгоритмов и инструментов машинного обучения с защитой конфиденциальности.
- [Foolbox](https://github.com/bethgelab/foolbox) - Инструментарий на языке Python для создания adversarial атак и оценки атак и защиты.
- [Advertorch](https://github.com/BorealisAI/advertorch) - Инструмент на python для генерации adversarial атак.
- [Artificial Intelligence Threat Matrix](https://collaborativeaicontrols.github.io/ATM/) - Фреймворк для идеентификации и смягчения угроз для систем машинного обучения.
- [Adversarial ML Threat Matrix](https://github.com/mitre/advmlthreatmatrix) - Ландшафт adversarial угроз для систем использующих ИИ.
- [CleverHans](https://github.com/cleverhans-lab/cleverhans) - библиотека для генерации adversarial атак а также защиты от них.
- [AdvBox](https://github.com/advboxes/AdvBox) - Advbox это инструмент для генерации Adversarial атак, которые работают на нейросетях, которые были реализованы при помощи PaddlePaddle, PyTorch, Caffe2, MxNet, Keras и TensorFlow.
- [Audit AI](https://github.com/pymetrics/audit-ai) - Тестирование на предвзятость для  приложений машинного обучения.
- [Deep Pwning](https://github.com/cchio/deep-pwning) - Deep-pwning - это легкий фреймворк для экспериментов с моделями машинного обучения с целью оценки их устойчивости против мотивированного противника. 
- [Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) - Библиотека с открытым исходным кодом для проверки конфиденциальности данных в статистических алгоритмах и алгоритмах машинного обучения.
- [TensorFlow Model Analysis](https://github.com/tensorflow/model-analysis) - Библиотека для анализа, проверки и мониторинга моделей машинного обучения в производстве.
- [PromptInject](https://github.com/agencyenterprise/PromptInject) - Фреймворк для реализации атак типа Prompt Injection, содержащий в себе множество adversarial подсказок.
- [TextAttack](https://github.com/QData/TextAttack) - Фреймворк для Adversarial Атак, Data Augmentation, и Adversarial обучения в NLP(ссылка на исходники).
- [OpenAttack](https://github.com/thunlp/OpenAttack) - Opensource решение для Текстовых Adversarial Атак.
- [TextFooler](https://github.com/jind11/TextFooler) - Модель для реализации атак в NLP на текстовые классифкаторы и вывод.
- [Flawed Machine Learning Security](https://github.com/EthicalML/fml-security) - примеры "дефектов безопасности машинного обучения", а также передовые методы обеспечения безопасности ML на всех этапах жизненного цикла моделей машинного обучения - от обучения, упаковки до развертывания.
- [Adversarial Machine Learning CTF](https://github.com/arturmiller/adversarial_ml_ctf) - Этот репозиторий - CTF-челлендж, в котором вам предстоит эксплуатировать недостатки распространённых ИИ. В основном это атаки связанные с плохой классификацией изображений.
- [Damn Vulnerable LLM Project](https://github.com/harishsg993010/DamnVulnerableLLMProject) - Большая языковая модель, предназначенная для взлома
- [Gandalf Lakera](https://gandalf.lakera.ai/) - Prompt Injection CTF 
- [Vigil](https://github.com/deadbits/vigil-llm) - сканер на наличие уязвимости prompt injection.
- [PALLMs (Payloads for Attacking Large Language Models)](https://github.com/mik0w/pallms) - список различных Payloads для атак на LLM, в одном месте.
- [AI-exploits](https://github.com/protectai/ai-exploits) - эксплоиты для MlOps инфраструктуры.
- [Offensive ML Playbook](https://wiki.offsecml.com/Welcome+to+the+Offensive+ML+Playbook) - Offensive ML Playbook. Заметки по атакам на машинное обучение и тестированию на проникновение(AI).
- [AI Goat](https://github.com/dhammon/ai-goat) - CTF с уязвимой LLM.
- [Pyrit](https://github.com/Azure/PyRIT) - Инструмент, выпущенный microsoft для оценки рисков Generative AI.
- [Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors](https://github.com/advmlphish/raze_to_the_ground_aisec23) - Исходный код для статьи "Raze to the Ground: Query-Efficient Adversarial HTML Attacks on Machine-Learning Phishing Webpage Detectors" представленной на AISec '23
- [Giskard](https://github.com/Giskard-AI/giskard) - Инструмент с открытым исходным кодом для тестирования LLM в приложениях. 
- [Safetensors](https://github.com/huggingface/safetensors) - Преобразование pickle в безопасный вариант сериализации.
- [Citadel Lens](https://www.citadel.co.jp/en/products/lens/)- Проверка качества моделей в соответствии с отраслевыми стандартами.
- [Model-Inversion-Attack-ToolBox](https://github.com/ffhibnese/Model-Inversion-Attack-ToolBox) - Фреймворк для реализации атак с инверсией модели.
- [NeMo-Guardials](https://github.com/NVIDIA/NeMo-Guardrails) - NeMo Guardrails позволяет разработчикам, создающим приложения на базе LLM, легко добавлять программируемые ограждения между кодом приложения и LLM.
- [AugLy](https://github.com/facebookresearch/AugLy) - Инструмент для создания Adversarial атак.
- [Knockoffnets](https://github.com/tribhuvanesh/knockoffnets) - PoC для реализации атак BlackBox с целью кражи данных модели.
- [Robust Intelligence Continous Validation](https://www.robustintelligence.com/platform/continuous-validation) - Инструмент для непрерывной проверки моделей на соответствие стандартам.
- [VGER](https://github.com/JosephTLucas/vger) - Фреймворк для атаки на Jupyter Notebook 
- [AIShield Watchtower](https://github.com/bosch-aisecurity-aishield/watchtower) - Инструмент с открытым исходным кодом от AIShield для изучения моделей искусственного интеллекта и сканирования их на наличие уязвимостей.
- [PS-fuzz](https://github.com/prompt-security/ps-fuzz) - инструмент для сканирования уязвимостей на LLM, однако он поддерживает в т.ч Российские LLM (GigaChat, YaGPT).
- [Mindgard-cli](https://github.com/Mindgard/cli/) - Проверьте безопасность вашей модели ИИ через CLI.

## Коммерческие решения
- [Databricks Platform, Azure Databricks](https://azure.microsoft.com/ru-ru/products/databricks) - Инструмент для управления данными.
- [Hidden Layer AI Detection Response](https://hiddenlayer.com/aidr/) - Инструмент для обнаружения и реагирования на инциденты.
- [Guardian](https://protectai.com/guardian) - Защита моделей в CI/CD.

## Данные
- [ARX -Data Anonymization Tool](https://arx.deidentifier.org/) - Инструмент для анонимизации датасетов.
- [Data-Veil](https://veil.ai/) - Инструмент для маскирования и анонимизации данных.

## Защита кода моделей
- [lintML](https://github.com/JosephTLucas/lintML) - линтер кода с sast-паттернами для моделей машинного обучения, by Nvidia
- [HiddenLayer: Model as Code](https://hiddenlayer.com/research/models-are-code/) - research about some vectors in ml libraries.
- [Copycat CNN](https://github.com/jeiks/Stealing_DL_Models) - proof-of-concept для создания копии конволюционной нейронной сети путем black-box запроса к ней со случайными данными и использования полученных результатов для обучения подражательной CNN, которая имитирует предсказательные шаблоны целевой CNN.
- [differential-privacy-library](https://github.com/IBM/differential-privacy-library) - Это библиотека, предназначенная для дифференциальной конфиденциальности и машинного обучения. Ее цель - позволить экспериментировать, моделировать и реализовывать модели с свойством дифференциальной приватности.
- 

## 101

Вы можете найти тут перечень ресурсов, которые помогут войти в тему безопасности ИИ. Разобраться с тем, какие атаки существуют и как они могут быть использованы злоумышленником.

- [AI Security 101](https://www.nightfall.ai/ai-security-101)
- [Web LLM attacks](https://portswigger.net/web-security/llm-attacks)
- [Microsoft AI Red Team](https://learn.microsoft.com/en-us/security/ai-red-team/)
- [AI Risk Assessment for ML Engineers](https://learn.microsoft.com/en-us/security/ai-red-team/ai-risk-assessment)

Ты хочешь изучить безопасность ИИ? Но незнаешь с чего начать? Загляни в эту карту...

[![map.png](https://i.postimg.cc/G2QdqnK6/map.png)](https://postimg.cc/sQvkg8tJ)

полноразмерная картинка в этом репозитории:
- [AI-LLM-ML_security_study_map](https://github.com/wearetyomsmnv/AI-LLM-ML_security_study_map) - LLM/AI/Security study map.

## Векторы атак

Тут мы приводим полезный список ресурсов, которые посвящены конкретному вектору атаки. 

- [Data Poisoning](https://github.com/ch-shin/awesome-data-poisoning)
- [Adversarial Prompt Exploits](https://research.nccgroup.com/2022/12/05/exploring-prompt-injection-attacks)
- [Evasion Attack](https://blogs.rstudio.com/ai/posts/2020-05-15-model-inversion-attacks/)
- [Membership Inference Exploits](https://arxiv.org/abs/2103.07853)

## Блоги и публикации

Сообщество в сфере ИИ-безопасности - растёт. Появляются новые блоги и множество исследователей. В этом пункте вы можете увидеть примеры некоторых блогов.


- [Рэд тиминг больших языковых моделей](https://huggingface.co/blog/red-teaming)
- [Google's AI red-team](https://blog.google/technology/safety-security/googles-ai-red-team-the-ethical-hackers-making-ai-safer/)
- [Топ-10 уязвимостей MLSecOps](https://ethical.institute/security.html)
- [Token Smuggling Jailbreak с использованием adversarial-промпта](https://www.piratewires.com/p/gpt4-token-smuggling)
- [Насколько токсичны данные? Единый бенчмарк для атак с использованием бэкдоров и отравления данных](https://arxiv.org/pdf/2006.12557.pdf)
- [Нам нужен новый способ оценки безопасности ИИ](https://blog.trailofbits.com/2023/03/14/ai-security-safety-audit-assurance-heidy-khlaaf-odd/)
- [PrivacyRaven: Реализация PoC для атаки типа model inversion](https://blog.trailofbits.com/2021/11/09/privacyraven-implementing-a-proof-of-concept-for-model-inversion/)
- [Adversarial Prompts Engineering](https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/guides/prompts-adversarial.md)
- [TextAttack: Фреймворк для Adversarial Атак, Data Augmentation, и Adversarial обучения в NLP](https://arxiv.org/abs/2005.05909)
- [Trail of Bits: отчёт об аудите безопасности библиотеки safetensors(Hugging Face)](https://github.com/trailofbits/publications/blob/master/reviews/2023-03-eleutherai-huggingface-safetensors-securityreview.pdf)
- [OWASP Top 10 для приложений, использующих большие языковые модели](https://owasp.org/www-project-top-10-for-large-language-model-applications/descriptions/)
- [LLM Security](https://llmsecurity.net/)
- [Утечка секретов в вашей инфраструктуре MLOps?](https://hackstery.com/2023/10/13/no-one-is-prefect-is-your-mlops-infrastructure-leaking-secrets/)
- [Embrace The Red - блог, в котором рассказывается о том, как можно взломать LLM.](https://embracethered.com/)
- [Audio-jacking: Using generative AI to distort live audio transactions](https://securityintelligence.com/posts/using-generative-ai-distort-live-audio-transactions/)
- [HADESS - Атаки на LLM в веб-приложениях.](https://hadess.io/web-llm-attacks/)
- [WTF-blog - Фреймворки MlSecOps ... Какие из них существуют и в чем разница?](https://blog.wearetyomsmnv.wtf/articles/mlsecops-frameworks-...-which-ones-are-available-and-what-is-the-difference)

## MlOps infrastracture vulnerabilities

Очень интересные статьи по уязвимостям MlOps инфраструктуры. В некоторых можно найти даже готовые эксплоиты.

- [SILENT SABOTAGE](https://hiddenlayer.com/research/silent-sabotage/) - Статья о компроментации бота Safetensors(huggingface) при помощи pickles.
- [NOT SO CLEAR: HOW MLOPS SOLUTIONS CAN MUDDY THE WATERS OF YOUR SUPPLY CHAIN](https://hiddenlayer.com/research/not-so-clear-how-mlops-solutions-can-muddy-the-waters-of-your-supply-chain/) - Эта статья рассказывает об уязвимостях, которые были найдены в ClearML.
- [Uncovering Azure's Silent Threats: A Journey into Cloud Vulnerabilities](https://www.youtube.com/watch?v=tv8tei97Sv8) - этот доклад демонстрирует недостатки защищённости MlaaS(Machine Learning As A Service) в Azure.
- [The MlOps Security Landscape](https://hackstery.com/wp-content/uploads/2023/11/mlops_owasp_oslo_2023.pdf)
- [Confused Learning: Supply Chain Attacks through Machine Learning Models](https://blackhat.com/asia-24/briefings/schedule/#confused-learning-supply-chain-attacks-through-machine-learning-models-37794) - Доклад рассматривающий атаки на цепочку поставок в MlOps, через вектор в keras.


## Ресурсы сообщества

Ещё парочку ссылок, на ресурсы, которые создаёт сообщество.

- [MLSecOps](https://mlsecops.com/)
- [MLSecOps Podcast](https://mlsecops.com/podcast)
- [MITRE ATLAS™ (Adversarial Threat Landscape for Artificial-Intelligence Systems)](https://atlas.mitre.org/)
- [OWASP Machine Learning Security Top Ten](https://owasp.org/www-project-machine-learning-security-top-10/)
- [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [OWASP LLMSVS](https://owasp.org/www-project-llm-verification-standard/)
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


## Инфографики

### MlSecOps жизненный цикл
[![MLSecOps_Lifecycle](https://github.com/RiccardoBiosas/awesome-MLSecOps/assets/65150720/236cd3f4-bce8-4659-b43f-8d4002df65a5)](https://www.conf42.com/DevSecOps_2022_Eugene_Neelou_ai_introducing_mlsecops_for_software_20)

### Карты рынка безопасности ИИ
[![Market Map](img/marketmap.png)](img/marketmap.png)
<img width="1024" alt="image_2024-04-18_18-15-29" src="https://github.com/wearetyomsmnv/awesome-MLSecOps/assets/129667548/bb29607b-1396-4653-a8e3-475bdd0b9dd1">
