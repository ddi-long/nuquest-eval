# NUQUEST 자동 평가 도구

RCT 논문(PDF)을 업로드하면 NUQUEST 14개 항목에 대한 평가 결과를 자동으로 생성하는 웹 도구입니다.

## 사용 방법

1. https://ddi-long.github.io/nuquest-eval/ 접속
2. Gemini API 키 입력 (최초 1회, 본인 브라우저에만 저장됨)
3. RCT 논문 PDF 업로드 (최대 5개)
4. 결과 확인 및 엑셀 다운로드

## Gemini API 키 발급 (무료, 5분)

1. https://aistudio.google.com/app/apikey 접속
2. 구글 계정 로그인 → "Create API key" 클릭
3. `AIzaSy`로 시작하는 키 복사 → 본 도구의 API 키 입력란에 붙여넣기

신용카드 불필요, Gemini 2.5 Flash 무료 티어 사용 (분당 약 15회, 일 약 1,500회).

## 주의사항

⚠️ **무료 티어는 Google이 입력 내용을 모델 개선에 활용할 수 있습니다.**
미발표 논문, 동료심사 중 원고, 기밀 자료의 평가에는 사용을 권장하지 않습니다.
이미 출판된 논문 평가에만 사용하세요.

## 적용 대상

- 적용 가능: RCT (parallel-arm, crossover, acute randomized feeding trial)
- 적용 불가: 비무작위 중재연구, single-arm, observational study

## 평가 결과 표시

| 표시 | 의미 |
|---|---|
| 🟢 초록 원 | 발췌 문장이 PDF 원문에 일치 — 신뢰 가능 |
| 🟡 노란 원 | 유사 매칭이거나 검토 필요 — 사용자 확인 권장 |
| 🔴 빨간 원 | 발췌 문장 PDF 미발견 — hallucination 의심 |
| ⚪ 회색 원 | 적용되지 않음 |

## 라이선스 / 데이터

- API 키와 PDF는 사용자 브라우저에만 머무르며, GitHub 또는 본 도구 운영자에게 전송되지 않습니다.
- Gemini API에는 PDF 텍스트가 전송됩니다 (Google 무료 티어 약관 적용).
