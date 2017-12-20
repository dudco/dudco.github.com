---
layout: post
title:  "Schooler (D3S해커톤)"
date:   2017-02-26 02:32:10 0000
tags: ['해커톤']
author: "dudco"
photos:
- http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_MElLcXgwSENiclk
---

# 기획

안녕하세요! 오늘은 2월 4일, 5일 무박 2일 동안 진행된 D3S해커톤에서 진행한 Schooler 입니다!!
일단 D3S해커톤은 D를 의미하는 <span style="color: #00c8ff;">디지털 미디어 고등학교</span>, <span style="color: #00c8ff;">대덕 소프트웨어마이스터 고등학교</span>, <span style="color: #00c8ff;">대구 소프트웨어 고등학교</span>와 S를 의미하는 <span style="color: #00c8ff;">선린인터넷</span> 고등학교 이렇게 네 학교가 모여서 진행한 해커톤입니다. 운영진까
지 모~두 네 학교 학생들이 맡았고 기획부터 협찬까지 모두 고등학생이 진행한
해커톤입니다!!

[기사](http://dthumb.phinf.naver.net/?src=%22http%3A%2F%2Ft1.daumcdn.net%2Fnews%2F201702%2F05%2Fetimesi%2F20170205151303243moug.jpg%22&type=ff500_300)

위쪽 링크는 D3S에 관한 기사입니당.
저희는 선린, 디미, 대덕 이렇게 세 학교에서 온 사람들로 팀이 구성되었습니다.
저와 기획자 선배가 선린, 개발자분이 대덕, 디자이너가 디미였습니다.

<p>이번 대회의 주제는... <strong style="color: red; font-size: 27px; font-weight: bold;">학교</strong> !였습니다.
저희는 학교라는 주제에 맞춰 <span style="color: #f02c8c">학생증을 만드는 앱</span>이 어떨까 생각을 하였습니다. 실제로 학교의 학생증의 디자인에 불만을 가진 학생들이 많다고 생각되었기 때문에 이대로 개발을 시작했고, 거기에 살을 더 붙여 이번 해커톤의 궁극적인 목표는 네 학교의 '<span style="color: red; font-size: 20px">네트워킹</span>'이라고 생각하여 NFC태그를 통한 <span style="color: #f02c8c">학생증 교환</span>과 <span style="color: #f02c8c">채팅기능</span> 까지 추가하였습니다.</p>



저는 이번 대회에서 백엔드 개발을 맡았습니다.
Node.js를 이용해서 <span style="color: rgb(0, 163, 80)">페북을 이용한 회원가입과 로그인</span>, 그리고 각종정보를 <span style="color: rgb(0, 163, 80)">DB에 저장후 CRUD</span>를 만드는 기능, 마지막으로 <span style="color: rgb(0, 163, 80)">이미지 업/다운로드</span> 기능을 개발하였습니다.
(선배의 협박으로 6시간만에 끝내고 프론트를 도와드렸다는... 아 저는 원래 안드로이드를 주로해요!)

***

# 서버
서버개발에서 어려웠던 점은 많지 않았지만
오랜만에 진행하는 서버였기 때문에 많이 헷갈렸던 기억이 있습니다. ㅎㅎ
한가지 에피소드로는 페이스북에서 로그인 후 가져오는 정보들을 저는 백엔드단에서 처리해주는 줄 알고 몇시간 동안 쩔쩔매며 "이메일이랑 나이같은거 어떻게 가져오지 ㅠㅠ" 하고 있었는데 알고보니 프론트엔드단에서 처리해주는 것이더라구요... 하... 이거 듣고 10분간 멍때렸어요.. ㅠㅠ

Node.js에서 주로 사용한 모듈(패키지)로는 무조건 필요한 <span style="color: rgb(167, 154, 0)">express</span>,
이미지 업/다운을 위해 <span style="color: rgb(167, 154, 0)">Multer</span>,
MongoDB를 이용하기 위해 <span style="color: rgb(167, 154, 0)">mongoose</span>
등을 이용했습니다.

일단 express는 웹 프레임워크로 보다 빠르고 간단하게 웹 서버를 짤 수 있게 도와주는 패키지 입니다.
그리고 Multer는 이미지 업/다운을 할 때 사용되는 패키지로 사용법이 굉장히 간단하고 어렵지않아
간간히 검색을 이용해서 사용이 가능했습니다.
마지막으로 mongoose는 MongoDB를 이용하기 위해서 만들어진 패키지입니다.

***

# 클라이언트
프론트 엔드의 경우는 이번 대회에서 개발자가 둘 이었기 때문에 각각 개발할 곳을 나누어
개발했습니다.
그래서 저는 실제로 명함을 원하는데로 디자인하고 만들 수 있는 그림판(?)같은 것을 만들었습니다.

| ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_d0lCUmhDZGlaaFk) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_M0lpWXNnWUhvR0k) | ![image](https://drive.google.com/open?id=0B0QMcRMI39U_bXVIUnZycDd6RXc)
|----
| ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_bXNnZ0VsVDc5d1U) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_bVczUjJRM2lxazA) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_cjNkWndMV0xjVVk)
{: rules="groups"}

