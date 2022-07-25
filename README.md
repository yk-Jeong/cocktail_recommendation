# 🍸cocktail recommendation model webapp 
추천 시스템 기반 칵테일 추천 모델&웹 애플리케이션 제작

### 기획의도
- **칵테일의 성분**을 기반으로 칵테일 문화에 입문하려는 소비자에게 음료를 추천하고자 함

### 진행과정
데이터 수집 및 정제 → 모델 구축 → DB 업로드 → 웹 애플리케이션 탑재
- 활용 데이터 : thecocktailDB[https://www.thecocktaildb.com/] 의 데이터베이스 api 활용
- 활용 모델(backbone): 추천 시스템 <- 머선 추천 시스템인데여?? 
- 프레임워크: flask

### 파일 설명
- **code.ipynb** 분석을 위해 작성한 전체 코드 
- **presentation.pdf** 프레젠테이션을 위해 제작한 ppt의 pdf 버전

### 한계 및 보완 가능성 
- 데이터 측면: 일러스트/디자인 표지를 분리하지 않고 수집, 표본이 지나치게 적음 → 왜곡 
- 모델 측면: 가상머신의 GPU 한계를 고려하여 깊이를 얕게 설정 → generator가 이미지의 특징을 충분히 탐색하지 못함 
