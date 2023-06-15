
# 잡았다 소음!  👋


 [![android](/profile/마스코트.png)](https://drive.google.com/file/d/1rRvhvFjUJRRTOW-yiM6hZ4_TpH39x9fd/view?usp=sharing)


#  [ 프로젝트 개요 ]


| 항목      | 내용                              |
|---------|---------------------------------|
| **프로젝트소개**  | 생활속의 소음트러블을 해소하기위한 서비스          |
| **구성인원**    | 기획자 1명, 디자이너 1명,안드로이드 1명, FE 1명, BE 1명          |
| **개발기간**    | 총 20일 (2023-05-23 ~ 2023-06-13) |
| **성과 및 결과** | 기한내 목표한 기능구현완료 ,CI/CD 파이프라인 구축 배포완료 |


# [ 프로젝트 소개 ]

## 1. 사용기술 📚
<div align="center">
 <span>
  <img src="https://img.shields.io/badge/android-3DDC84?style=flat-square&logo=android&logoColor=white"/> 
     <img src="https://img.shields.io/badge/kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white"/> 
 </span>
 <br>
  <span>
    <img src="https://img.shields.io/badge/python-3776AB?style=flat-square&logo=python&logoColor=white"/>
    <img src="https://img.shields.io/badge/tensorflow-FF6F00?style=flat&logo=tensorflow&logoColor=white"/> 
  </span>
   <br>
   <span>
   <img src="https://img.shields.io/badge/react-61DAFB?style=flat-square&logo=react&logoColor=white"/>
   <img src="https://img.shields.io/badge/reactrouter-CA4245?style=flat&logo=reactrouter&logoColor=white"/> 
   <img src="https://img.shields.io/badge/axios-5A29E4?style=flat&logo=axios&logoColor=white"/> 
   <img src="https://img.shields.io/badge/vercel-000000?style=flat&logo=vercel&logoColor=white"/> 
</span>
  <br>
  <span>
  <img src="https://img.shields.io/badge/springboot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/gradle-02303A?style=flat-square&logo=gradle&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=OpenJDK&logoColor=white"/>
  <img src="https://img.shields.io/badge/mysql-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/amazonrds-527FFF?style=flat&logo=amazonrds&logoColor=white"/>
</span>
<br>
<span>
  <img src="https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white"/>
  <img src="https://img.shields.io/badge/amazonec2-FF9900?style=flat&logo=amazonec2&logoColor=white"/>
  <img src="https://img.shields.io/badge/amazons3-569A31?style=flat-square&logo=amazons3&logoColor=white"/>
  <img src="https://img.shields.io/badge/github-181717?style=flat&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/githubactions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
</span>
  <br>

</div>
                

## 2. 아키텍처 🔔
<div align="center">
<img src="https://github.com/Greenie-crew/.github/assets/71303448/7c894022-9677-4202-8762-0fdc0b378e6a"  width="600" >
</div>

## 3. 백엔드 ERD 및 와이어 프레임 🛠
<div align="center">
  <img align="center" src="https://github.com/Greenie-crew/.github/assets/71303448/c36a9033-0c2c-4434-b471-3b62cc558753" width="600">
</div><br>

### [ 와이어프레임 ]   [ Figma ](https://www.figma.com/file/D1FJxm69kI0QDLSWs0adiG/Greenie-%EC%9E%A1%EC%95%98%EB%8B%A4!-%EC%86%8C%EC%9D%8C?type=design&node-id=0%3A1&t=o3BrwVucKr5HeBse-1)

### [ 백엔드 ERD ]  [ERD 주소](https://www.erdcloud.com/d/qro5eibi6BhBKvKSQ)


## 4. 시연 영상 ⛏

  [![Video Label](http://img.youtube.com/vi/ElwwGIre76s/0.jpg)](https://youtu.be/ElwwGIre76s)



## 5. 주요 기능 🎨

| 소음측정하기      | 소음 트래킹                             |
|---------------------------------|---------------------------------|
| <img align="center" src="https://github.com/Greenie-crew/.github/assets/71303448/7c61d241-4687-498c-b170-812fb178d252" width="240">| <img align="center" src="https://github.com/Greenie-crew/.github/assets/71303448/bff39e9b-7b61-49ae-9594-fb7d25ae336a" width="240">|


###  소음 측정하기 🔊 

- 소음을 측정하여 앱에 저장하고 분석 결과화면을 웹 뷰로 제공

  
###  소음 트래킹 🔊
- 특정 시간 동안 기준치 이상의 소음(80dB)이 몇번 발생했는지 그래프로 확인

<br>
<hr/>

## 👍 특장점 기술 

<details>
<summary>
<h3>✨ 안드로이드 기능 구현을 위한 생각들 </h3>
</summary>
<div markdown="1">

- 아키텍처 
    - Clean Architecture 및 MVVM 아키텍처를 멀티모듈 구조에 적용하여, 크게 Data ->   Domain <- UI 의 구조를 가지며, Dagger hilt를 통한 DI를 활용하여 UI에서 필요한 비즈니스 로직을 호출
    - app: 앱 수준 및 네비게이션 제어 등을 담당하는 앱의 시작점을 가르키는 모듈입니다.              Core 및 Feature 등의 모듈을 의존합니다.
    - core: 앱 구동간에 필요한 코드 및 특수 목적을 위한 공통 라이브러리 모듈입니다. Core       모듈 내 타 모듈에 대한 종속성을 가지지 않습니다.
    - Type은 확장이 용이하도록 BaseType을 선언해 중복되는 Property를 줄였어요.
    - feature: 앱에서 단일 책임을 처리하도록 범위가 정해진 기능 모듈입니다. Core 내의
               모듈만 의존합니다.
 
- tensorflow-model-maker-script <br>
    ◻ noise_model은 2개의 출력을 가진다.
    - 521가지의 분류를 가진 YAMNET
    - AI HUB의 소음 데이터를 기반으로 분류


</div>
</details>
<br>

<details>
<summary>
<h3>✨ 프론트엔드 기능 구현을 위한 생각들</h3>
</summary>
<div markdown="1">

![react-android-webview-communication-1](https://github.com/Greenie-crew/.github/assets/76466545/22cf181d-82ca-4a06-9396-ac41b39e924a)

#### ReactJS CSR(클라이언트 사이드 렌더링) 방식 </br>
👍 장점
- 초기 로드만 완료되면 이후 렌더링이 빠르다. </br>
- 서버에 요청할 것이 거의 없어 서버 부담이 적다. (data 필요할 때만 요청) </br>
- Web Applications에 좋다
- 
</br>
styled-components(CSS-in-JS) 활용:  비교적 가벼운 기능을 구현하는 것이기 때문에 CSS-in-JS 방식이 더 적합하다고 생각하였다
</br>

#### Redux리덕스 Reducer 리듀서로 
결과그래프 imgURL state 구현
</br>

👍 장점 </br>
-state 관리가 편하다! 관리를 한곳에서 할 수 있다. </br>
-상태를 예측 가능하게 만들어 준다. : 리덕스는 순수함수이기 때문에 다음상태가 어떻게 될지 쉽게 예측 가능 </br>
-유지보수 용이

</br>

#### vercel 배포

Vercel은 React, Vue, Angular 및 Next.js와 같은 프레임워크를 사용하여 정적 웹사이트를 더 쉽게 빌드하고 배포할 수 있는 서비스이다.
Vercel은 Git 저장소를 자동으로 인식하고, 변경 사항을 감지하여 배포하므로, 자동화된 배포가 가능하다.

또한 Vercel은 웹사이트의 성능에 대한 자세한 정보를 제공하며, 강력한 CDN을 사용하여 전 세계적으로 빠른 성능을 제공한다. 

마지막으로 Vercel은 다양한 기능과 툴을 제공하고, 서비스로 지원하는 프레임워크에서 더 많은 편의성과 효율성을 제공한다.

</br>

#### 자세히 보기 > 
https://github.com/Greenie-crew/greenie-web/blob/develop/README.md
</div>
</details>
<br>

<details>
<summary>
<h3>✨ 백엔드 기능 구현을 위한 생각들 </h3>
</summary>
<div markdown="1"> 
 
 - 기능 구현
    - 리스트를 주루룩 나열하는 것이 아닌 우선순위를 매기고 소음을 감소시키는 상품을 추천하는 기능 구현 
    - 디도스 공격 등 불특정 다수의 요청으로 인해 예기치 않은 상황이 발생하는 것을 막고자 nginx  웹 서버를 앞단에 두어 예측을 넘어서는
      이상한 요청건은 503에러 반환
    - jmeter 툴을 활용하여 부하 테스트 및 동시접속자 수를 예상하여 트래픽 핸들링

</div>
</details>







<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
