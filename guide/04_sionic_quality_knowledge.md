# 04. Sionic AI — Quality Knowledge Agent

## STORM Platform

Sionic AI의 STORM은 enterprise AI agent platform이다.

공식 사이트 기준 주요 기능:

- no-code agent / workflow builder
- RAG-based enterprise search
- unstructured document parsing
- On-premise / Private Cloud / SaaS
- access control
- version management
- operational dashboard

Sionic AI는 제조를 포함한 여러 산업의 enterprise AI deployment experience도 소개하고 있다.

## Why This Was Relevant to Semiconductor Quality

반도체 현장에는 많은 knowledge artifact가 존재한다.

- SOP
- OCAP
- FMEA
- 8D / CAPA
- equipment manual
- defect report
- process-change history
- troubleshooting guide

문제는 자료가 존재해도 필요한 순간에 빠르게 찾지 못하면 대응 시간이 길어진다는 점이다.

## My Application Idea

STORM과 같은 enterprise RAG system을 품질 workflow에 적용한다면 다음 질문을 빠르게 탐색하는 구조를 생각할 수 있다.

- 이 defect와 유사한 과거 사례가 있었는가?
- 해당 alarm 발생 시 어떤 OCAP을 따라야 하는가?
- 이 설비 문제와 관련된 manual section은 어디인가?
- 이전 process change 이후 유사 issue가 있었는가?

## Important Scope

이는 **내가 현장에서 도출한 semiconductor quality application idea**다.

Sionic AI가 현재 semiconductor-fab용 OCAP/FMEA product를 공식적으로 판매한다고 주장하는 것이 아니다.

핵심은 enterprise RAG가 **현장 지식 검색시간과 response consistency를 줄일 수 있는 구조**라는 점이다.
