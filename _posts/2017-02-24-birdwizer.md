---
layout: post
title:  "버드와이저"
date:   2017-02-24 18:20:28 0000
tags: ['달력', '일정관리어플', '디지털 콘텐츠 경진대회', '안드로이드']
author: "dudco"
---

## *한꺼번에 정리하는 2016년* ##

이 버드와이저라는 프로젝트는 앱잼 장려상의 뽕을 받고 김 xx가 다시 한번
"우리 이 팀으로 모곤(모바일 콘텐츠 경진대회의 줄임말)도 나가자!!" 라 해서 시작된 프로젝트였다.

이 기획을 말하기 전에 일단 이름부터 말하자면 버드와이저...  음...

![image](http://postfiles1.naver.net/MjAxNzAxMTJfMjM1/MDAxNDg0MjMwMDU0MTQx.bMwgt2PG5rIhXEiTAyIOt3ry9oget-rniOCpFjpdfwUg.sPTxdu9YL-NDbXTP86yUykaGoidWbHC04iFtTlp-vgEg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.07.16.png?type=w773)

크흠흠 ... ㅋㅋㅋㅋㅋ 그렇다 술이다. 술로 이름을 우리는 프로젝트명으로 끌어와서 썼다.
기획자는 버드와이저를 bird(새) wiser(현명한) 을 합친 거라고 한다.
***
#### 기획 ####
이제 이 프로젝트의 기획을 설명하자면..
요즘 우리가 다니는 모든 곳에는 "와이파이"가 설치되어있다. 그렇다면 이 와이파이를 이용해서 너무나 바쁜 현대인의 일정관리를 하면 훨씬 효율적이지 않을까? 해서 시작된 것이다. 이런 뼈에 회의를 하여 살을 더 붙여 완성시킨 것이 'Birdwizer'이다.

버드와이저의 몇몇 핵심 기술을 설명하자면 첫 번째로 **"와이파이"** 이다.
와이파이를 이용하여 장소를 구분하여 일정을 알려준다... 정말 참신한 아이디어였던 것 같다!!

두 번째는 "플로팅 기능" 이다.
플로팅 기능이 뭐냐... 궁금한 사람이 많을 것이다. 가장 가까이에 있는 것은 페이스북 메시지이다.
페이스북 메시지는 카카오톡과 다르게 화면 옆쪽에 아이콘을 항상 띄워둔다. 그리고 그 아이콘을 클릭하면 상세정보가 뜨게 되는 것이다.

![iamge](http://postfiles2.naver.net/MjAxNzAxMTJfMzIg/MDAxNDg0MjMxNDE4MjY5.ApgULJ3mshLi8BfOpW-EJr1Z6GRG3D9jdrK6ucN6k5Qg.PBjhcaTnc3XbM7NQypC3SNhZrBGDplMUXCUkNNhcTQsg.GIF.dudco1129/1-nXWx3gEVPpIRstANlLpzew.gif?type=w773)

세 번째는 ["Farallex Header View"](http://www.kmshack.kr/2014/05/android-parallaxheaderviewpager-%ec%bd%94%eb%93%9c%ea%b3%b5%ea%b0%9c/)이다.
이것은 아무 생각 없이 안드로이드 관련 글을 보다가  알게 된 디자인? 이였다.
클릭하면 더 자세한 정보를 확인 할 수 있다.

이리저리하여 프로젝트를 시작했다. (참고로 이번 프로젝트는 첫 장기 프로젝트였다.)
사실상 우리는 시간이 정~~~말 많았다. 앱잼이 끝나자마자 만들어진 팀이기 때문에 대략... 3~4개월 정도? 있었다. 근데 정말 그 사이에 아무것도 안 했다.

진짜 일을 시작한 것은 대략 모콘 마감 1달에서 3주전?쯤이었던 것 같다. 그나마 다행이었던 것은 내가 핵심 기능을 디자인 없이 대략적으로 구현해놨다는 것이었다.

일단 와이파이 구현에 대해 얘기하자면 시작할 때는 정말 막막했다. 처음으로 하드웨어 쪽을 다루는 것이었고 와이파이 고유의 이름을 못 가져오면 이대로 망한다는 생각을 가지고 시작했다.
하지만 우리에게는 구글 신이 있다!!

그리하여 정말 쉽게 현재 연결된 와이파이의 정보를 받아 올 수 있었다.

그리고 나서 플로팅을 구현하려는데... 저번 앱잼 때 이용했던 강제로 띄우는 View를 잘 이용하면 가능할 것 같았다. 하지만... 생각보다 엄청나게 진짜 정말 힘들었다. 실제로 움직이는 것과 가운데를 기준으로 벽으로 향하는 것, 없애는 것 등을 구현하는 것은 정말 힘들었다. 그나마 다행인 것은 github에 다양한 방법으로 구현한 코드들을 참고 할 수 있었다는 것인데 정말 보기만 해도 어려운 코드들이었던 것 같다.

세 번째로는  Parallax 헤더 뷰! 이것은 딱히 구현할 필요는 없었지만 너무 이뻐서... ㄹㅇ취적...
그래서 구현을 했던 것 같다. 아마 저것은 구현을 해 놓은 코드가 있어서 그냥 복붙하면 됐던 것 같은데 나는 이상하게 일일이 다 구현했다. 그것을 보고 갓 갓 선배님께서 Android Cordinator Layout에 대해 검색해보는 게 어때? 라고 해서 검색하고 신세계를 경험했다.(이래서 경험이란 게 중요한 듯)
구글 신의 힘으로 Cordinator Layout을 이용해서 직접 Parallex 헤더 뷰를 구현했다 물론 퀄리티가 높진 않다...!
***
#### 완성 ####
그리하여 완성된 앱!

![image](http://postfiles6.naver.net/MjAxNzAxMTJfMjM2/MDAxNDg0MjMyOTk2OTQ5.6Mri-cBnH_Nc62y6KV95OykP47t8MI-MFMGliHbPdCsg.HM0hghmpwq1X7N20KufRPyya3JvGcNAuI8Ms5ZwrbsAg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.51.27.png?type=w773)
튜토리얼
![image](http://postfiles11.naver.net/MjAxNzAxMTJfNzMg/MDAxNDg0MjMyOTk2ODUw.kTuahrihTdP8nrusk8Em4KDSiGfGt3fBwCdwfva9vJsg.KZbLUCNlL5uhsLdfIsFd4DJWx7ihcGGrM-r1YgLMWSEg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.51.35.png?type=w773)
메인 메뉴
![image](http://postfiles9.naver.net/MjAxNzAxMTJfMzkg/MDAxNDg0MjMyOTk2OTg2.j4h5LunEFi9SyxwJROmmkvnF6C1xs6qLCWl6OzN_orYg.vTI-Y389Kv914wfpNiX8tJT2D1KW7VA6yMBVeXHZsAEg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.51.50.png?type=w773)
와이파이 추가하기
![image](http://postfiles3.naver.net/MjAxNzAxMTJfMjUx/MDAxNDg0MjMzMDA0OTYy.PzpUFCZ8t_lu44p4iP8gnIE_-SkTFO14nrkfe2x1tA4g.NYvAyFRzyIuH7PuHV272i00IpruxaxxOGbwwgytbPeAg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.52.01.png?type=w773)
와이파이 관리 화면
![image](http://postfiles9.naver.net/MjAxNzAxMTJfNjcg/MDAxNDg0MjMzMDA1Mzc4._9W5m5apkJOE6oBqsyNGLBcJJ6BaL9TRyykcekEKfOEg.v7X9C7LCEezpCZIRV24xhIkAX3z1nmdDBNsip_46_88g.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.52.32.png?type=w773)
일정 추가 화면
![image](http://postfiles14.naver.net/MjAxNzAxMTJfMjU3/MDAxNDg0MjMzMDA0OTk4.A89EVkgnJIeSnCJzFvg6VokSjUchJyz99djTPwXx_tcg.fqZsVZfhles-S7aQ73nnr-jC7bDfsOMHKS9f8aVk6csg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.52.45.png?type=w773)
메인화면

대회 끝나고 메인화면에 저렇게 뜨는 거 고쳤는데 ㅠㅠㅠㅠㅠ

![image](http://postfiles6.naver.net/MjAxNzAxMTJfMTk3/MDAxNDg0MjMzMDA2OTQ0.46t8WNSV6wPXAlI-vbYbKVqwLlNNwZs2T4GGjJDOHUkg.r-s1qM1046VYFkwPCT1_Vax9t9AXRpFGu11AfxTx19kg.PNG.dudco1129/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2017-01-12_%EC%98%A4%ED%9B%84_11.52.22.png?type=w773)
플로팅!

<iframe width="544" height="306" src="http://serviceapi.nmv.naver.com/flash/convertIframeTag.nhn?vid=712E420107E99678FFB364E705C456CBA990&outKey=V12102f37ffba5458812c675b389fa5c322edec5fe6b05b0b717b675b389fa5c322ed" frameborder="no" scrolling="no"></iframe>

시연 영상인데 당시 제출 10분쯤 남기고 찍어서 엄청 급했다. (겁나 생생) 또 친구 목소리 그대로 나오니까 조심><

이번 프로젝트는 첫 장기 프로젝트였고 첫 교내 대회였다 앱잼 이후로는 첫 프로젝트로 앱잼 이후에 내 실력을 잘 판단할 수 있는 프로젝트였던 것 같다.

일단 실력은 정말 많이 는 것 같은데 저 때 부랴부랴 구현하는 것도 몇 개 있고 해서 코드가 정말 더럽다... 미친 듯이 더럽다... 하... 지금 저 코드를 보고 고치라면 절대 못 고칠 것 같다. 코드를 클린 하게 짜도록 좀 더 노력해야 될 것 같고, 시간이 많다고 여유를 부리면 정말 큰일 난다는 것도 잘 배울 수 있는 프로젝트였던 것 같다.

### *[소스코드](https://github.com/dudco/2016MoCon_BirdWiser)* ###
