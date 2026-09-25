# 06. Engineering Takeaways — Manufacturing & Quality

## 1. False Call Matters

품질검사에서는 defect를 많이 찾는 것만으로 충분하지 않다.

false positive가 많으면:

- manual verification 증가
- line response 지연
- unnecessary rework
- engineer workload 증가

가 발생할 수 있다.

AI inspection을 볼 때 accuracy 숫자 하나보다 false-call control과 repeatability를 같이 봐야 한다는 점을 배웠다.

## 2. Analysis Must Be Reproducible

양산기술 / 품질 업무에서 데이터 분석 script가 실제 decision에 사용된다면, code도 하나의 engineering asset이다.

따라서:

- version
- review
- test
- owner
- change reason

이 남아야 한다.

## 3. Knowledge Search Is Part of Response Time

불량 원인을 모르는 것과, 원인은 과거에 해결했지만 기록을 찾지 못하는 것은 현장에서 모두 response delay로 이어질 수 있다.

RAG / enterprise agent를 보면서 **knowledge retrieval speed itself can be a quality metric**이라고 생각했다.

## 4. AI Needs Human-in-the-Loop

제조현장에서 잘못된 판단의 비용은 클 수 있다.

따라서 AI output은 다음과 함께 운영되어야 한다.

- engineering approval
- confidence threshold
- traceable evidence
- exception handling
- rollback / revision history

## 5. Engineering Perspective

이 경험을 통해 양산 / 품질 엔지니어가 AI developer가 아니더라도:

- 어떤 data가 필요한지
- 어떤 output을 믿을 수 있는지
- 어떤 process decision에 연결할지
- 어떻게 검증하고 표준화할지

를 이해하는 것이 중요하다고 느꼈다.

즉, AI 활용의 핵심은 model 자체보다 **현장 문제 정의와 process integration**에 있다고 정리했다.
