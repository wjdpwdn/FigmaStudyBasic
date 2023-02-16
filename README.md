> 'UIUX를 알았다면 이것도 알아야 한다!( 와이어프레임 VS 프로토타입 )'

# 와이어 프레임 (정적)

제품 기획 단계에서 페이지를 어떻게 구성할 것인지 구조를 잡기위한 목적으로 3단계 레벨을 나누어 제작한다.

![스크린샷 2023-02-16 오후 9 24 49](https://user-images.githubusercontent.com/102521448/219363997-516ef985-44c7-4829-b4f0-48432057019c.png)

### 1. Lo-Fi
아이디어를 구체화 시키며 큰 그림을 잡을 때 사용한다.
선과 틀로 레이아웃을 설계해가기 때문에 수정이 용이하다.

### 2. Mid-Fi
와이어 프레임을 봤을때 해당 페이지가 어떻게 작동하게 될 지 예상 가능한 퀄리티로 lofi에서 업그레이드 시킨다.

### 3. Hi-Fi
이 레벨부터 mockup에 가까운 퀄리티 이기때문에 시간이 오래 걸린다.
따라서 와이어프레임 단계에서는 hifi까지 가지 않는다.
(단, 고객사가 원할경우 갈수도? 있다..)

# 프로토 타입 (동적)
와이어 프레임단계에서 lofi 혹은 midfi 단계를 거치면 프로토타입 단계로 오게된다.

### 1. Lo-Fi
구체적이 내용은 없는 상태로, 간단한 상호작용 / 페이지 이동 정도만 테스트 하는 단계
UserFlow 상에서 어색한 기능, 페이지가 없는지 빠르게 검토가 가능하다.

### 2. Mid-Fi
최종결과물과 거의 유사한 단계이다. 개발단계에 들어서기전 프로토타입 midFi를 걸쳐 개발비용 절감과 시간을 절약할 수 있다.

### 3. Hi-Fi
이 단계는 매우 optical 한 단계이다. 사실 midfi랑 큰차이도 없기 때문에 midfi에서 퀄리티가 더 높은 단계라고 봐도 무방하다.


> 와이어프레임과 프로토타입 제작이 가능한 Tool.. 그것은 Figma

# 피그마 짱이구마

![figma_thumbnail](https://user-images.githubusercontent.com/102521448/219366863-471421ad-1a33-40ae-8283-071ebb2f8bd4.png)

## 피그마 컴포넌트, 프레임만 알면 다 안거다.

### 컴포넌트

피그마에는 react, javascipt 처럼 컴포넌트 그리고 인스턴스의 개념이 있다
컴포넌트는 원본이 되며 인스턴스는 컴포넌트의 복제 품이다

컴포넌트 안에서 링크를 연결하고, hover의 기능등을 추가하여 단순 정적에서 동적 프레임워크로 변경이 가능하다.

### 프레임

프레임은 스마트폰을 생각하면 쉽다
한뼘의 디스플레이에서 아래로 내리면 스크롤이, 옆으로 쓸으면 새로운 이미지가 나온다.

## 모달, 토글, 탭, 아코디언은 비교적 제작하기 쉬운 UI 요소 이다.


### 모달
![modal](https://user-images.githubusercontent.com/102521448/219388910-c0dd141d-6b9b-4419-aa0d-3c44c4ec4032.gif)
<img width="455" alt="스크린샷 2023-02-16 오후 11 19 17" src="https://user-images.githubusercontent.com/102521448/219389858-a16918d6-4b72-4e51-ba6f-7a45ab55a52f.png"> <br>
modal 컴포넌트 와 close버튼의 frame에 연결 되어있다.
modal 컴포넌트 내부에는 hover시에 진해지는 기능과 클릭시에 frame6가 열리도록 하였다.
frame6는 모달창으로, 클릭시에 꺼지도록 하였다.

### 토글
![toggle](https://user-images.githubusercontent.com/102521448/219388205-2ef23469-28db-4f24-b06c-534b9eab0814.gif)
<img width="187" alt="스크린샷 2023-02-16 오후 11 22 47" src="https://user-images.githubusercontent.com/102521448/219390782-1a92b133-3964-4861-8064-d20fb261f840.png"> <br>
토글 컴포넌트안에 기본형태와 토글을 켰을때, 총 2개의 버튼이 있다.
smart animation으로 설정해두면 위의 영상처럼 자연스럽게 버튼이 이동하도록 보인다.

### 탭
![tab](https://user-images.githubusercontent.com/102521448/219388873-95af278a-048e-4441-bd60-e70f183e4106.gif)
<img width="518" alt="스크린샷 2023-02-16 오후 11 33 13" src="https://user-images.githubusercontent.com/102521448/219393555-a1987958-94df-48ec-828e-c33c858ac8ed.png"> <br>
tab의 버튼이 담긴 component3 와, tab 자체의 component6 이있다. componnent3는 hover가 담긴 버튼이며
component6은 tab 내용과 compoment3의 버튼을 이용한 컴포넌트 이다.
component3의 hover 버튼과 누르면 내용이 봐뀌는 component 6을 적용시켜 tab을 완성시켰다.

### 아코디언
![accor](https://user-images.githubusercontent.com/102521448/219388975-0322f4bb-a322-4bc2-8169-8fbecf14de85.gif)
<img width="310" alt="스크린샷 2023-02-16 오후 11 36 44" src="https://user-images.githubusercontent.com/102521448/219394462-e09b9b8a-2dcf-429a-9186-ef534a5115d8.png">  <br>
화살표 버튼으로 열고 닫고 작동하도록 하였다.아코디언또한 smart animation을 사용하면 자연스러운 아코디언 제작이 가능하다.
