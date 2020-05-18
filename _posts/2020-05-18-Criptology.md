---
layout: post
title: ADB Basic Usage for android debuging
categories: 
---


### 암호의 성질
1. 비밀성(Confidentiality)
2. 무결성(Integrity)
3. 인증(Authentication)
4. 부인방지(Non-repudiation)

### 기초용어
1. 평문(Plain-text): 암호화 전의 내용(Original Message)
2. 암호문(Cipher-text): 암호화된 내용(Coded MEssage)
3. 암호화(Encipher): 평문을 암호문으로 전환(Converter)
4. 복호화(Decipher): 암호문을 평문으로 전환(Reverse converter)
5. 키(Key): 비밀번호(The info used in cipher known only to sender/receiver)
6. 암호해독(Cryptanalysis): Analyzing of encrypted without legimate access of the key
7. 전수조사(Brute-force Search)

### 고전암호와 현대암호를 가르는 기준
Computer의 존재 유무
= 형태 그 자체는 환자와 전치의 반복으로 구성에는 크게 차이 없음

### 타원 곡선암호
키의 길이가 짧아 고속으로 동작하는 암호 기법
휴대용 Device에 사용하기 적합

### RSA
전치 환자의 응용  
개인 키를 도장처럼 활용

### 공개 키 암호와 공인인증서
전자 서명 개념(Revers RSA)

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