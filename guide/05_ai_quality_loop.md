# 05. AI-Enabled Manufacturing Quality Loop

이번 현장 경험에서 세 기업의 기술을 하나의 end-to-end quality loop로 재구성했다.

## Step 1 — Detect

**Delvitech / HORUS**

- visual inspection
- defect classification
- false-call reduction
- repeatable inspection

## Step 2 — Trace & Analyze

**GitLab**

- analysis code versioning
- review
- CI / validation
- root-cause workflow
- change history

## Step 3 — Retrieve Knowledge

**Sionic AI / STORM**

- SOP
- OCAP
- manuals
- defect history
- corrective-action knowledge

## Step 4 — Engineer Decision

AI output는 자동으로 최종 결정을 내리는 것이 아니라 engineer의 판단을 돕는다.

필요한 요소:

- context
- confidence
- process knowledge
- escalation criteria
- approval

## Step 5 — Feedback

조치 후 다음 artifact가 update될 수 있다.

- inspection rule
- analysis script
- SOP / OCAP
- knowledge base
- process condition

## Full Loop

```text
Inspection
   ↓
Anomaly
   ↓
Traceable analysis
   ↓
Knowledge retrieval
   ↓
Corrective action
   ↓
Standardization
   ↓
Feedback to production
```

## Key Insight

제조 AI의 핵심은 한 번의 prediction이 아니라 **closed-loop improvement**라고 정리했다.
