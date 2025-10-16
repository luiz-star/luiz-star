# Luiz Henrique de O. Bueno

Professor e Consultor | Data & Cloud Architect | Governança de Dados | BI & Analytics | Machine Learning | AWS & Azure

[LinkedIn](https://www.linkedin.com/in/luiz-henrique-sc) • [E-mail](mailto:riquebue@hotmail.com) • [Portfólio 1](https://www.startrainings.net/blog) • [Portfólio 2](https://luiz-star.github.io) • [Empresa](https://www.startrainings.net/)

- Local: Mafra, Santa Catarina, Brasil
- Idiomas: Português (Nativo), Espanhol (Profissional), Inglês (Intermediário)

[English version below](#english-version)

---

## Badges

<!-- Certificações (clique para verificar) -->
[![AWS Certified Machine Learning – Specialty](https://img.shields.io/badge/AWS-ML%20Specialty-orange?logo=amazon-aws&logoColor=white)](https://www.credly.com/badges/2849aea2-ba81-4ee8-86c0-d2848284692b/public_url)
[![AWS Certified Solutions Architect – Professional](https://img.shields.io/badge/AWS-Solutions%20Architect%20Pro-orange?logo=amazon-aws&logoColor=white)](https://www.credly.com/badges/9f4c64e4-d1f2-4a00-976e-82275e844ec7/public_url)
[![Microsoft Certified: Azure Solutions Architect Expert](https://img.shields.io/badge/Azure-Solutions%20Architect%20Expert-0078D4?logo=microsoft-azure&logoColor=white)](https://learn.microsoft.com/pt-br/users/luizhenriquedeoliveirabueno-7070/credentials/dd00a3f2c24ed014?ref=https%3A%2F%2Fwww.linkedin.com%2F)
[![Microsoft Certified: Azure Administrator Associate](https://img.shields.io/badge/Azure-Administrator%20Associate-0078D4?logo=microsoft-azure&logoColor=white)](https://learn.microsoft.com/pt-br/users/luizhenriquedeoliveirabueno-7070/credentials/bf7ca8841cd428e2?ref=https%3A%2F%2Fwww.linkedin.com%2F)

<br/>



<!-- Stack principal -->
![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Analytics%20%7C%20DW-4479A1?logo=postgresql&logoColor=white)
![Apache Spark 3.x](https://img.shields.io/badge/Spark-3.x-E25A1C?logo=apache-spark&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?logo=githubactions&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-IaC-844FBA?logo=terraform&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-Observability-F46800?logo=grafana&logoColor=white)
![AWS Cloud](https://img.shields.io/badge/Cloud-AWS-orange?logo=amazon-aws&logoColor=white)
![Azure Cloud](https://img.shields.io/badge/Cloud-Azure-0078D4?logo=microsoft-azure&logoColor=white)

---

## Status das Actions

- CI de Python (lint e testes)  
[![CI Python](https://github.com/luiz-star/luiz-star/actions/workflows/ci-python.yml/badge.svg?branch=main)](https://github.com/luiz-star/luiz-star/actions/workflows/ci-python.yml)

- Build e scan de imagem Docker (Trivy)  
[![Build and Scan Docker](https://github.com/luiz-star/luiz-star/actions/workflows/docker-build-scan.yml/badge.svg?branch=main)](https://github.com/luiz-star/luiz-star/actions/workflows/docker-build-scan.yml)

- CodeQL (análise de segurança)  
[![CodeQL](https://github.com/luiz-star/luiz-star/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/luiz-star/luiz-star/actions/workflows/codeql.yml)

---

## Sobre mim

Profissional com 10+ anos em Ciência de Dados, especializado em Governança de Dados e Inteligência de Dados, transformando dados em insights e ações. Experiência em arquiteturas de nuvem (AWS e Azure), segurança, automação e melhores práticas. Atuo também como professor e tutor em pós-graduação.

- Resultados: +35% eficiência operacional, +25% precisão de previsões, +40% qualidade de dados, -30% custos operacionais, +25% velocidade de acesso aos dados.
- Áreas de interesse: Cloud Computing, Data Engineering, Data Governance, Big Data, Machine Learning, DevOps, IA, Python, Spark, SQL, Analytics Engineering, Grafana.

---

## Diagramas ASCII — Arquiteturas de Referência

AWS Analytics (Lakehouse com Governança)

AWS Lakehouse (Governança)

[Produtores]
Apps/APIs | Batch | CDC
     |
     v
[Ingestão]
DMS | Glue Jobs | Lambda | Kinesis
     |
     v
+---------------------------+
|         Data Lake         |
|  S3 Bronze | Silver | Gold|
+-----+-----------+---------+
      |           |
      v           v
[Catálogo]    [Governança]
Glue Catalog  Lake Formation + IAM
      |           |
      +-----+-----+
            |
            v
[Consulta/Serviço]
Athena | Redshift | EMR/Spark
            |
            v
[BI/Consumo]
QuickSight | Apps | APIs
            |
            v
[Observ./Auditoria]
CloudWatch | CloudTrail | CW Logs
