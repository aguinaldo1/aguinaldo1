<div align="center">

# Aguinaldo Américo

### Site Reliability Engineer • DevOps • Observability

**Construindo sistemas confiáveis, observáveis e resilientes.**

`Linux` `Java` `AWS` `OCI` `Kubernetes` `Prometheus` `Grafana` `Terraform` `Docker`

<br>

[![Portfolio](https://img.shields.io/badge/Portfolio-Visitar-0A66C2?style=for-the-badge&logo=vercel&logoColor=white)](https://aguinaldo-americo-cv.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aguinaldo-americo)
[![Email](https://img.shields.io/badge/Email-Contato-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aguinaldoamerico2@gmail.com)

</div>

---

## 👋 Sobre mim

Sou **Aguinaldo Américo**, profissional de tecnologia com experiência em **Site Reliability Engineering (SRE), sustentação, monitoramento e observabilidade de aplicações**.

Atuei como **SRE no Itaú Unibanco via NTT DATA**, trabalhando com acompanhamento de ambientes, análise de falhas, troubleshooting e observabilidade.

Hoje concentro meu desenvolvimento técnico em quatro pilares:

> **Observabilidade • Incident Response • Automação • Reliability Engineering**

Meu portfólio é construído com laboratórios reproduzíveis nos quais simulo falhas, coleto evidências, investigo sintomas, identifico causas e valido a recuperação dos serviços.

---

## 🧭 Navegação rápida

[Projetos](#-projetos-em-destaque) •
[Roadmap](#-roadmap-sre) •
[Stack](#️-stack-técnica) •
[Experiência](#-experiência) •
[Formação](#-formação--certificações) •
[Contato](#-contato)

---

# 🚀 Projetos em destaque

> Projetos práticos construídos para demonstrar **como penso e atuo diante de problemas de confiabilidade**, e não apenas quais ferramentas conheço.

## P02 • SRE Production API Monitoring

**Monitoramento, alertas e investigação de incidentes em uma API Java/Spring Boot.**

[![Status](https://img.shields.io/badge/STATUS-COMPLETO-success?style=flat-square)](https://github.com/aguinaldo1/sre-production-api-monitoring)
[![Java](https://img.shields.io/badge/Java-17-orange?style=flat-square&logo=openjdk)](https://github.com/aguinaldo1/sre-production-api-monitoring)
[![Prometheus](https://img.shields.io/badge/Prometheus-Metrics-E6522C?style=flat-square&logo=prometheus&logoColor=white)](https://github.com/aguinaldo1/sre-production-api-monitoring)
[![Grafana](https://img.shields.io/badge/Grafana-Dashboards-F46800?style=flat-square&logo=grafana&logoColor=white)](https://github.com/aguinaldo1/sre-production-api-monitoring)

### O problema

Como detectar rapidamente quando uma API apresenta **erros, indisponibilidade ou degradação de latência**?

### O que implementei

- API Java 17 / Spring Boot;
- instrumentação com Actuator e Micrometer;
- coleta de métricas com Prometheus;
- dashboards no Grafana;
- alertas com Alertmanager;
- análise dos Golden Signals;
- simulação controlada de incidentes;
- introdução de SLI, SLO, Error Budget e Burn Rate.

### Incidentes

| Cenário               | Sinal observado | Detecção            |
| :-------------------- | :-------------- | :------------------ |
| 🔴 API indisponível   | Availability    | `up == 0`           |
| 🟠 Alta taxa de erros | Errors          | Prometheus / PromQL |
| 🟡 Alta latência      | Latency p95     | Prometheus / PromQL |

**Resultado:** ambiente reproduzível para detectar degradação, visualizar sinais operacionais e investigar incidentes com evidências.

➡️ **[Ver projeto completo →](https://github.com/aguinaldo1/sre-production-api-monitoring)**

---

## P01 • Linux Production Troubleshooting Lab

**Investigação sistemática de incidentes de produção em ambiente Linux.**

[![Status](https://img.shields.io/badge/STATUS-COMPLETO-success?style=flat-square)](https://github.com/aguinaldo1/sre-linux-troubleshooting-lab)
[![Linux](https://img.shields.io/badge/Linux-Troubleshooting-FCC624?style=flat-square&logo=linux&logoColor=black)](https://github.com/aguinaldo1/sre-linux-troubleshooting-lab)
[![Java](https://img.shields.io/badge/Java-Application-orange?style=flat-square&logo=openjdk)](https://github.com/aguinaldo1/sre-linux-troubleshooting-lab)

### O problema

Como investigar lentidão e indisponibilidade sem declarar uma causa raiz antes de possuir evidências suficientes?

### Método utilizado

**Sintoma → Hipóteses → Evidências → Testes → Diagnóstico → Causa raiz → Mitigação → Validação**

### Incidentes investigados

| Incidente | Cenário                   | Principais ferramentas          |
| :-------- | :------------------------ | :------------------------------ |
| INC-001   | I/O Saturation            | `iostat` `pidstat` `df` `lsblk` |
| INC-002   | CPU Saturation            | `top` `nproc` `ps`              |
| INC-003   | Memory Pressure           | `free` `ps`                     |
| INC-004   | Service Failure           | `systemctl` `journalctl`        |
| INC-005   | Port Connectivity Failure | `ss` `curl`                     |

**Resultado:** documentação de uma metodologia de troubleshooting orientada por evidências para CPU, memória, disco, serviços e conectividade.

➡️ **[Ver projeto completo →](https://github.com/aguinaldo1/sre-linux-troubleshooting-lab)**

---

# 🗺️ Roadmap SRE

O portfólio evolui de fundamentos de troubleshooting até engenharia de resiliência.

| Projeto                                  | Competência principal        | Status |
| :--------------------------------------- | :--------------------------- | :----: |
| **P01** Linux Production Troubleshooting | Troubleshooting + RCA        |   ✅   |
| **P02** Production API Monitoring        | Metrics + Alerting           |   ✅   |
| **P03** Full Stack Observability         | Metrics + Logs + Traces      |   🔨   |
| **P04** Reliability Engineering          | SLI + SLO + Error Budget     |   🗓️   |
| **P05** Kubernetes Reliability           | Reliability em Kubernetes    |   🗓️   |
| **P06** Chaos Engineering                | Resiliência + experimentação |   🗓️   |

### Próximo passo • P03 Full Stack Observability

```text
METRICS ─┐
LOGS ────┼──► CORRELATION ──► INVESTIGATION ──► ROOT CAUSE
TRACES ──┘
```

O objetivo é evoluir do monitoramento baseado principalmente em métricas para uma investigação correlacionando **métricas, logs e traces**.

---

# 🛠️ Stack técnica

<table>
<tr>
<td width="33%" valign="top">

### ⚙️ Reliability

- Observability
- Incident Response
- Troubleshooting
- Root Cause Analysis
- Golden Signals
- SLI / SLO
- Error Budget
- Burn Rate
- Chaos Engineering

</td>
<td width="33%" valign="top">

### 📈 Observability

- Prometheus
- Grafana
- Alertmanager
- AppDynamics
- Splunk
- Datadog
- CloudWatch
- Micrometer
- PromQL

</td>
<td width="33%" valign="top">

### ☁️ Platform

- Linux
- Java / Spring Boot
- Docker
- Kubernetes
- AWS
- OCI
- Terraform
- Ansible
- GitHub Actions

</td>
</tr>
</table>

---

# 💼 Experiência

### Site Reliability Engineering / DevOps

Experiência em ambientes corporativos com:

- monitoramento e sustentação de aplicações;
- observabilidade e acompanhamento de métricas e logs;
- troubleshooting e análise de incidentes;
- análise de disponibilidade e desempenho;
- suporte à identificação de causa raiz;
- documentação técnica;
- melhoria contínua da confiabilidade operacional.

**Experiência anterior:** SRE no **Itaú Unibanco via NTT DATA**.

---

# 🎓 Formação & Certificações

**Big Data e Inteligência Analítica — UNIASSELVI**

Certificações e desenvolvimento:

- **Gremlin Certified Chaos Engineering Professional — GCCEPro**
- **CCNA: Introduction to Networks**
- Certificação Executiva: Desenvolvimento de Negócios, Liderança e Networking
- Estudos contínuos em SRE, DevOps, Cloud, Linux, Kubernetes e Observabilidade

---

# 🧪 Engenharia orientada por evidências

A filosofia aplicada aos laboratórios é simples:

```text
PROBLEMA
   │
   ▼
BASELINE
   │
   ▼
FALHA CONTROLADA
   │
   ▼
OBSERVAÇÃO + EVIDÊNCIAS
   │
   ▼
INVESTIGAÇÃO
   │
   ▼
DIAGNÓSTICO
   │
   ▼
MITIGAÇÃO
   │
   ▼
VALIDAÇÃO + DOCUMENTAÇÃO
```

> **Ferramentas são meios. Evidências, diagnóstico e recuperação demonstram a prática de engenharia.**

---

<details>
<summary><strong>🤖 Transparência sobre uso de Inteligência Artificial</strong></summary>

<br>

Utilizo ferramentas de Inteligência Artificial como apoio para pesquisa, revisão, aprendizado e organização da documentação.

Nos projetos técnicos, os experimentos, comandos, configurações, simulações de incidentes, coleta de evidências, troubleshooting e validações são executados e analisados por mim.

A IA funciona como ferramenta de apoio ao processo de engenharia e aprendizado, sem substituir a compreensão técnica das implementações apresentadas.

</details>

---

# 📊 GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=aguinaldo1&show_icons=true&hide_border=true" alt="GitHub statistics" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=aguinaldo1&layout=compact&hide_border=true" alt="Most used languages" />

</div>

---

# 📫 Contato

<div align="center">

### Vamos conversar sobre confiabilidade de sistemas?

Estou aberto a conexões profissionais e oportunidades relacionadas a **SRE, DevOps, Observabilidade, Cloud e Reliability Engineering**.

<br>

[![Portfolio](https://img.shields.io/badge/PORTFÓLIO-Visitar-0A66C2?style=for-the-badge&logo=vercel&logoColor=white)](https://aguinaldo-americo-cv.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LINKEDIN-Conectar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aguinaldo-americo)
[![GitHub](https://img.shields.io/badge/GITHUB-aguinaldo1-181717?style=for-the-badge&logo=github)](https://github.com/aguinaldo1)
[![Email](https://img.shields.io/badge/EMAIL-Contato-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aguinaldoamerico2@gmail.com)

<br>

**Reliability is not just uptime.**  
_É a capacidade de detectar, entender, responder e aprender com falhas._

</div>
