### Project (2022.02.11 ~ 2022.02.16)
- - -
# 송전선로 고장 예측

### 주제 선정 이유
- 전력 수요 증가
- 고장 위험 노출 환경
  - 고장시 대전류 혹은 과전압 발생
  - 지속시 화재발생 가능성 유
- 최소 시간동안 오류를 감지하고 작동을 요구 

### 데이터 소개
- 출처 : https://www.kaggle.com/datasets/esathyaprakash/electrical-fault-detection-and-classification?select=detect_dataset.csv
- 3개의 선로 (A, B, C 선로이며 약간의 회로구성이 다름)
  - 각각 선로 전압(V), 전류(I), 불량유무

### 파이프라인
- ![image](https://user-images.githubusercontent.com/78893090/169687863-e5dc28c8-9e53-4ff2-812c-ffa8ce40ecb4.png)

### 웹 구현
- ![image](https://user-images.githubusercontent.com/78893090/169687952-b3b1d0e4-dcdd-49ab-91b9-e7024ae74c42.png)
- 데이터를 입력후 고장을 예측
- 선로 위치를 카카오map으로 표시

### 개선 사항
- 데이터를 입력하는 방식이 아닌 일정 시간 간격으로 데이터를 받아 판단한다
- 불량 발생시 해당 선로의 위치를 나타낼 수 있다

### 주요 스킬
- Flask, SQL
