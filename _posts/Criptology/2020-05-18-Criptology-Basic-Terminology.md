---
layout: post_dev
title: 암호학 개요 - 기초용어
subtitle: 기초 용어에 대한 설명
categories: Criptology
authoor: Jinho Choi
---

> (암호학 개요)  
Privacy와 Authenticity의 두 가지 데이터 보호 문제를 해결하기 위한 수학적 시스템에 대한 연구분야  

### Cryptology
- Cryptography: 암호화 방식/기법
- Cryptoanalysis: 암호 해독


### '암호'란?
- 해당 정보를 변형하여 비밀을 알고있지 않은 사람은 이요할 수 없도록 하는 방법

- 정보를 이해할 수 없도록 암호화하거나, 다시 해독하기 위한 일련의 단계를 정의한 알고리즘

- 평문을 해독 불가능한 형태로 변형하거나 암호화된 통신문을 원래의 해독 가능한 상태로 변환하기 위한 모든 수학적 원리, 수단, 방법 등을 취금하는 기술이나 과학

- 즉, 암호란, 중요한 정보를 다를 사람들이 보지 못하도록 하는 방법.

> (암호학 개요에서)  
평문을 암호문으로 바꾸는 '데이터 보호' 수단


### 암호의 성질
1. 비밀성(Confidentiality)  
부적절한 노출 방지, 허가받은 사용자 이외에는 접근 불가능해야 함.

2. 무결성(Integrity)  
부적절한 변경 방지, 허가받은 사용자가 아니라면 내용을 변경할 수 없어야 함.

3. 인증(Authentication) & 가용성  
부적절한 서비스 거부 방지.

4. 부인방지(Non-repudiation)  
메시지를 전달받거나 전달한 사실이 부인될 수 없어야 함.

### 기초용어
1. 평문(Plain-text): 암호화 전의 내용(Original Message)  
암호학을 이용하여 보호해야 할 메시지

2. 암호문(Cipher-text): 암호화된 내용(Coded MEssage)  
암호학적으로 변형된 평문

3. 암호화(Encipher): 평문을 암호문으로 전환(Converter)

4. 복호화(Decipher): 암호문을 평문으로 전환(Reverse converter)

5. 키(Key): 비밀번호(The info used in cipher known only to sender/receiver)

6. 암호해독(Cryptanalysis): Analyzing of encrypted without legimate access of the key

### 암호 강도/난도 (Complexity) - Shannon의 정의
- 무조건 안전(Unconditional Secure)
    - 암호해독자가 이용할 수 있는 연산능력이 무한하다고 하더라고, 해독에 이용할 수 있는 정보의 양이 불충분할 경우의 암호계
    - "유일해를 얻기 위해 요구되는 텍스트의 최소길이인 Unit Distance가 무한한 이상적인 랜덤 키를 이용하는 암호계"

- 계산적 안전(Computational Secure)
    - 암호해독자가 이용할 수 있는 정보의 양이 충분하여 언젠가는 암호를 풀 수 있으나, 그 해독과정이 복잡하고 시간이나 경비가 많이 요구되어 경제적으로 불리한 암호계
    - 계산적 복잡도에 의해 암호강도 결정
    - 대다수 현대 암호방식이 여기에 포함