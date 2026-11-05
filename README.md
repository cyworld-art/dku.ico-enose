# E-Nose Digital Twin (교육용 MVP)

React + Vite 기반 화학센서 후각센서 가상 실험 웹앱입니다.

## 실행

```bash
npm install
npm run dev
```

브라우저에서 표시된 localhost 주소를 엽니다.

## Vercel 배포

GitHub 저장소에 업로드한 뒤 Vercel에서 Import Project → Framework: Vite → Build command `npm run build` → Output directory `dist` → Deploy.

## 기능

- 6개 단계별 탐색
- 5채널 MOS 가상 센서 어레이
- 톨루엔/암모니아/에탄올 가상 신호 및 2종 혼합
- 농도, 온도, 상대습도, 노이즈, 드리프트, 유량 설정
- 노출/회복 시계열 및 채널별 특징량
- B-7/B-8/B-9 목표·검증 상태 구분
- 실험 기록(현재 브라우저 세션 한정) 및 CSV 내보내기

## 과학적 제한

모든 감도 계수, 시간상수, 환경 영향 계수는 시연을 위해 가정한 값입니다. 실제 BME688, SGP41 또는 다른 센서의 데이터시트·검량선에 기반한 예측이 아닙니다. B-7의 거리·ppb 검증, B-8의 독립 시험 정확도, B-9의 실제 혼합가스 분류 성능은 구현·입증되지 않았습니다. 이 앱을 유해가스 경보·보호 판단에 사용하지 마세요.
