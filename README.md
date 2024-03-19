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

Colab : 공공데이터포털 데이터 전처리 및 시각화<br/>
JupyterLab : 네이버 뉴스 크롤링,<br/>
Hadoop, Hive, Sqoop, MySQL : 일반음식점과 휴게음식점 데이터 분석<br/>
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
## ☕ 프로젝트 과정 및 분석 결과
### 1. 2022년 커피 관련 트렌드 분석
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/crawling/%EC%9B%8C%EB%93%9C_%EC%B9%B4%EC%9A%B4%ED%8A%B8_%EA%B2%B0%EA%B3%BC.png" style="float: left"><br/>
#### 뉴스 크롤링
'커피 물가' 뉴스 워드 클라우드를 통해 이슈들을 살펴본 후, 추가 키워드을 채택하여 크롤링하였다.<br/>
키워드 : 커피 물가, 외식 상승, 스타벅스, 원두 수입
#### 워드 클라우드
2022년에는 커피 물가뿐만 아니라 외식 업계 전반에서 물가 상승 이슈가 있었다. 다수의 커피 프렌차이즈가 가격을 인상했으며, 이 가운데 스타벅스가 이 상승 트렌드를 주도한 것으로 보인다. 급격한 물가 상승 후에는 카페 프렌차이즈들이 자체적으로 상생 협약을 체결하고, 정부도 부가세 면제 정책을 시행하여 불안정한 시장을 안정화하기 위한 다양한 노력을 기울였다.
### 2. 커피 물가 상승으로 인한 카페 시장 변화
#### 2022년 카페 개업 현황 지도 시각화
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/map/restarants_open_map.png">

#### 2022년 카페 폐업 현황 지도 시각화
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/map/restarants_closed_map.png">

#### 카페 개폐업 수 조사
<div>
  <img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/cafe/1_%EC%84%9C%EC%9A%B8%EC%8B%9C_%EC%A0%84%EC%B2%B4_2021%EB%85%84%EB%B6%80%ED%84%B0_2023%EB%85%84%EA%B9%8C%EC%A7%80_%ED%8F%90%EC%97%85_%EC%B9%B4%ED%8E%98_%EC%97%B0%EB%8F%84%EB%B3%84_%EB%B6%84%ED%8F%AC.png" width="500">
  <img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/cafe/2_%EC%84%9C%EC%9A%B8%EC%8B%9C_%EC%A0%84%EC%B2%B4_2021%EB%85%84%EB%B6%80%ED%84%B0_2023%EB%85%84%EA%B9%8C%EC%A7%80_%EC%9D%B8%ED%97%88%EA%B0%80_%EC%B9%B4%ED%8E%98_%EC%97%B0%EB%8F%84%EB%B3%84_%EB%B6%84%ED%8F%AC.png" width="500>
</div>
    
커피의 생활물가지수의 변동폭이 컸던 2022년도를 기점으로 2021년부터 2023년까지 카페의 개업 및 폐업 현황 자료를 수집하였다.  서울시로 조사 범위를 한정하여 자료를 조회한 결과, 개업 및 폐업의 전체적인 추이는 상승세였고, 2023년도에 폐업 매장은 2000개 가량 넘는 매장 수를 기록하고, 개업 매장(인허가 받은 매장을 기준으로 함.)은 2500넘는 매장 수를 보이며 더 높은 수치를 기록했다.


<div>
  <img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/cafe/3_%EC%84%9C%EC%9A%B8%EC%8B%9C_2021%EB%85%84%EB%B6%80%ED%84%B0_2023%EB%85%84%EA%B9%8C%EC%A7%80_%ED%8F%90%EC%97%85_%EC%B9%B4%ED%8E%98_%ED%96%89%EC%A0%95%EA%B5%AC%EC%97%AD%EB%B3%84_%EB%B6%84%ED%8F%AC.png" width="500">
  <img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/cafe/4_%EC%84%9C%EC%9A%B8%EC%8B%9C_2021%EB%85%84%EB%B6%80%ED%84%B0_2023%EB%85%84%EA%B9%8C%EC%A7%80_%EC%9D%B8%ED%97%88%EA%B0%80_%EC%B9%B4%ED%8E%98_%ED%96%89%EC%A0%95%EA%B5%AC%EC%97%AD%EB%B3%84_%EB%B6%84%ED%8F%AC.png" width="500">
