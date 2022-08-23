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

 1. EC2 AMI ubuntu 버전 차이로 인한 python 버전 불일치 문제</br>
- EC2 AMI의 ubuntu 버전을 18.04 LTS 로 지정하여 python version 이 3.6으로 설치가 되었고 그로 인해 프로젝트 python 3.8 버전과 일치하지 않아 requirements.txt에 작성한 패키지 버전들과 호환 오류 발생
- 처음에는 pip 로 python 3.6에서 사용 가능한 패키지 버전들로 다운그레이드하여 설치함으로써 불필요한 작업이 발생
이후 ubuntu 버전 차이라는 것을 인지하고 ubuntu 버전을 20.04 LTS 로 변경하여 해결
 
2. 추가 작업 없는 배포를 고민</br>
- Local 환경에서 작업하던 프로젝트를 어떻게 추가 작업없이 CI/CD 의 장점을 이용하여 EC2에 배포할 수 있을까 라는 고민을 시작
- 환경 변수 분리를 위해 Prod 환경과 Local 환경의 환경 변수들을 config 파일로 분리
