<div align="center">

# Miguel Ángel Ortiz Escobar

### DevOps & SRE Engineer · Platform Engineering · Cloud & Software Architecture

**IaC (Terraform) · Kubernetes & GitOps · CI/CD y Supply Chain Security · Azure & AWS · Observabilidad · Resiliencia**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/miguel-ortiz13)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@miguelldev)
[![TikTok](https://img.shields.io/badge/TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white)](https://www.tiktok.com/@miguelldev)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/miguelldev_)

</div>

---

## 👋 Sobre mí

Ingeniero **DevOps / SRE** con base sólida en **desarrollo y arquitectura de software**.
Diseño, automatizo y opero plataformas en la nube para que los equipos entreguen
software de forma **rápida, segura, observable y a bajo costo**.

Mi enfoque combina tres capas:

- **Plataforma:** infraestructura como código versionada, gobierno multi-nube (Azure + AWS), identidades sin secretos (OIDC) y FinOps desde el diseño.
- **Entrega:** pipelines CI/CD con controles de calidad y seguridad (SAST, escaneo de IaC, SBOM, firma de imágenes) y despliegue GitOps.
- **Operación:** observabilidad, recuperación ante desastres con RTO/RPO medidos y prácticas SRE para que los sistemas críticos **no dependan de la suerte**.

Como ingeniero de software, también construyo las aplicaciones que despliego:
APIs, frontends y arquitecturas de microservicios de punta a punta.

---

## 🎯 Áreas de especialidad

| Área | Qué aporto |
|---|---|
| 🏗️ **Platform Engineering & IaC** | Bibliotecas de módulos **Terraform** versionados (semver, tests con proveedores simulados, tflint, Checkov, terraform-docs), entornos reproducibles y **Bicep** en Azure |
| 🌐 **Gobierno de nube** | Landing zones como código: **management groups**, una suscripción/cuenta por proyecto, **Azure Policy** y **AWS Organizations + SCP**, presupuestos y alertas de costo |
| ☸️ **Kubernetes & GitOps** | AKS y kind, **Argo CD**, Kustomize, Helm, Gateway API y entrega progresiva (canary) |
| 🔄 **CI/CD & Supply Chain** | **GitHub Actions**, Jenkins y Azure DevOps; Trivy, **SBOM (Syft)**, firma keyless con **Cosign/Sigstore**, Gitleaks, SonarCloud, plan/apply con aprobación |
| 📈 **SRE & Observabilidad** | Prometheus, Grafana, Loki, Tempo, **OpenTelemetry**, New Relic y Log Analytics; SLOs y detección temprana de anomalías |
| 🛟 **Continuidad & DR** | Backups geo-redundantes, pruebas de restauración (SQL, Cosmos DB, Blob, Redis) con **≥99 % de éxito**, retención y legal hold |
| 💰 **FinOps** | Arquitecturas serverless que escalan a cero y aprovechan capas gratuitas: **costo fijo cercano a USD 0** en varios proyectos en producción |
| 🔐 **Seguridad & Cumplimiento** | **OIDC sin secretos**, identidades administradas, Key Vault, RBAC de mínimo privilegio y principios **ISO/IEC 27001** |
| 🧩 **Desarrollo & Arquitectura de Software** | **Java/Spring Boot**, **NestJS/TypeScript**, **Python/FastAPI** y **React**; microservicios, APIs REST, migraciones de bases de datos y diseño orientado a calidad |
| 🔎 **Análisis & Soluciones** | Levantamiento de requisitos, análisis de costos y riesgos, diagramas de arquitectura y documentación técnica (ADRs, runbooks) |

---

## 💼 Experiencia

### IndiGO Tech

**SRE – DR Infrastructure (Junior)** · abr. 2026 – actualidad
- Estandaricé la infraestructura como código con **Terraform** en Azure a nivel de producto: entornos reproducibles, versionados y auditables.
- Automaticé el ciclo de vida de infraestructura y el despliegue de servicios con **Docker** y **Azure Web App**.
- Diseñé y mantengo workflows de CI/CD en **GitHub Actions** y **Jenkins**, con pruebas de resiliencia antes de cada despliegue.
- Implementé monitoreo proactivo con **New Relic** y **Azure Log Analytics** sobre bases de datos y recursos críticos.
- Impulso **Kubernetes** como siguiente capa de estandarización en la orquestación de servicios.

**Continuity & Data Lifecycle Engineer** · sept. 2025 – abr. 2026
- Implementé el plan de recuperación ante desastres de la organización: retención, archivado y legal hold.
- Orquesté backups geo-redundantes y pruebas de recuperación (SQL, Cosmos DB, Blob, Redis) con **≥99 % de éxito en restauraciones** y RTO/RPO dentro de objetivo.
- Trabajé con **Azure Backup, ASR, Blob Lifecycle, Log Analytics y Sentinel**, aportando visibilidad operativa y cumplimiento **ISO/IEC 27001**.

---

## 🚀 Proyectos destacados

### 🏛️ Plataforma y gobierno de nube

| Proyecto | Descripción | Tecnologías |
|---|---|---|
| [**terraform-modules-iac**](https://github.com/miguelortiz13/terraform-modules-iac) | Biblioteca de módulos Terraform multi-proveedor (Azure y AWS) con estándares de nombres, etiquetas, seguridad y costo. Versionado semántico con release-please, tests sin nube (`mock_provider`), pipeline reutilizable de plan/apply con OIDC | Terraform · GitHub Actions · tflint · Checkov · terraform-docs |
| **platform-governance** *(privado)* | Landing zone multi-nube como código. **Azure:** management groups, una suscripción por proyecto, Azure Policy, estado central de Terraform, identidades de despliegue OIDC por repositorio y presupuestos. **AWS:** Organizations con OUs y SCP contra regiones y servicios costosos | Terraform · Azure Policy · AWS Organizations · OIDC |

### 📦 Productos en producción (diseño, desarrollo y operación)

| Proyecto | Descripción | Tecnologías |
|---|---|---|
| [**NexPOS**](https://github.com/miguelortiz13/nexpos-backend) · [frontend](https://github.com/miguelortiz13/nexpos-frontend) | Sistema POS y administrativo para supermercados: ventas, inventario, crédito y cartera, compras a proveedores, facturación PDF, modo offline y lector de códigos de barras por cámara. Desplegado en Azure con **base de datos sin contraseñas** (identidad administrada) y costo fijo ~USD 0 | Java 17 · Spring Boot 3 · Flyway · Azure SQL · React · Container Apps · Static Web Apps · Terraform |
| [**SSPM**](https://github.com/Juandks12/Sistema-de-Gestion-de-Postura-de-Seguridad-SSPM) *(co-autor principal)* | Plataforma SaaS de gestión de postura de seguridad: inventario de activos, escaneos (Nmap, TLS, cabeceras, CVE), puntaje de riesgo, alertas, reportes PDF y API pública para SIEM/SOAR | NestJS · TypeScript · Prisma · PostgreSQL · React · Container Apps · Supabase |
| [**cloudops-copilot**](https://github.com/miguelortiz13/cloudops-copilot) | Copiloto de operaciones cloud: inventario y gobernanza, FinOps, SecOps, cobertura de IaC y agentes de IA. Federación **Azure → AWS sin llaves** (identidad administrada + `AssumeRoleWithWebIdentity`) | Python · FastAPI · SQLAlchemy · React · Azure Resource Graph · boto3 · Terraform |

### 🧪 [devops-sre-lab](https://github.com/miguelortiz13/devops-sre-lab) — Laboratorio DevOps/SRE

Todo lo que un equipo de plataforma necesita para operar microservicios en producción,
construido paso a paso sobre **Online Boutique** (11 microservicios gRPC). Cada proyecto
es un repositorio con evidencia: PRs, ejecuciones de CI y documentación.

| # | Proyecto | Tema | Estado |
|---|---|---|---|
| P0 | [local-k8s-lab](https://github.com/miguelortiz13/local-k8s-lab) | Kubernetes local reproducible: kind, Helm, Makefile y e2e en CI | ✅ |
| P1 | [infra-azure-terraform](https://github.com/miguelortiz13/infra-azure-terraform) | AKS, VNet y Key Vault con Terraform y pipeline OIDC | ✅ |
| P2 | [online-boutique-ci](https://github.com/miguelortiz13/online-boutique-ci) | CI de imágenes: Hadolint, Trivy (SARIF), SBOM, firma Cosign, GHCR y promoción GitOps | ✅ |
| P3 | [platform-gitops](https://github.com/miguelortiz13/platform-gitops) | Argo CD, Kustomize, Gateway API, secretos y canary | ✅ |
| P4 | [observability-stack](https://github.com/miguelortiz13/observability-stack) | Prometheus, Grafana, Loki, Tempo y OpenTelemetry | 🟨 en curso |
| P5 | sre-reliability-lab | SLOs, error budgets, k6, Chaos Mesh, runbooks y postmortems | ⬜ |
| P6 | k8s-security-policies | Kyverno, NetworkPolicies, Falco y Workload Identity | ⬜ |
| P7 | dr-finops | Velero, simulacro de DR (RTO/RPO), autoscaling y OpenCost | ⬜ |
| P8 | infra-aws-terraform | Portabilidad: la misma plataforma en AWS EKS | ⬜ |

### 🧱 Arquitectura de referencia

- [**cloud-mart-platform**](https://github.com/miguelortiz13/cloud-mart-platform): e-commerce de microservicios en Azure con Terraform (Container Apps, PostgreSQL, Redis, Service Bus, Application Gateway) y diagramas de arquitectura en Mermaid generables por agentes de IA.

---

## 🧰 Stack tecnológico

**Cloud**
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Container Apps](https://img.shields.io/badge/Container_Apps-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![AKS](https://img.shields.io/badge/AKS-0078D4?style=flat-square&logo=kubernetes&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)

**IaC, contenedores y GitOps**
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Bicep](https://img.shields.io/badge/Bicep-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Kustomize](https://img.shields.io/badge/Kustomize-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

**CI/CD y seguridad de la cadena de suministro**
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat-square&logo=azuredevops&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat-square&logo=aqua&logoColor=white)
![Sigstore](https://img.shields.io/badge/Cosign_/_Sigstore-2B2D42?style=flat-square&logo=sigstore&logoColor=white)
![Checkov](https://img.shields.io/badge/Checkov-6A2C70?style=flat-square&logo=paloaltonetworks&logoColor=white)
![SonarCloud](https://img.shields.io/badge/SonarCloud-F3702A?style=flat-square&logo=sonarcloud&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Observabilidad y seguridad**
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![New Relic](https://img.shields.io/badge/New_Relic-1CE783?style=flat-square&logo=newrelic&logoColor=black)
![Log Analytics](https://img.shields.io/badge/Log_Analytics-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Microsoft Sentinel](https://img.shields.io/badge/Sentinel-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)

**Desarrollo**
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Datos**
![Azure SQL](https://img.shields.io/badge/Azure_SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Cosmos DB](https://img.shields.io/badge/Cosmos_DB-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

---

## 📜 Certificaciones

| Certificación | Emisor | Año |
|---|---|---|
| AWS Certified AI Practitioner | Amazon Web Services | 2026 |
| New Relic Verified Foundation (NVF) | New Relic | 2026 |
| Microsoft Applied Skills: Protección del almacenamiento para Azure Files y Blob Storage | Microsoft | 2025 |
| Microsoft Certified: Security, Compliance, and Identity Fundamentals (SC-900) | Microsoft | 2025 |
| ISO/IEC 27001 Information Security Associate | SkillFront | 2025 |
| Microsoft Certified: Azure Fundamentals (AZ-900) | Microsoft | 2025 |

## 🎓 Formación

- **Ingeniería de Software** — Universidad Surcolombiana (2022 – 2027)
- **Diplomado en Arquitectura y Calidad de Software** — Universidad Nacional de Colombia (2025)
- **Tecnología en Análisis y Desarrollo de Software** — SENA (2022 – 2024)
- **AWS re/Start, Cloud Computing** — Amazon Web Services (2022)
- **Técnico laboral en Programación con énfasis en aplicaciones web** — Universidad Autónoma de Bucaramanga (2021 – 2022)

---

## 📊 GitHub

<div align="center">

<img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=miguelortiz13&theme=github_dark" alt="Estadísticas de GitHub" />
<img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=miguelortiz13&theme=github_dark" alt="Lenguajes con más commits" />

<img src="https://streak-stats.demolab.com/?user=miguelortiz13&hide_border=true&theme=github-dark-blue" alt="Racha de contribuciones" />

</div>
