# UI / UX 디자인 구성요소 설계 및 제작

## link : http://tws1.dothome.co.kr/my_weather/

### 기상예보 모바일 웹 & 앱 Project
* **프로젝트 기획 이유?**
  > PC 또는 모바일에 맞춰 반응형 웹사이트를 만들고자 했습니다.
  >
  > 기상예보를 선택한 이유는 PC 또는 모바일에서 손쉽게 접근이 가능하고 원하는 정보를 바로 확인 할 수 있을것 같아 채택했습니다.
  >
  > 또한 외부 data 받아 송수신 할 수 있도록 설계했습니다.  
  
  * **설계**

* **기술스택** 

    <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
    <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white">
    <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=Bootstrap&logoColor=white">
    <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
    <img src="https://img.shields.io/badge/jquery-0769AD?style=for-the-badge&logo=jquery&logoColor=white">
    <img src="https://img.shields.io/badge/json-181717?style=for-the-badge&logo=json&logoColor=white">
    <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">

# 프로젝트 소개 

* **글꼴 및 색상**

    <img src="https://user-images.githubusercontent.com/111415080/219701264-aaaa65da-1b0a-4bdf-8b9e-dee08b11cde9.png" width="50px" height="50px"> 
    
    
  > #33495F : 단일 배경 색상 사용, 하얀색 글자색과 대비 되고 텍스트 정보전달의 목적을 위해 다양한 색상을 사용하지 않았습니다.   
  
    
    <img src="https://user-images.githubusercontent.com/111415080/219701276-e972d61b-a311-4364-b7de-c98897a1700c.png">
    
    
  > Century Gothic 서체, 영문사이트기준으로 기획하였기에 영문에 맞는 고딕계열, 그중에서 좀더 부드럽고 클래식한 느낌의 Century Gothic 을 선택했습니다.
    
