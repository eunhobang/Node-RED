# Node-RED

https://wikidocs.net/16814

### Node.js 설치
  https://nodejs.org/ko/
  * LTS로 다운로드 받기

### Node-RED 명령어 설치

  맥/우분투
  
    sudo npm install -g node-red
    * 안 될 경우: sudo apt install npm 입력 후 설치
    
  윈도우
  
    npm install -g node-red 
  
  
## Node-RED 실행
  모든 OS
  
    node-red
  
## Node-RED 접속
  크롬에서 "localhost:1880" 입력하여 접속
  
## Node-RED 화면 구성

![그림1](https://user-images.githubusercontent.com/80435502/147364279-93600011-b0e8-4631-97cc-93546acb4fa3.png)
  파레트
  - 우리가 Node RED에서 사용할 수 있는 노드들이 나열되어있습니다. 나중에 다른 노드들을 설치를 통하여 추가할 수 있습니다.
  
  작업 공간
  - 파레트에서 노드를 드래그하여 놓는 곳입니다. 우리가 구현할 시스템을 작업하는 곳입니다.
  
  사이드 바
  - 노드에 대한 정보, 노드 간에 전달되는 데이터(메시지)가 표시됩니다. 에러 메시지도 이곳을 통해 확인할 수 있으며, 추가 설치를 통해 사이드 바 기능을 확장할 수 있습니다.


### Node-RED 명령어
  접속
    node-red

  정지
    node-stop
    
  재시작
    node-red-start
  
  
### 노드 종류
1. 입력노드: 시작 신호 담당
2. 출력노드: 최종 처리 노드
3. 활용노드
  - 입력과 출력 노드 사이에 연결되어 데이터를 가공하거나 제어하는 노드(함수노드 포함)
  - 내가 원하는 대로 메시지를 조작하거나 정답 또는 오류처리를 작업할 수 있음

## 노드 연결
  입력노드-(활용노드)-출력노드
  
## msg 객체
  - 각 노드들은 반드시 링크를 통해 정보를 전달하며 이 데이터가 msg이다.
  ![msg구조](https://user-images.githubusercontent.com/80435502/147436918-9f40ed4b-2590-4bdf-b467-5e1a94dea417.png)

## postgresql 연동
  - 터미널 설치
     sudo npm install node-red-contrib-re-postgres
  - 팔레트에서 설치(추천)
    
