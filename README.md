<div align="center">

<h1>Project ROKC</h1>

</div>

## 0. Overview

해당 프로젝트는 Knowledge graph, knowledge inference 관련으로 강의 영상에서 정보를 생성하여 다루는 서비스의 집합입니다.


## 1. Reasoning_over_Knowledge_Component_Streams

https://github.com/BonhyeonGu/Reasoning_over_Knowledge_Component_Streams

<div align="center">

![d](https://img.shields.io/badge/-Python3-3776AB?style=flat-square&logo=python&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Flask-000000?style=flat-square&logo=flask&logoColor=FFFFFF)  ![d](https://img.shields.io/badge/-Javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=FFFFFF) 

![z1](https://user-images.githubusercontent.com/24387014/209905568-c3955e29-59c7-46c9-8d49-6be6adf2af73.gif)

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

![d](https://img.shields.io/badge/-Python3-3776AB?style=flat-square&logo=python&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=FFFFFF) ![d](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=Mongodb&logoColor=FFFFFF)  ![d](https://img.shields.io/badge/-Javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=FFFFFF)

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