맨 왼쪽위가 아무것도 없는 그림판의 상태이고, 나머지 사진들은 디자인을 하는 중인 사진입니다. 실제로 저런식으로 자신이 원하는 글씨를 넣은 후 색, 폰트, 크기들을 원하는 데로 조절이 가능합니다.

여기서는 Stiker라는 라이브러리를 사용했습니다.
저렇게 이미지와 텍스트를 추가하고 사용자가 원하는데로 조절할 수 있도록 해주는 라이브러리 입니다.

[https://github.com/wuapnjie/StickerView](https://github.com/wuapnjie/StickerView)

| ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_RFh6Wmt0VmIzRjA) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_bkhXS19XUXktaGc)

위 사진은 메인화면과 내 정보 설정 화면입니다.
(제가 개발한 곳이 아니라 자세힌 모름...)
메인 화면에는 아래와 같은 명함이 들어갑니다.

| ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_RGdzRVJiaWpBekE) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_WGpSTXgtaDJyY3c) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_VXNUVDhUWWJNOG8)

그리고 명함의 디자인을 사용자간의 커뮤니티에서 교환, 구매, 팔기 등이 가능하게 만들고 싶었지만 시간이 부족하여 실제로 구현은 못하였어요 ㅠㅠㅠㅠ

그리고 채팅! 부분은 사진이..없네요...
아무튼 설명을 드리자면 제출 2시간 전에 개발을 시작해서 겨우 끝낸 부분으로
구글의 FireBase를 이용해서 엄청나게 빠르게 만든 부분입니다.
이 것을 보고 대덕에서 오신 개발자분이 넘나 대단하다는 것을 느꼈죠...

이번 대회를 나가면서 사실 저는 개발이 하고 싶어서라기보다
<span style="color: rgb(255, 156, 35);">인맥을 쌓고싶어서</span> 나간 것이 좀 더 큰 이유였습니다. 실제로 대한민국은 인맥사회이기도 하니까요 ㅎㅎ
그리하여 대덕과 디미고 선배분들을 한 분 씩 알 수 있는 좋은 기회였던 것 같습니다.

또 다른 점으로 저희학교는 역시 대단하다(?)입니다.
이번 대회의 상이 6개였는데 그중 4개를 선린이 있는팀이 수상한...
그리고 대상은 <strong style="font-size: 27px">저희팀</strong>이!!! 헤ㅔㅔㅔㅔㅎㅎㅎㅎ

굉장히 기분이 좋았어요 ㅎㅎㅎㅎ
팀 빌딩에 실패하여 팀, 기획이 나오지않는 팀, 디자이너가 없어 디자인이 안나온느 팀 등
정말 다양한 팀이 있었지만 저희 팀은 그렇지않아서 정말 재미있게 대회를 즐길 수 있었습니다.
또 엄청나게 수고해주신 저희 팀원 분들께 감사하고 사랑해요~

# *[소스코드](https://github.com/dudco/2016_School_Iot)*

| ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_Uk1JdmpwQmVLbkU) | ![image](http://drive.google.com/uc?export=view&id=0B0QMcRMI39U_OWJ0OFJFQVY2NHM)
