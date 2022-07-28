# 🍸cocktail recommendation model webapp 
추천 시스템 기반 칵테일 추천 모델&웹 애플리케이션 제작 프로젝트


### 프로젝트 개요
(기획의 배경 및 의도 들어갈 자리) 

- 전제: '칵테일에 대한 선호도는 칵테일 성분의 **유사도**로 측정할 수 있다'
- 프로젝트의 목표: 칵테일 문화에 입문하려는 소비자에게 음료를 **추천**하고자 함

### 파일 설명
- **code.ipynb** 분석을 위해 작성한 전체 코드(`google colab`에서 작업)
- **presentation.pdf** 프레젠테이션을 위해 제작한 ppt의 pdf 버전
- **model.pkl** 부호화한 모델(복호화 테스트 완료)

>💭 **작업환경** `google colab` `flask` `PostgreSQL` `VScode` `Heroku`
>
>📅 **진행기간** 1차 21.12.08 ~ 21.12.13 수정 22.08.00~
### 문제해결 과정
데이터 수집 및 정제 → 모델 구축 → DB 업로드 → 웹 애플리케이션 탑재 → 배포
- 분석 기법: 코사인 유사도 
- 사용 모델: tfidvectorizer 


### 데이터 세트의 특징

- 출처: 칵테일 관련 DB 중 가장 방대하고 접근성이 뛰어난 [TheCocktailDB](https://www.thecocktaildb.com/)의 openAPI를 활용
- 구성: 이름, 고유ID, 알코올 포함 여부, 분류, 서빙 잔의 형태, IBA 등록 여부, 성분(15가지), 각 성분당 분량

※데이터 세트 전처리 과정: 결측치 비율을 확인하여 **총 15종의 성분 중 주성분 5종**만 사용
그 외 결측치 제거, 대소문자 통일 등 기본적인 전처리 완료 

### 결과 요약

- 가설: 검증되었는지?
- 목표: 달성되었는지?
- 그 밖에 기대하지 않았던 인사이트가 있었다면?

### 한계점과 보완 방안
- 해결하지 못한 문제: TheCocktailDB 원본이 업데이트될 때마다 자동으로 업데이트할 수 없을까? 

#### 한계
- 데이터상의 한계, 모델 구축상의 한계, HW상의 한계 등

#### 보완방안
- 



### Update

- (2022.07.26~) 프로젝트 소개문 재작성

