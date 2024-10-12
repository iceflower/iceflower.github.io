---
layout: post
title: "유한 상태 기계(FSM) - 기본개념 정리"
subtitle: "날아다니는 스파게티 괴물 (Flying Spaghetti Monster) 아닙니다."
banner:
  image: https://github.com/user-attachments/assets/fae8919e-152b-4b23-bab1-2bc76c0c709f
  opacity: 0.618
  background: "#000"
  height: "70vh"
  min_height: "38vh"
  heading_style: "font-size: 3.25em; font-weight: bold; text-decoration: underline"
author: UncleCoder
tags:
    - statemachine
categories: software-study
date: "2024-10-12 16:55:00 +0900"              
last_modified_at: "2024-10-12 16:55:00 +0900"   
---

### 1. 개요
유한 오토마톤(finite automaton, FA)이라고도 하며, 컴퓨터 프로그램과 전자 논리회로를 설계하는 데 쓰이는 수학적 모델이다.

### 2. 주요 요소
유한상태기계는 다음과 같은 요소를 가지고 있다.
- **상태(State)** : 특정한 시점에 처한 상황을 표시하기 위한 플래그. (2개 이상의 집합, 중복 불가)
- **천이(Transition)**: 특정 이벤트에 반응하여, 상태를 변화시키는 과정. `전이` 라고도 한다.
- **이벤트(Event)** : 특정 데이터 입력이나 명령 등, 상태 천이를 발생시키는 사건. 

즉, 유한 상태 기계는 중복되지 않은 여러개의 상태값 중 하나를 가지고 있으며, 이 상태값들이 사이에서 어떤 상태천이가 일어나는지를 설계하는 방법이라고 할 수 있다.

### 3. 주요 유형
#### 3.1. 예측가능 여부
상태기계 동작의 예측 가능여부를 가지고, 다음과 같이 구분할 수 있다.
- **결정론적 유한 상태기계** : (예측 ⭕) 현재 상태와 주어진 이벤트에 대해, 유일한 상태천이를 취함.
- **비결정론적 유한 상태기계** : (예측 ❌) 결정론적 상태기계와는 달리, 2개 이상의 상태천이를 취하는 것이 가능.

#### 3.2. 입력값 의존성 여부
- **밀리 모델** : 상태기계가 가진 상태값과 입력값을 모두 고려하는 모델.
- **무어 모델** : 입력값을 고려하지 않고, 현재 가진 상태값만을 고려하는 모델.

### 4. 참고자료
- **위키백과 한국어판** 
  - [오토마타 이론](https://ko.wikipedia.org/wiki/%EC%98%A4%ED%86%A0%EB%A7%88%ED%83%80_%EC%9D%B4%EB%A1%A0){:target="_blank"}
  - [결정론적 알고리즘](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98){:target="_blank"}
  - [비결정적 알고리즘](https://ko.wikipedia.org/wiki/%EB%B9%84%EA%B2%B0%EC%A0%95%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98){:target="_blank"}
  - [유한 상태 기계](https://ko.wikipedia.org/wiki/%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}
  - [결정론적 유한 상태 기계](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}
  - [비결정론적 유한 상태 기계](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}

---