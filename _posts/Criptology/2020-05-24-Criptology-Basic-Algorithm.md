---
layout: post_dev
title: 암호학 개요 - 기초 알고리즘
subtitle: 기초 알고리즘에 대한 이해
categories: Criptology
authoor: Jinho Choi
---

### 고전암호와 현대암호를 가르는 기준
Computer의 존재 유무
= 형태 그 자체는 환자와 전치의 반복으로 구성에는 크게 차이 없음.

### 환자(Subtitution)  
1. Simple Subtitution  
평문 한 문자를 암호문 한 문자로 1대1 대응(mapping) 시키는 것.  
통계적 해석이 가능.  
2. Homophomic Subtitution  
한 평문 철자에 대해 그 철자의 빈도수가 비례하는 갯수의 암호문 집합(이를 Homophones로 정의)을 할당하여, 그 가운데 하나를 랜덤선택하여 변환 시키는 것.
3. Polyalphabetic Subtitution  
평문을 일정한 문자 그룹으로 대치시키는 것.  
반복 주기를 통하여 유추 가능.
4. Polygram Subtitution  
한 문자단위가 아닌 보다 큰 문자 블럭 단위로 암호화 함으로써 해독을 어렵게 한 방식.

### 전치(Tanspostion)
평문의 문자나 비트의 순서를 어떤 절차에 따라 재조정함으로써 메시지를 암호화 시키는 방법.

### 타원 곡선암호
키의 길이가 짧아 고속으로 동작하는 암호 기법
휴대용 Device에 사용하기 적합

### RSA
전치 환자의 응용  
개인 키를 도장처럼 활용

### 공개 키 암호와 공인인증서
공개 키 암호 논문: New Direction in Cryptography
전자 서명 개념(Reverse RSA)

### 해쉬함수
암호화폐에 사용  
단방향성 압축  
Criptographic Hash: 암호학적으로 안전한 해쉬 방식  
MD4/5  SHA 등의 방식 있음

### Multi-signature
해킹에 대한 방지

### PKI
자물쇠의 소유자를 validate 하는 방식  
인증서  

### Dawn of Provable Security(논문)
암호'학'의 시작  
용어들의 엄밀한 정의와 이론 기재, 안정성에 대한 수학적 증명

### 영지식 증명
프라이버시를 위한 수단  
개인정보의 보호  
나의 정보를 알려주지 않으면서도 암호의 Validity를 확인할 수 있다.  
블록체인에 적용하는 경우에는 매우 비 효율적으로 동작한다.

### 데이터베이스의 암호화