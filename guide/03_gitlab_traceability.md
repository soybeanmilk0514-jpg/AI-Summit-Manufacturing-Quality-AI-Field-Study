# 03. GitLab — Engineering Traceability

## What GitLab Provides

GitLab은 software development / DevSecOps platform이며, GitLab Duo Agent Platform은 AI agents를 software lifecycle에 연결한다.

공식 GitLab documentation의 대표 use case:

- CI/CD pipeline failure diagnosis
- root-cause analysis
- automated code review
- security review
- issue-to-merge-request workflow

## Why I Connected This to Manufacturing

반도체 양산 / 품질 조직에서도 많은 분석 logic이 code 형태로 존재할 수 있다.

예:

- SPC analysis
- equipment-log parsing
- defect-data preprocessing
- recipe comparison
- dashboard generation
- automated reporting

이러한 script가 사람마다 다르게 관리되면:

- 결과 재현성이 낮아질 수 있고
- 수정 이유가 사라지며
- 검증되지 않은 version이 사용될 수 있다.

## Manufacturing Application I Derived

```text
Abnormal event
   ↓
Issue registration
   ↓
Analysis script modification
   ↓
Peer review / version history
   ↓
Automated validation
   ↓
Approved tool
   ↓
Traceable engineering decision
```

## Main Takeaway

GitLab booth에서 가장 의미 있게 본 포인트는 “AI가 code를 생성한다”가 아니라,

**분석 workflow와 변경 이력을 시스템적으로 관리할 수 있다는 점**이었다.

품질관리에서는 결과 자체뿐 아니라 “누가, 언제, 왜 분석 logic을 바꿨는가”가 중요한 traceability 정보가 될 수 있다.
