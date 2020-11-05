---
layout: post
title: Looper and Handler
categories: [Android]
authoor: Jinho Choi
---

- 기본적으로 하나의 main thread 만을 갖고 작업을 진행
- UI 외에 다른 시간이 오래 걸리는 작업 실행 시 UI가 버벅이거나 멈추는 상황이 발생
- 이는 사용자 경험에 매우 안좋은 영향을 끼침
- 이를 해결하기 위해 시간이 오래 걸리는 작업들을 멀티스레드를 통하여 진행
- 이때, Thread 간의 통신을 도와주는 장치 중 하나로 Looper와 Handler가 사용된다.

### Looper:  
- Thread 내의 Message Queue를 감시하여, msg 객체의 인입이 있을 때, Handler에 전달

### Handler:  
- msg를 전달받아 처리,
- msg를 다른 Thread로 전달

### MSG:  
- Thread/Activity 간 통신에 사용되는 객체
- 직접 Parcelable을 구현하는 것은 복잡하고, 유지보수 측면에서도 불리
- 이에 객체 형태로 전달 가능한 Msg를 활용하며, 이를 Looper/Handler에 전달하여 통신에 활용