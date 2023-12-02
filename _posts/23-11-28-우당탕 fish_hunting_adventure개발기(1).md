---
published: true
title: "[Pygame] 게임 개발 프로젝트(1)"
categories: Project
tag: [pygame ,project, penguin]

---

**본격적으로 들어가기에 앞서..**
이 프로젝트는 [오픈SW개발] 수업시간에 진행한 프로젝트입니다. 

## 🐧개발 동기
인터넷 연결이 안될때 등장하는 공룡게임을 알고 있나요?
![공룡게임](https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/7da322a9-3cd9-495c-b72d-3af9ba44c9a0)

저희 팀은 이 게임을 모티브로 하여 게임을 만들기로 하였습니다. 
python으로 작성가능한 pygame이라는 게임개발 라이브러리가 있었기에 pygame으로 개발을 진행하였으며
처음부터 코드를 작성하기에는 pygame을 다뤄본적이 없어서 기본 뼈대가 될만한 코드를 참고하였습니다. 

[https://blockdmask.tistory.com/419](https://blockdmask.tistory.com/419)

위 블로그의 코드를 뼈대로 하여 게임 제작을 시작하였습니다. 

<span style='background-color:#fff5b1'> **관련영상** </span>
[![공룡게임 유튜브](https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/f91fdd2f-6377-4229-a337-707dbcd45e27)](https://www.youtube.com/watch?v=ok_8mvQ8CiY&t=145s){: width="100%" height="100%"}

<hr>

## 🐧게임 스토리 배경
기존 공룡게임에서 주인공인 공룡을 펭귄으로 바꿔 진행하였습니다.

#### 게임정보
- 장르: 액션, 장애물 뛰어넘기
- 형태: 가로형
- 스테이지: 0단계



#### 스토리
> 펭귄의 오랜 꿈은 우주여행을 떠나는것입니다. 펭귄이 무사히 포식자들을 피해 우주여행을 떠날 수 있도록 도와주세요!

#### 캐릭터 소개

<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/3a52e6a8-fc17-4f02-8d92-cffa87d13387" width="400" height="200"/>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/6bff4b56-0a10-4ed1-b255-e4469f160ff4" width="400" height="200"/>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/11e9dd66-97e1-4669-97bc-d72dbc50cfb9" width="300" height="200"/>






#### 게임 화면

<b>시작화면 </b><br>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/e8170719-9ac1-421f-98f8-e536fc7ba32d" width="400" height="200"/>

<b>스토리화면 </b><br>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/b4f18298-2237-47f1-939c-d74dc7d844c7" width="400" height="200"/>

<b>게임오버화면</b><br>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/59c23b46-9f8d-4384-a9dd-5bfca71a67c1" width="400" height="200"/>

<b>게임진행화면 </b><br>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/4b12c0e5-c5cb-4224-be05-de44448779b7" width="500" height="200"/>


원작 게임의 8-bit 느낌을 살리고 싶어서 캐릭터와 배경 모두 8-bit 이미지를 사용하였습니다. 

<hr>

## 🐧이미지 ISSUE 해결 과정
프로젝트를 진행하는 도중 다른 팀들과 ISSUE를 주고 받는 과정이 존재했습니다. 
그 중 이미지와 관련된 ISSUE의 해결과정에 대해 이야기해볼까 합니다. 

**피드백1**<br>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/93fdedfd-731c-4e0a-ac95-e3d0d8b3131b" width="500" height="150"/>

**피드백2**<br>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/e471b119-98be-4dcf-bd76-fec81cdd0afe" width="500" height="200"/>

이미지 자체가 png 파일이였어서 여백 공간이 존재했던 것이 문제였습니다.
코드 적으로도 해결한 부분이 있지만 이미지 자체를 사이즈를 줄이고 여백 부분을 잘라내었습니다. 

원래는 스토리를 보여주는 파트가 없었는데  스토리를 설명하면 좋을꺼같다는 의견을 수용하여
**게임 메뉴 -> 스토리 소개-> 게임시작 -> 게임오버**
식으로 화면 구성을 변경하였습니다. 

---
다음 포스트에서는 코드적인 부문에 대해 프로젝트 과정을 담아보겠습니다😄