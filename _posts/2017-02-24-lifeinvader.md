---
layout: post
title:  "lifeinvader"
date:   2017-02-24 21:08:33 0000
tags: ['안드로이드', '보안']
author: "dudco"
---


## *한꺼번에 정리하는 2016년* ##

핡핡 안녕하세요 이번 프로젝트는 <strong style="font-family: ">'lifeinvader'</strong>입니다.

음... 음... 어디서 많이 본 것 같지 않나요? ㅋㅋㅋㅋ

![image](http://postfiles8.naver.net/MjAxNzAxMTZfNyAg/MDAxNDg0NTUyMTkwMjM5.bUi7OpsiH7Oyg6csSkmme340yv4oMJQwOhh-lkpDRnAg.Lp3_9rd-Dvq_psijkFBUkx_whfSVO945lJaGrh2nIxYg.JPEG.dudco1129/maxresdefault.jpg?type=w773)
바로 GTA에 나오는 SNS의 이름입니다! ㅋㅋㅋㅋㅋㅋ

친구한테 SNS 앱을 만들 건데 관련된 이름 좀 추천해달라고 하니까 이걸 추천하더군요 덕분에 디자인도 어느 정도 된 앱을 만들 수 있게 되었습니다! ㅎ

사실 이번 프로젝트는 KISA(한국 인터넷 진흥원)에서 주최하는 제3회 소프트웨어 보안 경진대회에 출전하기 위해 진행한 프로젝트입니다. 대회에서 간단하게 인터넷과 연결된즉 로그인, 로그아웃, 회원가입, 글쓰기 등이 되는 앱을 스스로 만들고 그 앱에 보안적 이슈를 최대한 적게 만드는 대회입니다.

### 간단하게 말해 '안전한 모바일 앱 만들기'입니다 ###

그래서 저는 SNS를 만들었던 것이죠! ㅎㅎ

이번 프로젝트는 보안 쪽을 해보고 싶었던 저를 위해 저랑 가장 친한 선배가 팀을 한 개 꽂아주셨습니다.


실제로 이 팀에는 저를 제외한 두 분이 BOB셨습니다.

원래는 웹 해킹 분야를 나가려다가 제가 끼는 바람에 모바일 보안 분야로 중복 신청을 하게 되었습니다.

하지만 선배 두 분이 모두 바쁘셔서 거의 대회에 신경을 쓰지 못하시는 바람에 웹 해킹은 거의 못했고(제가 웹 해킹을 못함 ㅎㅎ;;), 모바일 분야는 앱 개발이 가능한 사람이 저 밖에 없어 저 혼자 심심풀이로 앱을 만들었습니다.

딱 이때 제가 Android Animation 쪽에 관심을 가지면서 어떻게 앱을 이쁘게 만들 수 있을까??를 고민하던 찰나였습니다. 그래서 완성된 로그인 화면이 이렇습니다.

<div class="image3">
<img src="http://postfiles13.naver.net/MjAxNzAxMTZfMTU3/MDAxNDg0NTU0Mjk0MDg5.o1ZVGx2HNqsl2-rynaT88W9Z2n7VP6Ox6Aw5TOgVl8Eg.AP4yj4Vndw44WKGSnzBFp0bplTUj8Wg-KTnRLvVVb4cg.GIF.dudco1129/liefeinvader1.gif?type=w773" style="margin-right: 3px; width: 100%; height: 100%"/>
<img src="http://postfiles11.naver.net/MjAxNzAxMTZfMTc3/MDAxNDg0NTU0MjkzMTIx.Rw-FeaXoFcrc2jvHUUngFIwFTruzC4Rq5thRcSvQjiYg.OvhwY8bPegpd-HSBVHosyrIbY2op0XGRw49hmqkSkYAg.GIF.dudco1129/lifeinvader2.gif?type=w773" style="margin-right: 3px; width: 100%; height: 100%;"/>
<img src="http://postfiles5.naver.net/MjAxNzAxMTZfMTky/MDAxNDg0NTU0MjkyODI2.xWmiZiGm1UHUKQuC14uVzym-PqbhOOXbDSKB0efu6BYg.QcgL_LYY1b66ppZuZpPsa72Fx9U_tF4RpKMygjuJwLEg.GIF.dudco1129/lifeinvader3.gif?type=w773" style=" width: 100%; height: 100%;"/>
</div>

<ul style="text-align: left">
<li>
<p>
일단 첫 번째 사진은 앱을 처음 켰을 때 화면으로 스플래시 화면이 진행되면 로고가 위로 올라가면서 로그인 창이 뜨는 방식이죠! ㅎㅎ
아마 이 방식이 페이스북 방식인데 이뻐서 따라 해봤습니다!
</p>
</li>

<li>
<p>
두 번째 사진은 EditText를 포커싱 하면 사용자의 입력을 도와주는 hint가 EditText 위로 살짝 올라가는 효과입니다.
겁나 어려울 것 같지만 착하디착한 구글에서 이미 만들어두어서 TextInputLayout과 TextInputEditText를 사용하면 쉽게 구현이 가능합니다!
</p>
</li>

<li>
<p>
세 번째 사진은 비밀번호 찾기를 누르면 원으로 메인화면이 변하는 화면입니다.
(색깔이 같아서 티가 별로 안 나네요 ㅠㅠ)
이거 때문에 Xml 코드가 겁나 길어진...
이 땐 심심해서 했던 걸로 기억하는데 실제 개발에서 이렇게 하면 아마 맞지 않을까요?? 퍽<<<
</p>
</li>
</ul>

그 외에 회원가입과 게시물 작성 등이 있는데 그쪽은 시간 부족으로 거의 구현을 못 해서 패스! ㅎㅎㅎㅎㅎㅎㅎ...

이번 대회는 앱의 완성도도 중요하지만 앱에 적용된 보안 방식이 중요했기 때문에 예선 통과하자마자 죽어라 선배들과 보안을 적용했습니다

<h5 style="text-align:left"> 첫 번째로 난독화 사용입니다. </h5>

![image](http://postfiles7.naver.net/MjAxNzAxMTZfMTI3/MDAxNDg0NTU0OTg3NjU0.XLFgFOF2Y6eHDfIzR2kfDzAKKnGo67_RqdPVG6C3lAwg.wE-x8TW5yv9gKZVJ7KBNjOlqDu_IDJxWhXPSo58DKdkg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.22.59.png?type=w773)

앱을 개발하고 apk를 유포하면 사용자는 apk를 사용해서 앱을 설치하고 사용합니다. 그런데 이 apk를 decompile 하면 앱의 java 소스 코드가 그대로 노출되는데 그때 악용을 방지하고자 난독화를 시킵니다. 이 난독화는 ProGuard를 사용하면 쉽게 가능합니다!

<h5 style="text-align:left"> 두 번째로 기타 정보를 암호화해서 저장하는 것입니다. </h5>

![image](http://postfiles9.naver.net/MjAxNzAxMTZfMjUy/MDAxNDg0NTU1MzA5MTk3.Zc2FrCFjRImOqrwDvJH8lUa9aSvoO_yyUEJEGZLi-1sg.wO2M7CLFHOmiC4YXR3mXNGOzeFEXeZCRVfFesj7BLsAg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.28.20.png?type=w773)

 위쪽에 저장된 DB에는 name에 '김동규'라고 암호화가 되지 않은 채로 저장되어있었지만 아래쪽의 경우는 알 수 없는 문장으로 암호화되어 저장되었습니다.

 <h5 style="text-align:left"> 세 번째로 입력값의 유효성입니다. </h5>

 ![image](http://postfiles16.naver.net/MjAxNzAxMTZfMTkw/MDAxNDg0NTU1Mzg0MTYy.rj0h3us48sGrXcrSC4XUbmKdLeb61ytSoOJoZMv08log.RXEMb400FhLuYhGiAqeT2GmBpnXTHlvzmee0dQI4x7og.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.29.37.png?type=w773)

  위 쪽의 코드를 사용하면 공란 입력 시에도 회원가입과 로그인이 가능했었는데 아래쪽 코드로 대체함으로 불가능하게 바꾸고, 로그인시의 이메일이 맞는지도 확인했습니다.

  <h5 style="text-align:left"> 네 번째로 비밀번호 조합 규칙 부재입니다. </h5>

  ![image](http://postfiles12.naver.net/MjAxNzAxMTZfNDAg/MDAxNDg0NTU1NTM3MjIy.IYKKVCNev48hwy1FcyhctjcoUQ_TezGYYOwkek8lOQUg.snOGn0LdWsGJmGa7URXXdoHXcbGHf1YhX2uY0UYltVQg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.32.01.png?type=w773)

  위 쪽 코드는 비밀번호로 아무거나 사용해도 됐습니다. 심지어 공란도 가능했지만 아래쪽 코드를 사용함으로써 비밀번호로 숫자, 영어, 한글만 사용 가능하도록 변경했습니다.

<h5 style="text-align:left"> 다섯 번째로 하드코딩된 암호화키입니다. </h5>

![image](http://postfiles10.naver.net/MjAxNzAxMTZfMTQw/MDAxNDg0NTU1NzExNzM5.q9xz5WKPDvTsbqDcNiupsvF5KyIVrz1SWMjQtyjAu00g.OJT8q1SuQUQbrja0qfrsgGMRSWhE08hMvV47GFzIjowg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.35.05.png?type=w773)

자바 코드에 암호화키를 그대로 하드코딩해놨기 때문에 apk를 DeComfile 암호화키를 그대로 볼 수 있습니다. 이것을 방지하기 위해 RSA 공개키 암호화를 한번 덧씌워 주었습니다.

<h5 style="text-align:left"> 여섯 번째로 중요 정보 평문 저장입니다. </h5>

![image](http://postfiles14.naver.net/MjAxNzAxMTZfNDIg/MDAxNDg0NTU1ODk3MTE1.klq4k7foSAkA4P-FmnHz0hlmQQjJrqS8qxkLrt6ALK0g.k_zRz0Rnuj9iSVejIY60zfc5oYDjksVy2UrWBummV5Ag.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.38.11.png?type=w773)

중요 정보 예를 들면 id나 비밀번호를 평문으로 저장하는 것을 AES-256암호화 알고리즘을 통해 저장함으로써 보안성을 높였습니다.

<h5 style="text-align:left"> 일곱 번째로 오류 상황 대응 부재입니다. </h5>

![image](http://postfiles10.naver.net/MjAxNzAxMTZfMjAx/MDAxNDg0NTU2MDIyNjgz.ft4kBM-75FpjMrov4IqPci7wWftT8zNOLD3yuYqh8kEg.CHAbhiUKN2eSUgd78vawf6F2Fel9xL_OBRHajcCzEWMg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.40.13.png?type=w773)

위 쪽의 로그인 화면에서 동그란 애니메이션과 함께 변환되는 부분이 있었습니다.

이 부분은 안드로이드 롤리팝이 상부 터 가능한 것입니다.

위쪽 코드에서는 롤리팝 이하에서 실행시키면 앱이 터져버리지만 아래쪽 코드에서는 롤리팝 미만은 애니메이션 없이 변환되도록 합니다.

<h5 style="text-align:left"> 여덟 번째로 SQL injection입니다. </h5>

![image](http://postfiles15.naver.net/MjAxNzAxMTZfMTYz/MDAxNDg0NTU2MjAxNDM0.yKRVHOPMurbZj0LQlnThrjMEvEDPq_Fn4hIlcbrAlkkg.bXZw4999eYOBgAJccf-XpIMCT_73qWEd_EKiePGev7Qg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-16_%EC%98%A4%ED%9B%84_5.43.15.png?type=w773)

요번 프로젝트에서는 NoSQL인 mongoDB를 사용했지만 mongoDB도 SQL injection이 가능하다 하여 많이 놀란 부분입니다. mongoDB의 대부분의 Sql injection은 $(달러)를 제한하면 방지된다 하여 로그인할 때 $를 쓸 수 없도록 하였습니다.

와.. 정말 많네요... ㅋㅋㅋㅋㅋ

요번 대회는 처음으로 보안에 대해 알 수 있었습니다. 원래 저는 보안 전문가를 꿈으로 삼고 컴퓨터를 접하였는데 생각보다 개발이 재밌어서 개발을 하는 중이었습니다. 그러던 중 대회 포스터를 보고 보안에 대한 관심이 다시 증가되었고, 선배의 도움 덕분에 출전까지 할 수 있었던 것 같습니다.

![image](http://postfiles6.naver.net/MjAxNzAxMTZfMjY0/MDAxNDg0NTU2NTEyMTY3.c83YBm6mBvCy4z3Uyn0rg55hpB5LeI-eH-_1NqDADLsg.lppDhzMw6EmLzvD_SUP5u6DvJajui3pci_inUgTcrsog.JPEG.dudco1129/IMG_20160906_115758.jpg?type=w773)

운 좋게 최우수상도 수상하여 무려 행정자치부 장관상도 수상했습니다! ㅎㅎㅎ

![image](http://postfiles1.naver.net/MjAxNzAxMTZfMTQ5/MDAxNDg0NTU2NzQ4NzM4.f9lo_nlgpDnapQZCmtKV-PGooh_D1Tq7QMuF3lIuzBQg.aXy2xk092tPkKdQXb7aHBDjfxg6nYr-gGZYErDD1A88g.JPEG.dudco1129/image_2765720801484556693579.jpg?type=w773)

덕분에 이렇게 학교에 플래카드도 걸려보네요 >< 헿

#### *[소스코드](https://github.com/dudco/SecureCoding)* ####
