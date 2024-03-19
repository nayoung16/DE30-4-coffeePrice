# ☕ 2022년도 커피 물가 상승 요인 및 커피 소비 분석 프로젝트
### 🌱 TEAM
PLAYDATA 데이터 엔지니어링 30기<br/><br/>
[김나영](https://github.com/nayoung16) [김보경](https://github.com/michelle9876) [정제윤](https://github.com/JeongJeaYoon) [최예림](https://github.com/CYERIM)
### 🚀 Used Tech
![Google Colab Badge](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab&logoColor=fff&style=for-the-badge)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Rocky Linux](https://img.shields.io/badge/-Rocky%20Linux-%2310B981?style=for-the-badge&logo=rockylinux&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Apache Hadoop](https://img.shields.io/badge/Apache%20Hadoop-66CCFF?style=for-the-badge&logo=apachehadoop&logoColor=black)
![Apache Hive](https://img.shields.io/badge/Apache%20Hive-FDEE21?style=for-the-badge&logo=apachehive&logoColor=black)
### 📘 Used Datas
#### 공공데이터포털
- 생활물가지수
- 서울시 일반음식점 인허가 정보
- 서울시 휴게음식점 인허가 정보
- 서울시 사업체조사결과정보
#### 농식품수출정보
- 2021년~ 2023년 커피 품목 수입 데이터
#### 크롤링
- 2021.01 ~ 2023.01 네이버 뉴스 기사 크롤링
## ☕ 프로젝트 개요
### 동기
다양한 품목의 3년 간 생활물가지수 변화 추이를 살펴보았다. 그 중 22년 커피 물가가 조금 특이했는데, 년초에 물가 상승 후 1년 동안 동결되던 기존과 달리 22년 커피 물가는 1년 동안 꾸준히 상승하였다.<br/>
#### 커피 생활물가지수
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/coffee_bean/%EC%BB%A4%ED%94%BC_%EC%83%9D%ED%99%9C%EB%AC%BC%EA%B0%80%EC%A7%80%EC%88%98_%EB%B3%80%ED%99%94.png"
  style="float: left" width=700><br/>
2022년은 코로나 거리두기가 해제되며 다시 상권이 활기를 찾기 시작한 시기기에 커피 물가 변화를 통하여 코로나 이후 카페 산업의 소피 패턴 변화를 알아보고자 한다.
### 목표
코로나 팬데믹 이후의 카페 산업의 변화를 파악하고, 커피의 물가 변동과 시장 동향을 통해 외식 업계의 현황을 이해한다.
## ☕ 프로젝트 과정
### 1. 2022년 커피 관련 트렌드 분석
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/crawling/%EC%9B%8C%EB%93%9C_%EC%B9%B4%EC%9A%B4%ED%8A%B8_%EA%B2%B0%EA%B3%BC.png" style="float: left"><br/>
#### 뉴스 크롤링
'커피 물가' 뉴스 워드 클라우드를 통해 이슈들을 살펴본 후, 추가 키워드을 채택하여 크롤링하였다.<br/>
키워드 : 커피 물가, 외식 상승, 스타벅스, 원두 수입
#### 워드 클라우드
2022년에는 커피 물가뿐만 아니라 외식 업계 전반에서 물가 상승 이슈가 있었다. 다수의 커피 프렌차이즈가 가격을 인상했으며, 이 가운데 스타벅스가 이 상승 트렌드를 주도한 것으로 보인다. 급격한 물가 상승 후에는 카페 프렌차이즈들이 자체적으로 상생 협약을 체결하고, 정부도 부가세 면제 정책을 시행하여 불안정한 시장을 안정화하기 위한 다양한 노력을 기울였다.
### 2. 물가 상승으로 인한 커피 시장 변화와 소비 변화
#### 카페 개폐업 수 조사
<img src=""><br/>
커피의 생활물가지수의 변동폭이 컸던 2022년도를 기점으로 2021년부터 2023년까지 카페의 개업 및 폐업 현황 자료를 수집하였다. 서울시로 조사 범위를 한정하여 자료를 조회한 결과, 개업 및 폐업의 전체적인 추이는 상승세였고, 2023년도에 폐업 매장은 2000개 가량 넘는 매장 수를 기록하고, 개업 매장(인허가 받은 매장을 기준으로 함.)은 2500넘는 매장 수를 보이며 더 높은 수치를 기록했다. 더불어, 2021년부터 2023년까지 서울시 내 행정구역별로 범위를 세분화하여 다시 자료를 분류하자, 강남구, 마포구, 송파구, 순으로 개업 매장이 많았고, 강남구, 마포구, 강서구 순으로 폐업 매장 수가 많았다. 커피 물가가 상승한 2022년도에 집중하여 살펴보면, 강남구, 마포구, 송파구 순으로 개업 매장수가 높았으며, 강남구, 마포구, 강서구 순으로 폐업 매장 수가 높아, 동일한 행정구역에서 매년 비슷한 추이가 나타고 있음이 관찰되었다.
#### 일반 외식 식당 개폐업 수 조사
#### 커피 수입량 조사
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/coffee_bean/%EC%9B%90%EB%91%90_%EC%88%98%EC%9E%85%EB%9F%89%EA%B3%BC_%EC%9D%8C%EC%8B%9D%EC%A0%90_%EA%B0%9C%ED%8F%90%EC%97%85_%EC%88%98_%EB%B9%84%EA%B5%90_(2021~2023).png"><br/>


### 3. 활동 인구(종사자수)와 카페 개폐업 간의 관계
## ☕ 프로젝트 결과

