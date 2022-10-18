<p align="middle" >
  <img width="200px;" src="https://github.com/woowacourse/javascript-baseball-precourse/blob/main/images/baseball_icon.png?raw=true"/>
</p>
<h1 align="middle">숫자 야구 게임</h1>

## 🔍 진행방식

- 미션은 **기능 요구사항, 프로그래밍 요구사항, 과제 진행 요구사항** 세 가지로 구성되어 있다.
- 세 개의 요구사항을 만족하기 위해 노력한다. 특히 기능을 구현하기 전에 기능 목록을 만들고, 기능 단위로 커밋 하는 방식으로 진행한다.

---
## 🎯 기능 요구사항

기본적으로 1부터 9까지 서로 다른 수로 이루어진 3자리의 수를 맞추는 게임이다.

- 같은 수가 같은 자리에 있으면 `스트라이크`, 다른 자리에 있으면 `볼`, 같은 수가 전혀 없으면 `낫싱`이란 힌트를 얻고, 그 힌트를 이용해서 먼저 상대방(컴퓨터)의 수를 맞추면 승리한다.
  - 예) 상대방(컴퓨터)의 수가 425일 때
     - 123을 제시한 경우 : 1스트라이크
     - 456을 제시한 경우 : 1볼 1스트라이크
     - 789를 제시한 경우 : 낫싱
- 위 숫자 야구게임에서 상대방의 역할을 컴퓨터가 한다. 컴퓨터는 1에서 9까지 서로 다른 임의의 수 3개를 선택한다. 게임 플레이어는 컴퓨터가 생각하고 있는 3개의 숫자를 입력하고, 컴퓨터는 입력한 숫자에 대한 결과를 출력한다.
- 이 같은 과정을 반복해 컴퓨터가 선택한 3개의 숫자를 모두 맞히면 게임이 종료되고, 재시작 버튼이 노출된다.
- 게임이 종료된 후 재시작 버튼을 클릭해 게임을 다시 시작할 수 있다.
- 사용자가 잘못된 값을 입력한 경우 `alert`으로 에러 메시지를 보여주고, 다시 입력할 수 있게 한다.

---
## 💻 기능 구현 목록
- 3자리의 랜덤 값 생성 후 array에 저장
  - 3자리의 숫자를 랜덤하게 생성
  - 해당 숫자들은 중복될 수 없음

- Input 값을 받아 유효성 확인
  - Input 값을 string -> array로 변경
  - Input Array의 글자 수 확인
  - 각 숫자가 허용되는 범위 내의 수인지 확인
  - 각 숫자가 중복되는지 확인
  - 조건을 만족시키지 못하면 alert로 에러 메시지 출력 후 재입력

- 랜덤 값과 Input 값 비교
  - 같은 수가 같은 자리에 있는 경우 : 스트라이크
  - 같은 수가 다른 자리에 있는 경우 : 볼
  - 같은 수가 없는 경우 : 낫싱
  - 3자리의 정답을 맞췄을 경우 : 정답 출력

- 재시작 버튼 구현
  - 재시작 버튼 클릭시 새로운 랜덤 숫자 생성

---

## ✔ 결과

![image-20221019001612752](./README.assets/image-20221019001612752.png)
