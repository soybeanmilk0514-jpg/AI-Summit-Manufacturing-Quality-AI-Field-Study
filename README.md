# AI Summit Seoul & Expo 2026 — Manufacturing & Quality AI Field Study

2026년 8월 20일 서울 코엑스에서 열린 **AI Summit Seoul & EXPO 2026** 전시를 방문해 AI 솔루션을 직접 체험하고, 현장 실무자들과 대화하며 **AI가 제조·양산·품질관리 업무에 어떻게 적용될 수 있는지** 조사한 field-study project입니다.

공식 행사 일정은 2026년 8월 19–21일이며, Expo는 COEX 전시장 B홀에서 진행되었습니다.

이번 현장 경험에서 특히 인상 깊었던 세 기업/솔루션을 제조 품질 업무의 서로 다른 레이어로 재구성했습니다.

- **Delvitech / KAIS — HORUS**: AI-native 3D AOI & SPI를 통한 자동 검사
- **GitLab — Duo Agent Platform**: 분석 코드·자동화 workflow의 변경 추적과 CI/CD 품질 관리
- **Sionic AI — STORM**: 기업 내부 문서와 지식을 활용하는 RAG / AI Agent

> The goal of this repository is not to claim that all three products are semiconductor-fab solutions. It documents what I observed at the expo and then translates each technology into realistic manufacturing / quality-management use cases.

---

## Field Visit at a Glance

| Item | Details |
|---|---|
| Event | AI Summit Seoul & EXPO 2026 |
| Visit date | 2026.08.20 |
| Official event dates | 2026.08.19–21 |
| Venue | COEX Grand Ballroom & Exhibition Hall B |
| Visit type | EXPO visitor / booth experience |
| Career lens | Semiconductor manufacturing technology / quality management |
| Main companies | Delvitech / KAIS, GitLab, Sionic AI |
| Core question | How can AI improve inspection, engineering traceability, and quality knowledge workflows? |

![Field visit](./figures/field-visit-01.jpg)

*Field photo at the Delvitech / KAIS HORUS demonstration area.*

---

## Why I Viewed the Expo Through a Manufacturing / Quality Lens

AI 전시회에는 생성형 AI, 개발도구, 비전검사, enterprise agent 등 서로 다른 기술이 섞여 있었습니다.

나는 각 솔루션을 단순히 “AI 기술”로 보는 대신 다음 제조 현장 질문에 연결했습니다.

1. **불량을 더 빨리, 일관되게 찾을 수 있는가?**
2. **분석 코드와 자동화 로직의 변경 이력을 남길 수 있는가?**
3. **과거 품질 이력과 표준 대응 절차를 빠르게 찾을 수 있는가?**
4. **검사 → 원인 분석 → 조치 → 재발방지의 feedback loop를 더 짧게 만들 수 있는가?**

이 관점에서 세 기업의 역할은 서로 경쟁 관계라기보다 **하나의 quality loop에서 다른 문제를 해결하는 기술**로 볼 수 있었습니다.

---

## 1. Delvitech / KAIS — AI-Native Visual Inspection

사진 속 장비는 Delvitech의 **HORUS** 계열 AI 3D inspection platform입니다. 국내에서는 KAIS가 AI Summit Seoul & Expo 2026에서 제조 혁신용 자동화 솔루션으로 소개했습니다.

HORUS는 SMT/PCB 생산을 대상으로:

- 3D SPI
- pre-reflow AOI
- post-reflow AOI
- AI-based classification
- 3D optical measurement

을 하나의 platform에서 다루는 방향의 검사 시스템입니다.

![HORUS field visit](./figures/field-visit-02.jpg)

### What I Learned from a Quality Perspective

기존 rule-based inspection은 threshold와 recipe tuning에 많은 engineering effort가 필요할 수 있습니다.

AI-native inspection의 가치 포인트를 다음과 같이 정리했습니다.

- defect classification consistency
- false-call reduction
- inspection recipe reuse / standardization
- faster line setup
- less manual verification
- more scalable multi-line quality control

### Important Scope

HORUS는 **SMT / PCB assembly inspection** 장비입니다.

따라서 이 경험을 wafer front-end inspection 경험으로 표현하지 않습니다.

대신 다음 transferable concept을 반도체 품질관리 / 양산기술에 연결했습니다.

**machine vision → defect classification → false-call management → traceable inspection result → process feedback**

---

## 2. GitLab — Engineering Traceability for Manufacturing Analytics

GitLab은 검사장비 자체가 아니라 software development / DevSecOps platform입니다.

GitLab Duo Agent Platform은 AI agents를 software lifecycle에 연결하고, GitLab 공식 문서에서 다음과 같은 use case를 제공합니다.

- failed CI/CD pipeline diagnosis
- root-cause analysis
- code review
- security review
- issue → merge-request automation

### My Manufacturing Application Idea

반도체 양산/품질 조직에서도 다음과 같은 engineering artifacts가 계속 바뀝니다.

- SPC analysis Python scripts
- defect-data preprocessing code
- equipment-log parser
- recipe-comparison script
- dashboard logic
- automated report generator

이 파일들이 개인 PC에만 남거나 변경 이력이 불명확하면 재현성과 품질이 떨어질 수 있습니다.

GitLab의 개념을 다음처럼 제조 엔지니어링에 적용할 수 있다고 생각했습니다.

```text
Issue / abnormal event
        ↓
Analysis code change
        ↓
Version-controlled review
        ↓
Automated test / CI
        ↓
Approved engineering tool
        ↓
Traceable root-cause analysis
```

