
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
<img src="https://github.com/Greenie-crew/.github/assets/71303448/7c894022-9677-4202-8762-0fdc0b378e6a"  width="600" height="480">
</div>

## 3. 백엔드 ERD 및 와이어 프레임 🛠

사진 뭐 넣고 싶은데 와이어프레임 어떻게 보여줄지 추천 받기 

### [ 와이어프레임 ]   [ Figma ](https://www.figma.com/file/D1FJxm69kI0QDLSWs0adiG/%EB%91%90%EB%91%90's-team-library?type=design&node-id=411%3A2&t=cK2CQkRgg4JjV27l-1)

### [ 백엔드 ERD ]  [ERD 주소](https://www.erdcloud.com/d/qro5eibi6BhBKvKSQ)


## 4. 시연 영상 ⛏

  [![Video Label](http://img.youtube.com/vi/ElwwGIre76s/0.jpg)](https://youtu.be/ElwwGIre76s)



## 5. 주요 기능 🎨

| 소음측정하기      | 소음 트래킹                             |
|---------------------------------|---------------------------------|
| <img align="center" src="https://github.com/Greenie-crew/.github/assets/71303448/7c61d241-4687-498c-b170-812fb178d252" width="240">| <img align="center" src="https://github.com/Greenie-crew/.github/assets/71303448/bff39e9b-7b61-49ae-9594-fb7d25ae336a" width="240">|


###  소음 측정하기 🎉 

- 소음을 측정하여 앱에 저장하고 분석 결과화면을 웹 뷰로 제공

  
###  소음 트래킹 🎉
- 특정 시간 동안 기준치 이상의 소음(80dB)이 몇번 발생했는지 그래프로 확인

<br>
<hr/>

## 👍 특장점 기술 

<details>
<summary>
<h3>✨ 안드로이드 기능 구현을 위한 생각들 </h3>
</summary>
<div markdown="1">

- 코드 컨벤션
    - **협업 및 분업**을 원활하게 하기 위해 개발 시 **통일성**을 부여하고자 많이 고민했어요.
    - **TypeScript,  Prettier** 덕분에 버그를 예방하고 협업 생산성을 높일 수 있었어요.
    - `Button` `Label` `Input` `Title`과 같은 **재 사용성**이 요구되는 UI 요소는 **Atom 단위**로 설계하여 **생산성**을 높일 수 있었어요
    - Type은 확장이 용이하도록 BaseType을 선언해 중복되는 Property를 줄였어요.
    - 덕분에 200줄의 Type 코드가 60줄로 줄어 들 수 있었어요.
    - 그 외 통일해야 할 부분을 발견하면 즉시 함께 고민하고 실행했어요.

- 기술
    - **RTK** 를 사용하여 Client 상태를 관리했어요.
    - **RTK Query**를 활용하여 Server 상태를 관리하였으며, Caching을 활용하여 통신 비용을 줄일 수 있었어요.
    - 덕분에 응답 다음 작업이나 에러 발생 시에도 통일된 작업을 수행할 수 있었어요.
    - **Emotion**을 활용한 스타일링 작업 시에 글로벌 스타일 적용과 **Typo, Palette**로 선언한 변수를 이용하도록 협의하여 통일성을 부여했어요.

</div>
</details>
<br>

<details>
<summary>
<h3>✨ 프론트엔드 기능 구현을 위한 생각들</h3>
</summary>
<div markdown="1">

- 코드 컨벤션
    - **협업 및 분업**을 원활하게 하기 위해 개발 시 **통일성**을 부여하고자 많이 고민했어요.
    - **TypeScript,  Prettier** 덕분에 버그를 예방하고 협업 생산성을 높일 수 있었어요.
    - `Button` `Label` `Input` `Title`과 같은 **재 사용성**이 요구되는 UI 요소는 **Atom 단위**로 설계하여 **생산성**을 높일 수 있었어요
    - Type은 확장이 용이하도록 BaseType을 선언해 중복되는 Property를 줄였어요.
    - 덕분에 200줄의 Type 코드가 60줄로 줄어 들 수 있었어요.
    - 그 외 통일해야 할 부분을 발견하면 즉시 함께 고민하고 실행했어요.

- 기술
    - **RTK** 를 사용하여 Client 상태를 관리했어요.
    - **RTK Query**를 활용하여 Server 상태를 관리하였으며, Caching을 활용하여 통신 비용을 줄일 수 있었어요.
    - 덕분에 응답 다음 작업이나 에러 발생 시에도 통일된 작업을 수행할 수 있었어요.
    - **Emotion**을 활용한 스타일링 작업 시에 글로벌 스타일 적용과 **Typo, Palette**로 선언한 변수를 이용하도록 협의하여 통일성을 부여했어요.

</div>
</details>
<br>

<details>
<summary>
<h3>✨ 백엔드 기능 구현을 위한 생각들 </h3>
</summary>
<div markdown="1">

    

- 기술 
   - java <br>
    ◻ 내부 클래스를 활용해서 request 클래스로 들어오고 response 클래스로 나가는 변수를 핸들링하여 원하는 변수만 접근하도록 구현하였습니다. <br>
    ◻ 제너릭 클래스를 활용하여 의도한 구조를 가진 Object를 응답하도록 구현하였습니다. <br>
   - 추천 상품 조회 기능 구현 <br>
    ◻ 소음 

 - 트래픽

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
