---
hide:
  - feedback
tags:
  - DevSecOps
  - Tools
---

# **DevSecOps**

## **Обучение**

- [DevSecOps-Studio](https://github.com/teacheraio/DevSecOps-Studio): DevSecOps Distribution - виртуальная среда для изучения DevSecOps

## **Инструменты**

### **Управление уязвимостями**

- [DefectDojo](https://github.com/DefectDojo/django-DefectDojo): DefectDojo - это инструмент корреляции уязвимостей приложений и оркестровки безопасности с открытым исходным кодом.
- [Whitespots portal](https://gitlab.com/whitespots-public/appsec-portal): Whitespots portal - Комерческая система для поиска и управления уязвимостями с функцией создания правил для валидации и скоринга уязвимостей, а также дедупликации уязвимостей пришедших от разных сканеров. Одним из компонентов платформы является своя [CI система](https://gitlab.com/whitespots-public/auditor), на базе которой осуществляется запуск сканеров.
- [DependencyTrack](https://github.com/DependencyTrack/dependency-track): Dependency-Track - это интеллектуальная платформа анализа состава программного обеспечения (SCA), которая позволяет организациям выявлять и снижать риски, связанные с использованием компонентов сторонних разработчиков и компонентов с открытым исходным кодом.

### **Автоматизированное тестирование безопасности**

- [mobsf-ci](https://github.com/Soluto/mobsf-ci): Все, что требуется для запуска MobSF в ci
- [glue](https://github.com/OWASP/glue): Glue - это фреймворк для запуска ряда инструментов. В целом, он предназначен для автоматизации конвейера инструментов анализа безопасности.

### **Хранениe секретов**

- [HashiCorp Vault](https://github.com/hashicorp/vault)

### **Безопасность контейнеров**

- [CIS Docker Benchmark](https://github.com/docker/docker-bench-security): Скрипт для проверки на соответствие best practice.
- [Dockle](https://github.com/goodwithtech/dockle):  Послойный анализ образа контейнера на соответствие best practice.
- [Trivy](https://github.com/aquasecurity/trivy): Анализ образа контейнера на наличие CVE.
- [KICS](https://github.com/Checkmarx/kics): Ультимативная штука по анализу IaC. В отличии от других сканеров, может проверить и docker compose файлы на мисконфигурации.
- [Hadolint](https://github.com/hadolint/hadolint): Линтер Dockerfile.