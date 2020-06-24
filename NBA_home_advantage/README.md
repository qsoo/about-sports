# about-sports

Things I've done for fun
### NBA homecourt advantage 분석

---------------------------------
##### 0.Introduction

##### 취미로 즐겨하던 농구에서 응원을 받으면 평소보다 더 잘되는 것 같은 느낌이 항상 있었습니다. 여기에 더해서 대회를 참여할 때면 익숙한 코트에서는 더 성적이 잘 나왔던 경험이 있습니다. 여기서 출발하여 진짜 홈코트 어드밴티지가 있는지 살펴보고자 분석을 실시하였습니다. NBA나 KBL할 것 없이 모든 프로스포츠에서는 playoff가 되면 홈코트어드밴티지를 얻기 위해 정규시즌 성적을 잘 거두기 위해 노력하고 있기에 실제로 홈코트 어드밴티지는 적용되는지, 그리고 그중 응원이 가진 힘이 실제로 존재하는지 밝히고자 하는 것이 가장 큰 목표입니다.



---

##### 분석에 사용한 데이터는 NBA league에 참여하고 있는 LA Lakers와 LA Clippers가 주요 데이터이며 이 두팀이 같은 코트를 사용한 1999-2000 season부터 2018-2019 season까지의 Game Log를 사용하였으며 이를 통해 원정 거리, 숙소 등의 기타 변수를 제외하고 응원이라는 한 변수만을 집중적으로 분석할 수 있을 것이라 생각합니다.


---

##### 첫 Raw data로 이용하였던 자료인 LAclippers.csv는 기준 팀으로 삼은 LA Clippers의 매 시즌 게임 결과를 이용하였습니다. 허나 추후에 시즌이 2년에 걸쳐져서 기록이 되어있기 때문에 분석과정에서 문제가 발생하였고 이를 수정하기 위해 새로운 raw data를 사용하였습니다.

---
##### *참고사항
##### NBA의 한 시즌 정규리그 경기는 총 82경기이며, 단축시즌인 11-12(66경기)를 제외하고는 82경기로 이뤄져 있습니다. 경기 스케쥴은 시즌마다 상이하나 일반적으로

##### 다른 컨퍼런스 15개 팀과 2경기 = 30경기

##### 같은 지구 4개 팀과 4경기 = 16경기

##### 같은 컨퍼런스 다른 지구 10개 팀 중 6개 팀과 4경기 =24경기

##### 같은 컨퍼런스 다른 지구 10개 팀 중 나머지 4개 팀과 3경기 =12경기

##### 이렇게 해서 총 82경기가 구성되어집니다.

##### 데이터 중 팀명이 변경된 경우가 있으며

##### Charlotte Bobcats = Charlotte Hornets  
##### Vancouver Grizzlies = Memphis Grizzlies  
##### New Orleans Hornets = New Orleans Pelicans  
##### New Jersey Nets = Brooklyn Nets  
##### New Orleans/Oklahoma City Hornets, Seattle SuperSonics =   Oklahoma City Thunder
  ##### 로 처리하였습니다(최근 팀명)
