## 3 일차
- [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTOpyvf8OAZ_zyuEyXoyuWkcrQdXQR0sOMrOg&s)

### 1. [서울시 따릉이 데이터](https://data.seoul.go.kr/dataList/OA-15182/F/1/datasetView.do) 수집
### 2. 따릉이 데이터 기초분석(EDA, Exploratory Data Analysis)
### 3. 서울시 따릉이 데이터 전처리 (Data Preprocessin)

# 실전 종합과제 (데이터 전처리 및 시각화까지)
### 1. 선지후행(先知後行)
- 문제를 정의하고(Problem Definition)
- 전체 작업을 설계하고(Process Definition)
- 작업 방법론은 순차적으로 정의하고
- LLM에 질문하고
- 코딩을 만들고 그 내용을 공부한다.

### 2. LLM과 코딩 작업 수행과정(하드/소프트 스킬 사용)
1. 원자료 : [Raw Data](https://adstat.kobaco.co.kr/mcr/portal/mainPage.do)  에서 [2018년/2019년도 데이터 수집](https://adstat.kobaco.co.kr/mcr/portal/dataSet/mdssListPage.do)
2. 데이터 수집 (Obtain Data)
    - 데이터의 결측치, 고유값, 데이터 형태, 데이터 내용 등 확인
    - Object 데이터 변환
    - 통계학 데이터 종류와 예시
# 통계학 데이터 종류와 예시

| 대분류 | 소분류 | 설명 | 예시 |
|:------|:------|:------|:------|
| 범주형(Categorical) | 명목형(Nominal) | 의미 없이 단순 구분하는 데이터 | 성별(남/여), 혈액형(A/B/O/AB), 국적(한국/미국/일본) |
|  | 순서형(Ordinal) | 순서나 등급은 있으나 간격은 불규칙 | 학점(A/B/C), 건강 상태(양호/보통/불량) |
| 수치형(Numerical) | 이산형(Discrete) | 셀 수 있는 정수 형태 데이터 | 자녀 수(0,1,2명), 판매 수량, 출석일수 |
|  | 연속형(Continuous) | 연속적으로 측정 가능하며 소수점 값 존재 | 키(170.5cm), 체중(65.2kg), 시간(2.35초) |
|  | 등간형(Interval) | 0의 의미가 없고, 차이만 의미 | 온도(섭씨 20도, 30도), 날짜(2000년, 2025년) |
|  | 비율형(Ratio) | 절대적 0이 존재하며, 비율 계산이 가능 | 무게(0kg, 50kg), 매출액(0원, 100만원) |  

3. 결측치 대체 (Missing Value Imputation)
    - 결측치를 어떤 방식으로 처리(제거, 대체 방법 등등)할 지 결정
        - 결측치를 가진 변수 : 소득, 자녀수,
          
4. 이상치 처리 (Anomaly Detection)
    - 상자박스 IQR
      
5. [데이터 시각화 (Data Visualization)](https://github.com/ancestor9/beat-master/blob/main/5%EC%9E%A5%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EC%8B%9C%EA%B0%81%ED%99%94.ipynb)

6. [특성공학](https://github.com/ancestor9/2025_Spring_Data-Management/blob/main/week_10/A%20Short%20Guide%20for%20Feature%20Engineering%20and%20Feature%20Selection.pdf)
    - 1. 기존변수 변환
      - [정규화(number --> number)](https://pycaret.gitbook.io/docs/get-started/preprocessing/scale-and-transform)
      - [이산화(number --> category)](https://pycaret.gitbook.io/docs/get-started/preprocessing/feature-engineering)
      - [dummy화(categoty --> number): Onehotencoder](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html)

    - 2. 새로운 변수 추출(Feature Extraction)
7. 특성 추출 (Feature Selection)
    - [Feature selection](https://scikit-learn.org/stable/modules/feature_selection.html)

8. 예측 모형 개발
![머신러닝 연구절차](https://www.scribbr.nl/wp-content/uploads/2023/07/machine-learning-process-flow.webp)