* **디자인 구상 및 설계**
  
  ![img2](https://user-images.githubusercontent.com/111415080/219711988-539bb363-1b54-4214-aadf-ec6806fdf00b.PNG)
  
  > 메인페이지 첫 화면에서 현재 날씨 정보를 불러오는걸 목표로 했습니다.  
  >
  > 현재 기온정보, 체감온도, 최고기온 및 최저기온, 풍향 및 강수 예보, 대기질 등 필요한 정보를 최대한 깔끔하게 보일 수 있도록 디자인 구상을 했습니다.  
  
  ![CPT2302180434-992x163](https://user-images.githubusercontent.com/111415080/219772613-d633c856-09d6-4a04-b397-5fb6a27cfcc5.gif)
  
  > 이미지 파일을 이용해 직관적으로 해당 날짜의 날씨 정보를 알 수 있도록 했습니다.
  >
  >  맑은날, 흐린날, 비오는날, 바람부는날등 해당 날씨정보에 따라 이미지파일을 다르게 표현해 한 눈에 알아 볼 수 있게했습니다.

* **기상예보 구현**
 
  ![CPT2302180241-980x701](https://user-images.githubusercontent.com/111415080/219730323-ad9f2034-d0d3-49a1-a53b-caa2c0131752.gif)


  > 첫 화면에서 스크롤을 밑으로 내리면 현재 날씨정보는 상단nav에 고정되고 계속 정보를 확인 가능합니다.
  >
  > 두번째 정보로는 기상 예보입니다. 현재 날짜기준으로 3시간 간격의 5일치 정보를 받아옵니다.
  >
  > 슬라이더로 간략한 날짜 및 시간대에 기온과 날씨를 표기하고 자세한 정보를 보고싶을땐 해당하는 정보를 클릭하게되면 자세한 정보를 밑쪽 detail forecast 란에 표기하게 됩니다.
  
  
* **네비게이션 및 검색**
  
  ![CPT2302180249-980x635](https://user-images.githubusercontent.com/111415080/219744352-9ec9f97c-5707-42c9-8aaf-ec3e4d1b46b7.gif)
  
  > 네비게이션 서치 입니다. 스크롤을 내릴경우 현재 날씨 정보는 상단탑에 고정됩니다.
  >
  > 왼쪽 상단에 메뉴버튼을 누르게되면 사이드 네비게이션이 나타나고 이를 통해 웹페이지의 위치이동이 가능합니다.
  >
  > 또한 검색을 통해 알고싶은 도시의 기상예보로 확인할 수 있도록 구현했습니다.

* **사이드 네비게이션**

  <p align="center"><img src="https://user-images.githubusercontent.com/111415080/219765818-cad62d2b-3831-4b1e-8ec8-c44e37133803.gif"></p>
  
  > 사이드 네비게이션 검색바를 통해 도시 이름을 검색할 수 있습니다.
  >
  > 초기 정보는 KR(한국) 의 seoul(서울) 날씨 정보를 불러옵니다.
  >
  > 검색할 경우 검색한 도시명과 일치하는 도시들만 리스트에 노출이 되고 클릭을 하게되면 해당 도시의 날씨정보 및 기상예보 데이터를 불러옵니다.

* **API 활용**

  > 날씨 관련 데이터를 얻기 위해 openAPI를 활용했습니다.
  > 
  > 데이터를 불러오는 기준은 경도와 위도를 바탕으로 해당 좌표에 있는 국가 및 도시이름의 정보 와 날씨데이터를 불러옵니다.
  > Current Weather (현재날씨) , 3-hour Forecast 5 days (5일간 3시간 간격의 예보), Air Pollution API (대기오염도) 의 data를 사용했고 가장 많은 시간을 할애했습니다.
  > 
  > 이유로는 데이터 처리를 위한 작업과 받은 데이터를 적재적소에 배치해야하는데 하나의 데이터를 여러군데에 배치 및 노출 시켜야 했고 비동기처리를 위한 고민을 많이했습니다.
  > 먼저 현재날씨정보를 두 가지로 나눴습니다. 첫화면에 보여줄 큰 글꼴의 maindata와 상단 nav에 보여줄 정보로 작은 글꼴의 subdata로 나누고 처음에는 maindata만 표기를 합니다.
  > 그 후 스크롤이벤트로 Y축의 기준점을 정하고 스크롤이 해당 기준점을 넘게되면 maindata의 위치를 상단 nav로 옮겨지게되고 subdata를 표기합니다.
  
    <p align="center"><img src="https://user-images.githubusercontent.com/111415080/219784566-daf71680-ffda-4084-b7aa-5e2849030806.gif" width="600"></[>
    <p align="center">스크롤 Y축에 따라 data 표기위치를 다르게 설정</p>

  > json 형태의 정보를 받아오기 위해 &.ajax 메소드를 이용했고 콘솔로그로 체크하면서 작업을 진행했습니다.
  > 
  > 처음에는 객체의 정보를 받아 출력하는데 어려움이 많았습니다. 정확한 객체정보를 받아오기 위해 콘솔디버깅을 많이 했고 data 호출을 위해 함수를 따로 따로 구분해서 작업을 진행했습니다. 그결과 각 함수에서 data작업을 처리하고 바로 데이터를 넘겨 웹상에 표기 시켜줄 수 있었고 원하는 결과를 얻을 수 있었습니다.
  > 
  ```json
  Current Weather
  {
    "coord": {
        "lon": 139.7744,
        "lat": 35.6839
    },
    "weather": [
        {
            "id": 500,
            "main": "Rain",
            "description": "light rain",
            "icon": "10n"
        }
    ],
    "base": "stations",
    "main": {
        "temp": 9.36,
        "feels_like": 8.02,
        "temp_min": 7.77,
        "temp_max": 10.49,
        "pressure": 1013,
        "humidity": 69
    },
    "visibility": 10000,
    "wind": {
        "speed": 2.57,
        "deg": 340
    },
    "rain": {
        "1h": 0.63
    },
    "clouds": {
        "all": 75
    },
    "dt": 1676229651,
    "sys": {
        "type": 2,
        "id": 268395,
        "country": "JP",
        "sunrise": 1676237457,
        "sunset": 1676276370
    },
    "timezone": 32400,
    "id": 1857654,
    "name": "Marunouchi",
    "cod": 200
  }
  ```
<p align="center">json 형태의 data 정보 </p>

* **json 데이터 리스트 활용**

  > 이제 경도와 위도를 바탕으로한 날씨정보를 불러올 수 있었는데 중요한 점은 경도와 위도를 어떻게 불러와야 하는 것 이었습니다.
  > 처음 생각했던 방법은 도시의 위치정보를 api로 받아오는 것이었는데 해외 국가 코드명 및 도시명, 경도 위도 api를 구하기 쉽지 않아 다른방법을 찾아야 했습니다.
  > 고민끝에 내린 결론은 '데이터 파일을 새로 만들자' 였습니다. 전세계 국가명 및 도시명과 경도 위도 데이터를 기반으로 검색한 결과 json 파일을 찾을 수 있었고 이를 바탕으로 
  > 도시명 및 국가명(국가코드)로 리스트를 정리했고 데이터를 받아 올 수 있게 기능구현했습니다.

  ```json
  cities.js
  {
      "country": "GB",
      "name": "Thorngumbald",
      "lat": "53.721",
      "lng": "-0.17175"
    },
    {
      "country": "GB",
      "name": "Thorney",
      "lat": "52.62147",
      "lng": "-0.10815"
    },
    {
      "country": "GB",
      "name": "Thorner",
      "lat": "53.86093",
      "lng": "-1.42676"
    },
    {
      "country": "GB",
      "name": "Thorne",
      "lat": "53.61122",
      "lng": "-0.96308"
    }
  ``` 
  
<p align="center">국가/도시명에 관한 경도, 위도 데이터 리스트</p>

  ```javascript
        <!-- cites data -->
        <script type="module">
            import cities from "./js/cities.js"
            const CITIES_LENGTH = 300
            $(document).ready(function () {
                for (var i = 0; i < CITIES_LENGTH; i++) {
                    $(".country_list").append("<li class='languages'><a href=index.html?lat=" + cities[i].lat + "&lng=" + cities[i].lng + ">(" + cities[i].country +
                    ")" + cities[i].name + "</li>")
                }
            });
        </script>
  ```
  
  <p align="center">국가/도시명 list에 추가</p>


# 프로젝트 후기

  ### 동기
  
  > API 활용하기 위해 날씨 어플 프로젝트를 진행하게되었습니다. 많은 데이터 처리, 비동기화 작업, 실시간 업데이트등 웹개발을 하면서 경험해보지 못했던것들 만들어보고자 했고 부족하지만 원하는 결과물을 만들었던 것 같습니다. data 요청과 호출 값을 객체로 받아오는 과정 및 데이터 표기를 위한 변수 처리 및 함수 사용등 많은 경험을 얻었고 프로젝트를 진행하면서 공부도 많이 됐습니다. 

  ### 아쉬웠던 점
  
  > 어플처럼 다운로드 및 사용 가능하게 PWA 개발을 목표로 했으나 정해진 시일내에 완성을 위해 배제하게 되었습니다. uiux 프로젝트 진행하면서 pc, tablet, mobile 에 맞춰 웹페이지 크기를 조절하면서 작업한다는게 생각보다 많은시간이 걸렸고 데이터 처리과정도 익숙치 않아 많은 시간이 걸렸던거 같습니다. 또한 처음 기획 당시 js파일, css파일등 캡슐화하여 작업 할 계획이었는데 코드를 만들어 갈수록 기능구현에 급급한 나머지 제대로 분리 및 정리가 되지 않았습니다. 

  > 웹페이지 배포를 위한 호스팅작업을 염두해 두고 코드를 만들었지만 막상 호스팅 했을 시 경로 오류나 파일 대소문자오류등 수정해야 할 부분들이 많았습니다. 차후 프로젝트 진행 시 해당사항을 유의하며 작업을 할 것입니다.

# 다음 프로젝트 진행 방향

  ### React & Vue
  
  > 여태까지 바닐라 스크립트로만 작업을 해왔기에 다음 프로젝트로는 react 로 작업을 할 예정입니다. CLI 개발 환경은 구축되어있고 react hook의 개념정리 및 예제 연습등을 통해 어느정도 기초를 쌓은 후 프로젝트 작업을 진행할 것입니다. 생각건대 프로젝트를 진행하면서 공부하는것이 제일 학습에 효율적인거 같습니다. 정해진 기한 없이 작업하는것보다 프로젝트 마감일을 정해두고 계획을 세세하게 나누어 작업을 하고 마감일 기준 일주일 단위 또는 2~3일 단위로 잘게 나누어 정해진 작업을 끝마치는것에 중점을 둬야겠습니다.



# 라이센스
 
  **프로젝트에 사용된 모든 이미지 및 API 정보들은 상업적 목적없이 개인 학습 및 교육으로만 사용했습니다.**  
  
  **참고 사이트 날씨날씨 (https://www.nalssinalssi.com/)     오픈웨더(https://openweathermap.org/)**
