---
layout: single
title: 우당탕 fish_hunting_adventure 개발기(1)
excerpt: 
writer: Kiwiio
categories: 
    - Project
tag: "pygame" ,'project' , 'penguin'
toc: true
toc_sticky: true
author_profile: false
date: 2023-11-28
sidebar: 
    nav: "docs"
---
**본격적으로 들어가기에 앞서..**

오픈SW개발 수업시간에 깃허브에 대해 배우며 세명이서 팀을 이루어 pygame을 만드는 프로젝트를 진행하였다.

## 🐧개발 동기
인터넷 연결이 안될때 등장하는 공룡게임을 알고 있는가?
![공룡게임](https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/7da322a9-3cd9-495c-b72d-3af9ba44c9a0)

우리 조는 이 게임을 모티브로 하여 게임을 만들어보고자 하였다.
python으로 작성가능한 pygame이라는 게임개발 라이브러리가 있었기에 pygame으로 게임을 진행하였다.
1부터 코드를 작성하기에는 pygame을 다뤄본적이 없어서 기본 뼈대가 될만한 코드를 가져왔다. 

https://blockdmask.tistory.com/419
위 블로그의 코드를 뼈대로 하여 게임을 제작하기로 했다.

<span style='background-color:#fff5b1'> **관련영상** </span>
[![공룡게임 유튜브](https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/f91fdd2f-6377-4229-a337-707dbcd45e27)](https://www.youtube.com/watch?v=ok_8mvQ8CiY&t=145s){: width="100%" height="100%"}

<hr>

## 🐧게임 스토리 배경
우리 조는 공룡 대신 펭귄으로 주인공을 바꿔 진행하기로 하였다.

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

<b>시작화면 </b>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/e8170719-9ac1-421f-98f8-e536fc7ba32d" width="400" height="200"/>

<b>스토리화면 </b>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/b4f18298-2237-47f1-939c-d74dc7d844c7" width="400" height="200"/>

<b>게임오버화면</b>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/59c23b46-9f8d-4384-a9dd-5bfca71a67c1" width="400" height="200"/>

<b>게임진행화면 </b>
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/4b12c0e5-c5cb-4224-be05-de44448779b7" width="500" height="200"/>


도트느낌을 살리고 싶어서 엄청난 이미지 서칭과 이미지 제작도 했다.. 
하나하나 손수 만들고 코드가 바뀌거나 스토리 내용이 바뀔때마다 업데이트 되어야했기때문에 시간이 오래 걸렸다. 

## 🐧이미지 ISSUE 해결 과정
개발 과정 도중 다른조와 함께 피드백을 하는 과정이 있었다.
가장 많이 언급되었던 히트박스 문제가 있었는데

**피드백1**
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/93fdedfd-731c-4e0a-ac95-e3d0d8b3131b" width="500" height="150"/>

**피드백2**
<img src="https://github.com/kkiwiio/kkiwiio.github.io/assets/121476928/e471b119-98be-4dcf-bd76-fec81cdd0afe" width="500" height="200"/>

이미지 자체가 png 파일이였어서 여백 공간이 존재했던 것이 문제였다. 코드 적으로도 해결한 부분이 있지만 이미지 자체를 사이즈를 줄이고 여백 부분을 잘라내었다.

원래는 스토리를 보여주는 파트가 없었는데 피드백 주신 부분에서 스토리를 설명해주셨으면 좋겠다고 하셔서 
**게임 메뉴 -> 스토리 소개-> 게임시작 -> 게임오버**
식으로 화면 구성을 변경하였다.
확실히 스토리가 추가되니 게임이 조금 더 기승전결이 있어보였다.
<hr>
우당탕 게임 개발기 2탄에서는 본격적인 코드 개발 과정과 그 과정상에서 발생했던 오류들에 대해 소개해보고자 한다!