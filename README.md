# Devit(python)
> 개발자 구인 구직 서비스 <br/>

<br/>



## 1. 제작 기간 & 참여 인원
* 2022.05.06 ~ 2022.05.13
* 3명 : [이다혜](https://github.com/ekgpgdi), [김지호](https://github.com/kimziaco?tab=repositories), [김대희](https://github.com/eet43)
<br/>

## 2. 사용 기술 
<b>```Back-end```<b/>
 
* Flask
* boto3 <br/>
* requests <br/>
* pymongo <br/>

<b>```Front-end```<b/>

- HTML
- Bootstrap
- JavaScript

## 3. Data Model Design - Embedded Data Models

![image (2)](https://user-images.githubusercontent.com/88760828/186060695-0a689fcb-9f88-41c0-a1db-a609f8d44530.png)

![스크린샷 2022-08-23 오전 11 37 37](https://user-images.githubusercontent.com/88760828/186060731-337dad08-6e46-4b74-85d0-497c859cd252.png)

![스크린샷 2022-08-23 오전 11 37 55](https://user-images.githubusercontent.com/88760828/186060742-1f000113-c53f-4c07-b8bf-37e1f5bef518.png)



## 4. 아키텍처
<p align="center">
<img width="786" alt="Devit(python)Architecture" src="https://user-images.githubusercontent.com/88760828/185904373-3545ffdc-5547-4380-ad03-65484fb71d48.png">


  </p>

## 5. 핵심 기능

![devit(python)클래스다이어그램](https://user-images.githubusercontent.com/88760828/186060808-4c5e5674-d374-40ae-b400-4887edfab375.png)


## 6. 핵심 트러블 슈팅 

1. EC2 ubuntu18 버전을 사용하여 python3.6으로 다운이 되면서 필요한 라이브러리가 설치되지 않는 문제
버전이 낮아 python 버전이 3.6으로 다운되는 문제 
(프로젝트 내 버전 3.8 로 패키지들의 설치 ~~)

2. EC2 내에서 환경변수를 어떻게 지정할까? 라는 의문으로 시작되어 config 파일을 통한 환경 분리
