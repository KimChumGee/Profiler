## 0. 프로그램 개요

### 📌 프로그램명  
**Node.js 기반 Core-Task Profiler**

### 🧩 개발 목적  
이 프로그램은 `inputFile.txt` 파일로부터 Core별 Task 실행 시간 데이터를 입력받아,  
각 Task에 대해 **최소값(MIN), 최대값(MAX), 평균값(AVG), 표준편차(STDDEV)**를 계산하고,  
웹 브라우저를 통해 결과를 **그래프 형태로 시각화**하는 경량 프로파일링 도구입니다.

### ⚙️ 주요 기능

| 기능 | 설명 |
|------|------|
| 📂 파일 업로드 | 브라우저에서 `.txt` 형식의 실행 시간 데이터 업로드 |
| ⚙ 분석 처리 | Node.js 서버에서 Task별 통계 계산 (MIN/MAX/AVG/STDDEV) |
| 📊 시각화 출력 | Chart.js를 이용해 각 Task의 결과를 그래프로 시각화 |
| 📄 보고서 활용 가능 | 분석 결과는 JSON 형태로도 활용 가능 |

### 🏗️ 개발 환경

| 구성 요소 | 설명 |
|-----------|------|
| Node.js | 서버 사이드 프로그래밍 |
| Express.js | 웹 서버 프레임워크 |
| multer | 파일 업로드 처리 |
| Chart.js | 클라이언트 측 데이터 시각화 |
| HTML/CSS | 사용자 UI 구현

### 📁 입력 데이터 형식 예시 (inputFile.txt)

task1 task2 task3 task4 task5
core1 886 749 849 909 352
core2 959 849 788 1053 324
...

### 📈 출력 결과 예시
- 업로드 후 각 Task에 대해  
  → `MIN / MAX / AVG / STDDEV` 값이 막대 그래프로 출력됨  
- 시각화는 Chart.js 기반, Core별 또는 Task별로 커스터마이징 가능
