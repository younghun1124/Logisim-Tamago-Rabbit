# Logisim-Tamago-Rabbit
Seoul National University of Science and Technology(SeoulTech)'s second-year digital logic circuit class project.
This project received the highest overall score.
## 작동법
If you hit the Hit button one after another, Pet's experience level increases. You can start from the beginning by pressing the reset button.
![image](https://github.com/user-attachments/assets/d1287451-36af-46bd-a69c-e60f4337e662)

[Watch cute rabbit!](https://github.com/younghun1124/Logisim-Tamago-Rabbit/files/7804759/_poster.pdf)


## 프로젝트 수행 중 부딪힌 문제들과 해결 방법, 끝내 해결하지 못한 부분
### 문제 1-1 : 랜덤으로 올라갈 경험치를 생성하는 모듈을 만들었는데, 그 값에는 0도 포함되어있어 버튼을 눌러도 경험치가 오르지 않는 경우가 있었다.

해결방법 : 랜덤 경험치 값에 1을 더하여 0이 나오지 않게 함. 
 
### 문제 1-2 : 랜덤 경험치 값에 1을 더했더니 이제는 오버플로가 일어나서 1111값이 0으로 표시되게 되었다.

해결방법 : XOR Gate를 이용하여 0000값일 때 0001값을 전달하도록 수정

### 문제 2: Led 매트릭스 상에 데이터를 전송할 때 각각의 문자를 모듈화 하여 만들었더니 글자가 겹쳐 보이는 문제가 생겼다. 

해결방법 : bit shift를 이용해 글자들을 밀어주었다.

### 문제 3 : 화면에 표시될 element가 많아지다 보니 일일이 element를 합성해주는 것이 정말 작업량이 많았다.

해결방법 : 화면에 표시될 정보들을 or 연산으로 합쳐서 출력해주는 모듈을 만들었다. 또한 모듈의 외형적 크기를 수정하여 다른 모듈들과 바로 붙여서 연결할 수 있게 하였다.

### 문제 4 : splitter를 이용해 선 연결을 간소화 하려고 하였는데(LED 매트릭스에 표시될 부분이 처음에는 60x50 사이즈로 총 3000비트였다) splitter가 나를 수 있는 비트의 수가 그렇게 많지 않아서 수많은 비트를 터널을 이용해 합성하고 연결해야 했다.

해결방법 : 로지심 내에서 회로의 인풋과 아웃풋 위치를 적절히 배열하여 선 한 개로 이을 수 있게 하였다.마우스 드래그 한번으로 여러 개의 값을 전달할 수 있었다.

## 프로젝트 수행 중 새롭게 배운 점
아날로그 조이스틱의 원리 : 최종 완성본에 포함된 기능은 아니지만 게임 내 캐릭터를 이동하는 것을 구현해보던 중 아날로그 조이스틱이 정보를 전달하는 원리를 알게 되었다. LED 매트릭스 상에 아날로그 조이스틱을 움직일 때마다 다른 패턴의 무늬가 나오는 것이 신기했다.
모듈화의 중요성과 설계의 중요성 : 최대한 확장이 용이한 구조로 회로를 만들려고 했고 생각도 많이 했지만, 실제로 회로를 만들다 보니 새롭게 기능 하나 넣을 때마다 회로를 뜯어고쳐야 했다. 

## 프로젝트를 수행하며 느낀 점과 앞으로의 각오 (감정적인 부분)
일단 최종 결과물이 나름 만족스럽게 나온 것 같다. 토끼도 귀엽고. 
처음 계획에는 여러가지 효과나 이벤트들도 추가해 주려고 했지만 주제 특성상 반복되는 작업이 많았어서 그럴 시간이 충분하지 않았다. 앞으로 프로젝트를 할때는 디테일에 너무 신경쓰기보단 다양한 아이디어들을 구현해 보는데 집중해야겠다고 생각했다. 공책에 픽셀을 그려보며 숫자와 그림이 어떤 생김새를 가질 지 고민하는 것이 즐거웠다. 시험공부 하다가 지칠 때 간간히 하기 좋았다.
