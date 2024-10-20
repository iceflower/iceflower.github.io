---
layout: post
title: "유한 상태 기계(FSM) - 설계해보기 (with. 상태천이도)"
subtitle: ""
banner:
  image: https://github.com/user-attachments/assets/fae8919e-152b-4b23-bab1-2bc76c0c709f
author: UncleCoder
tags:
    - algorithm
    - statemachine
categories: algorithm-study
date: "2024-10-17 16:55:00 +0900"              
last_modified_at: "2024-10-17 16:55:00 +0900"   
---

### 1. 개요
기본 개념 정리에 이어, 상태천이도를 활용하여 유한 상태 기계를 설계해보는 시간을 가져보려고 한다.


### 2. 초간단 예제 - 스위치
전등이나 기계 따위의 전원을 켜고 끌 수 있는 스위치를 설계해보자.
#### 2.1. 스위치가 가질 수 있는 상태값을 정의해보자.
우선, 스위치가 가질 수 있는 상태값부터 정의해보자.
우리가 흔히 아는 스위치의 상태값은, 전원이 켜진 상태임을 뜻하는 `ON` 상태와, 전원이 꺼진 상태임을 뜻하는 `OFF` 상태가 존재함을 알 수 있다.

#### 2.2. 스위치의 이벤트를 정의해보자
스위치의 상태를 바꾸기 위해선, 달리 말해 스위치의 상태천이가 일어나게 하기 위해선, 아래와 같이 스위치 외부에서 스위치로 가해지는 이벤트가 필요하다.



#### 2.3. 상태천이도를 그려보자.

<div class="mermaid"> 
flowchart TD
 subgraph subB["switch"]
    direction LR
        START["START"]
        OFF(("OFF"))
        ON(("ON"))
  end
    finger["버튼 누름 이벤트"] -.-> subB
    OFF -- turn-up --> ON
    ON -- turn-down --> OFF
    START --> OFF

    START@{ shape: f-circ}
    finger@{ img: "https://github.com/user-attachments/assets/114680fa-3864-47c4-b6aa-d39009bd92cd", h: 60, w: 60}    
</div>

### 4. 참고자료
- **위키백과 한국어판** 
  - [오토마타 이론](https://ko.wikipedia.org/wiki/%EC%98%A4%ED%86%A0%EB%A7%88%ED%83%80_%EC%9D%B4%EB%A1%A0){:target="_blank"}
  - [결정론적 알고리즘](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98){:target="_blank"}
  - [비결정적 알고리즘](https://ko.wikipedia.org/wiki/%EB%B9%84%EA%B2%B0%EC%A0%95%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98){:target="_blank"}
  - [유한 상태 기계](https://ko.wikipedia.org/wiki/%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}
  - [결정론적 유한 상태 기계](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}
  - [비결정론적 유한 상태 기계](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}

---