</div>

더불어, 2021년부터 2023년까지 서울시 내 행정구역별로 범위를 세분화하여 다시 자료를 분류한 결과이다. <br/>
개업 매장 수 : 강남구 > 마포구 > 송파구<br/>
폐업 매장 수 : 강남구 > 마포구 > 강서구<br/>

<div>
  <img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/cafe/6_%EC%84%9C%EC%9A%B8%EC%8B%9C_2022%EB%85%84_%EC%9D%B8%ED%97%88%EA%B0%80_%EC%B9%B4%ED%8E%98_%ED%96%89%EC%A0%95%EA%B5%AC%EC%97%AD%EB%B3%84_%EB%B6%84%ED%8F%AC.png" width="500">
  <img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/cafe/5_%EC%84%9C%EC%9A%B8%EC%8B%9C_2022%EB%85%84_%ED%8F%90%EC%97%85_%EC%B9%B4%ED%8E%98_%ED%96%89%EC%A0%95%EA%B5%AC%EC%97%AD%EB%B3%84_%EB%B6%84%ED%8F%AC.png" width="500">
</div>

커피 물가가 상승한 2022년도에 집중하여 살펴보면, 강남구, 마포구, 송파구 순으로 개업 매장수가 높았으며, 강남구, 마포구, 강서구 순으로 폐업 매장 수가 높아, 동일한 행정구역에서 매년 비슷한 추이가 나타고 있음이 관찰되었다.<br/>

#### 활동 인구(종사자수)와 카페 개폐업 간의 관계
서울시 행정구 별 카페 개폐업 수 비교
사업체가 많은 곳에 소비자(회사원)가 많은 지역일수록 커피 소비가 꾸준히 이루어져 물가 상승과 상관없이 안정적인 카페 시장을 유지하는 경향이 있을 것으로 추측하여, 종사자수 상위 5곳을 선정하여 행정구 별로 종사자 수와 카페 개폐업 수를 비교해보았다.
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/coffee_bean/%ED%96%89%EC%A0%95%EA%B5%AC%EC%97%AD%EB%B3%84_%EC%A2%85%EC%82%AC%EC%9E%90%EC%88%98_top5.png">
**강남구, 송파구**<br/>
카페 개폐업 수: 폐업 수가 개업 수에 비해 높은 경향이 있음.<br/>
**서초구, 중구**<br/>
카페 개폐업 수: 폐업과 개업이 모두 적은 편임.<br/>
**영등포구**<br/>
카페 개폐업 수: 개업이 폐업보다 많은 편임.<br/>

