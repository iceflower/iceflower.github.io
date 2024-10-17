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
date: "2024-10-12 16:55:00 +0900"              
last_modified_at: "2024-10-12 16:55:00 +0900"   
---

### 1. 개요
기본 개념 정리에 이어, 상태천이도를 활용하여 유한 상태 기계를 설계해보는 시간을 가져보려고 한다.
### 4. 참고자료
- **위키백과 한국어판** 
  - [오토마타 이론](https://ko.wikipedia.org/wiki/%EC%98%A4%ED%86%A0%EB%A7%88%ED%83%80_%EC%9D%B4%EB%A1%A0){:target="_blank"}
  - [결정론적 알고리즘](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98){:target="_blank"}
  - [비결정적 알고리즘](https://ko.wikipedia.org/wiki/%EB%B9%84%EA%B2%B0%EC%A0%95%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98){:target="_blank"}
  - [유한 상태 기계](https://ko.wikipedia.org/wiki/%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}
  - [결정론적 유한 상태 기계](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}
  - [비결정론적 유한 상태 기계](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%9C%A0%ED%95%9C_%EC%83%81%ED%83%9C_%EA%B8%B0%EA%B3%84){:target="_blank"}

---