즉 GitLab에서 가장 인상 깊었던 점은 “AI가 코드를 대신 써준다”보다 **engineering logic itself can be traceable and reviewable**하다는 점이었습니다.

---

## 3. Sionic AI — Enterprise Knowledge for Quality Response

Sionic AI의 **STORM Platform**은 현업 사용자가 no-code 방식으로 AI agent를 만들고, 기업 내부 문서를 RAG 기반으로 검색·활용할 수 있게 하는 enterprise AI platform입니다.

공식 자료에서 확인되는 주요 기능:

- no-code workflow / agent builder
- RAG-based enterprise search
- unstructured-document parsing
- On-premise / Private Cloud / SaaS deployment
- access control and version management
- operational dashboard
- manufacturing-industry deployment experience

### My Semiconductor Quality Application Idea

반도체 품질 / 양산 현장에는 다음과 같은 문서가 축적됩니다.

- SOP
- OCAP
- FMEA
- 8D / CAPA
- equipment manuals
- defect reports
- process-change history
- troubleshooting guides

이 지식을 RAG agent로 연결한다면 다음과 같은 질문을 빠르게 탐색하는 형태를 생각할 수 있습니다.

> “이 defect와 유사한 과거 사례가 있었는가?”

> “해당 이상 발생 시 어떤 OCAP 순서를 따라야 하는가?”

> “이 설비 alarm과 관련된 manual / 과거 조치 이력은 무엇인가?”

이 부분은 **Sionic AI가 현재 반도체용 품질관리 제품을 제공한다는 주장**이 아니라, STORM의 enterprise-RAG 기능을 바탕으로 내가 현장에서 확장해 본 manufacturing use case입니다.

---

## AI-Enabled Quality Loop

세 기업을 하나의 제조 품질 workflow로 연결하면 다음과 같이 정리할 수 있습니다.

```text
[1] Detect
Delvitech / HORUS
AI visual inspection
        ↓
[2] Trace & Analyze
GitLab
versioned analysis logic / CI / RCA
        ↓
[3] Retrieve Knowledge
Sionic AI / STORM
SOP / OCAP / history / manuals
        ↓
[4] Corrective Action
Engineer decision + standard response
        ↓
[5] Feedback
inspection rule / analysis tool / knowledge base update
```

이 구조에서 AI는 엔지니어를 대체하는 단일 도구가 아니라, **검출–분석–지식검색–조치의 시간을 줄이는 보조 infrastructure**로 해석했습니다.

---

## What This Means for Semiconductor Manufacturing / Quality

### Manufacturing Technology

- equipment / process data interpretation
- abnormality detection
- recipe / condition change traceability
- faster root-cause workflow
- standardized engineering scripts

### Quality Management

- inspection false-call reduction
- defect history retrieval
- structured corrective-action knowledge
- reproducible analysis
- audit-friendly change history

### My Main Takeaway

현장에서 느낀 가장 중요한 점은 **“AI 모델의 정확도”만으로 제조 AI의 가치가 결정되지 않는다는 것**이었습니다.

실제 현장 적용에는:

- reliable data acquisition
- false-positive control
- version / change management
- domain knowledge
- human approval
- feedback to the production process

가 함께 필요합니다.

---

## Read the Project

| Page | Description |
|---|---|
| [Project Page](./index.html) | 현장 경험 전체 요약 |
| [Navigation](./guide/00_navigation.md) | 전체 문서 안내 |
| [Event Context](./guide/01_event_context.md) | 행사 공식 정보와 방문 목적 |
| [Delvitech / HORUS](./guide/02_delvitech_horus.md) | AI inspection과 품질관리 |
| [GitLab](./guide/03_gitlab_traceability.md) | 분석 코드와 engineering traceability |
| [Sionic AI](./guide/04_sionic_quality_knowledge.md) | RAG 기반 품질 지식 활용 |
| [Quality Loop](./guide/05_ai_quality_loop.md) | 세 기술을 하나의 workflow로 연결 |
| [Career Takeaways](./guide/06_career_takeaways.md) | 양산·품질 직무 관점의 학습 |
| [Evidence Scope](./guide/07_evidence_scope.md) | 현장 경험 / 공식 자료 / 적용 아이디어 구분 |
| [References](./references/README.md) | 공식 행사·기업 자료 |
| [Field Photos](./figures/README.md) | 현장 사진 설명 |

---

## Structured Analysis

- [company_technology_matrix.csv](./results/company_technology_matrix.csv)
- [manufacturing_ai_use_cases.csv](./results/manufacturing_ai_use_cases.csv)
- [quality_loop.csv](./results/quality_loop.csv)

These tables are portfolio analysis artifacts, not company-provided performance data.

---

## Repository Structure

```text
AI-Summit-Manufacturing-Quality-AI-Field-Study/
├── README.md
├── index.html
├── index.md
├── _config.yml
├── assets/
├── figures/
├── guide/
├── results/
├── study/
├── references/
├── appendix/
├── source/
└── report/
```

---

## Scope

This repository clearly separates:

1. **Personal field experience** — booth visits, demonstrations, and conversations at AI Summit Seoul & Expo 2026
2. **Company-supported facts** — product/platform capabilities from official sources
3. **My application ideas** — how these technologies could support semiconductor manufacturing and quality workflows

No employment, implementation, or production deployment at these companies is claimed.

---

[← Back to Subin Joo's GitHub Portfolio](https://github.com/soybeanmilk0514-jpg)
