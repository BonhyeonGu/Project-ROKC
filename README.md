<div align="center">

<h1>Project ROKC</h1>

</div>

## 0. Overview

### Info
해당 프로젝트는 Knowledge graph, knowledge inference 관련으로 강의 영상에서 정보를 생성하여 다루는 서비스의 집합입니다.

해당 reposit에서 모두 실행할 수 있는 도커 컴포즈를 지원하며 요구 사양은 아래와 같습니다. (준비중)

### Install & Run
```bash
git clone https://github.com/BonhyeonGu/Project-ROKC rokc
cd rokc
docker-compose up
```
이후 zol1 에서 "Ready to ROKCS"가 출력되면  
Reasoning_over_Knowledge_Component_Streams 서비스를 이용하실 수 있습니다.    

그리고 zol2 에서 "Ready to ShowPoolWeb"가 출력되면 ShowPoolWeb 서비스를 이용하실 수 있습니다.    
해당 출력은 순서가 상이할 수 있습니다.

각 웹 서비스는 Reasoning_over_Knowledge_Component_Streams 가 http://127.0.0.1:5050  
ShowPoolWeb 는 http://127.0.0.1:5051 로 접속이 가능합니다.
  
## 1. Reasoning_over_Knowledge_Component_Streams

https://github.com/BonhyeonGu/Reasoning_over_Knowledge_Component_Streams

<div align="center">

![d](https://img.shields.io/badge/-Python3-3776AB?style=flat-square&logo=python&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Flask-000000?style=flat-square&logo=flask&logoColor=FFFFFF)  ![d](https://img.shields.io/badge/-Javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=FFFFFF) 

![01_Over](https://user-images.githubusercontent.com/24387014/184350904-12adecf5-0adb-498d-922d-a8c8da9bf513.gif)

</div>

유튜브 URL을 입력하면 주제 컴포넌트를 출력할 수 있는 서비스입니다. 여러 선택지가 주어집니다.


## 2. PoolMaker_Youtube_KnowledgeGraph

https://github.com/BonhyeonGu/PoolMaker_Youtube_KnowledgeGraph

<div align="center">

![d](https://img.shields.io/badge/-Python3-3776AB?style=flat-square&logo=python&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=FFFFFF)  

</div>

*Reasoning_over_Knowledge_Component_Streams* 의 기능을 Neo4j DB에 넣을 수 있게 작성된 서비스입니다.


## 3. ShowPoolWeb_Youtube_KnowledgeGraph

https://github.com/BonhyeonGu/ShowPoolWeb_Youtube_KnowledgeGraph

<div align="center">

![d](https://img.shields.io/badge/-Python3-3776AB?style=flat-square&logo=python&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Flask-000000?style=flat-square&logo=flask&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=Mongodb&logoColor=FFFFFF)  

![03](https://user-images.githubusercontent.com/24387014/209906492-20388a10-0910-40ea-8050-1051c69b349d.gif)

</div>

Neo4j DB에 올라간 정보들을 유저들에게 가시화 할 목적으로 제작된 웹 서비스 입니다.
해당 서비스는 *ShowPoolWeb_Recommendation* 서비스가 동작해야 모든 기능을 확인할 수 있습니다.


## 4. ShowPoolWeb_Recommendation

https://github.com/BonhyeonGu/ShowPoolWeb_Recommendation

<div align="center">

![d](https://img.shields.io/badge/-Python3-3776AB?style=flat-square&logo=python&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=Mongodb&logoColor=FFFFFF)  

</div>

ShowPoolWeb_Youtube_KnowledgeGraph 서비스의 사용자 유저를 통해 영상 추천을 시행하는 서비스입니다.
해당 서비스는 Mongo DB 또는 *ShowPoolWeb_Youtube_KnowledgeGraph* 로 출력을 확인할 수 있습니다.