### 3. 일반 외식 식당 개폐업 수 조사
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/coffee_bean/%EC%9B%90%EB%91%90_%EC%88%98%EC%9E%85%EB%9F%89%EA%B3%BC_%EC%9D%8C%EC%8B%9D%EC%A0%90_%EA%B0%9C%ED%8F%90%EC%97%85_%EC%88%98_%EB%B9%84%EA%B5%90_(2021~2023).png"><br/>
그렇다면, 카페 이외에 외식 산업에도 변화가 있었는지 살펴보자.<br/> 
2022년도를 기준으로 서울시 내 일반 음식점의 개폐업 매장 수를 보니, 개업 및 폐업 매장 모두 전반적으로 상승세를 보이고 있으나, 폐업 매장이 개업 매장보다 더 변화 폭이 큰 그래프가 그려지고 있음이 보인다. 특히, 2월에는 개업매장이 최하점을 찍고 있고, 12월에는 폐업 매장이 최고점을 찍고 있다. 이러한 결과를 바탕으로 커피를 비롯한 외식비 상승으로 인한 영향이 음식점의 개업 및 폐업에도 영향을 미치고 있음이 보여진다. 
### 4. 커피 수입량 조사
#### 원두 수입량과 카페와 음식점 개폐업의 관계
원두 수입량을 기준으로 커피 소비량을 가정하였을 때, 커피의 소비량이 카페의 개폐업에 미치는 영향을 살펴보자. 원두의 수입량은 폐업 매장과 개업 매장과 전반적으로 비례하는 그래프를 그리고 있다. 커피의 소비는 매장의 개업 및 폐업에 큰 영향을 받지 않고 꾸준하게 이루어지고 있음을 볼 수 있다. 일반음식점의 경우, 개폐업의 수치가 대체적으로 원두 수입량보다 더 낮은 수치를 보인다. 더불어, 개업 및 폐업의 변화가 원두의 수입량보다 더 변화폭이 큰 것으로 보여진다.
#### 원두 수입량
<img src="https://github.com/pladata-encore/DE30-4-coffeePrice/blob/main/3.img/visualization/coffee_bean/%EA%B3%84%EC%A0%88%EC%97%90%20%EB%94%B0%EB%A5%B8%20%EC%9B%90%EB%91%90%20%EC%88%98%EC%9E%85%EB%9F%89%20%EB%B9%84%EA%B5%90(2021~2023).png">
커피 소비량 데이터를 찾고자 하였으나, 현실적으로 관련 데이터 수집이 어려워, 고안해낸 방법이 원두 수입량 데이터가 원두 수입량과 비슷할 것이라고 생각되어, 원두 수입량 데이터를 수집하여 분석하였다. 하지만 원두 수입량 데이터 기반으로 분석을 하였을 때, 원두 수입량과 커피소비량이 비례하지 않았고 관련성이 떨어져 있는 것으로 보였다. 원두 수입량은 수확 계절에 영향을 많이 받는다는 것으로 판단이 되었고,
그에 해당한 계절에 따른 원두 수입량 데이터를 분석해 보았다.
계절에 따른 원수 수입량 그래프를 2021년~ 2023년, 3년동안 데이터를 분석했을 때, 주로 5월, 9월에 수입량이 다른 시즌보다 현저히 떨어지는 것으로 보인다.

## ☕ 프로젝트 결론
### 물가 상승과 카페 개폐업 간의 관계
2022년에는 커피 물가를 포함한 외식 업계 전반에서 물가 상승 이슈가 있었다.
종사자수가 많다고 해서 카페 시장이 안정적으로 유지되지는 않았다. 지표가 안정적인 행정구도 있었지만 폐업 수가 더욱 많은 행정구들도 있었는데, 이는 코로나로 인한 재택 근무가 증가하면서 소비량이 줄어 카페 폐업 수가 늘어났을 것으로 추측된다.
### 물가 상승과 원두 수입량
위 분석 결과를 토대로 커피 가격이 상승하였음에도 원두 수입량 및 카페의 개업 수치는 증가하고 있음으로 보아, 서울시 내 커피 소비량은 계속해서 증가할 것으로 보여진다. 커피 가격의 상승으로 인해 일시적으로 카페의 폐업에 영향을 주었으나, 점진적으로 하락세인 것이 관찰되며, 음식점의 폐업 수치보다 완만하게 변화를 보이고 있다. 이로 인해, 외식비 상승으로 인한 일반 음식점에 대한 개업 및 폐업의 변화폭은 크지만, 커피 가격 상승으로 인한 카페 분포의 변화는 보다 적을 것으로 보인다. <br/>
또한, 원두 수입량은 커피 소비량과의 관계보다는 수확 계절에 영향을 많이 받는다는 사실을 알게 되었다. 데이터 수집에 있어서, 어떻게 데이터를 수집, 확보 할 것인지 또한 이 데이터가 분석하고자 하는 주제에 관련성이 얼마나 있는지 분석해내고, 알아내는 능력도 중요함을 느꼈다.


