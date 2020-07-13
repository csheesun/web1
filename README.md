<p>This is what I created while learning 'WEB1 - HTML & Internet' lecture of www.opentutorials.org</p>
<p>www.opentutorials.org의 'WEB1 - HTML & Internet' 강의를 학습하면서 만든 내용입니다.</p>

- aws community heroes - 제도 - 글로벌 전문가로 성장 가능 

- 페북/슬랙을 통해 초보자 도와 주기 slack.awskr.org

- 테스트 및 프로토 타입 만든 거 공유 

- aws Korea youtube 채널 

​

https://yah.ac/aws

# AWS 야학 1일차 - 기본 (다시 안봐도 됨) 

 aws educate 

남의컴퓨터 빌려서 원격 제어를 통해서 사용, 컴퓨터 입대업 ex) EC2

확장 : 서버 컴퓨터에 동작하는 소프트웨어 설치, 운영, 백업(위험한 일임), 보안 까지 대신해 줌 ex) RDS : MySQL, SQL Server, Oracle 이걸 서비스 형태로 제공해줌. 직접 설치 안함 

물론 EC2 안에 MySQL, SQL Server, Oracle 설치해도 된다. 



host, hosting 

사용량이 매우 적거나 매우 많을 떄 클라우드 유용 

​

맥에서 윈도우 쓰고 싶을 때 : Cloud Computing 으로 가능 

목표설정 - 목표설정에 맞는 서비스 찾기 - 요금 따져보기 

프리티어 750 시간: 여러 컴퓨터 띄워도 750 시간만 안넘으면 상관 없다는 거임 



# AWS 야학 2일차 - 기본 

AWS1 – 8. 원격제어 (따라하기) 

키페어 잃어버렸을 때

똑같은 키페어와 같은 키페어는 발급되지 않는다. 

<stong> 인스턴스를 복제한 뒤에 그 인스턴스에 새로운 키페어를 발급해줘야 함 </stong>

​

AWS1 – 9. 서비스 끄기 EC2

질문 : 750 시간 넘어도 1년 동안은 무료라는 건지? 750시간 넘으면 1년 무관하게 바로 과금인지? 

<stong> 
주의 : 
인스턴스 중지 : 데이터는 유지함. 이걸 하기 위해 아주 약간 과금
인스턴스 종료 : 데이터 날아감. 추가 과금 없음. 
 
 여러분이 컴퓨터를 끄면 ip 가 해소되고 요 다시 키면 다른 ip 가 부여 돼요 그렇기 때문에 여러분이 예전에 세팅해 놓은 방법 그대로 접속할 수 없고
 접속하는 방법을 다시 재 설정을 해주셔야 됩니다. '연결' 을 다시 해야 함 
</stong>

10. budget 정해 놓을 수 있다.


11. OTP(one time password) <stong> 다시 보기 </stong>

IAM -> MFA 
로그인 – MFA(아이디+비번+OTP) 코드 
'Activate MFA on your root account' 따라하기 -> 활성화 됐는지 확인 -> 로그인 할 때 MFA 뜨는 지 확인 

TODO : <기기가 없어서 일단 패스> 

​

13. 수업을 마치며 <stong> 다시 보기 </stong>

- S3 시범(따라하기 완료) - 파일을 'make public' 으로 만들기 

- CLI 로 S3 에 파일업로드 시범 
<strong> aws s3 cp [filename] s3://[bucket name] </strong>
<strong> aws s3 cp hello-cli.txt s3://coding-everybody </strong>

- 프로그래밍(코드)으로 aws 제어 시범(이게 sdk 임?)

​

3일차 

3일차 

s3

내 파일이 하나의 리전의 3개 이상의 az 에 복제됨 

파일서버로 사용 가능 

​

폴더 이름 못바꿈 

​

--------

오픈스택을 쓰면 맞춤형 클라우드 구축가능

오픈스택을 비즈니스/연구용으로 이용시 꺼리게 되는 점이 있다면 바로 난이도(진입장벽)가 높다는 것 

​

Usage 별로 best practice 를 template 으로 제작하여 클라이언트의 시간과 비용 절감에 도움 주기 위함임 

​

목표 

서버 인프라 구성 리눅스용 배포판용 

기업용/연구기관용 서버환경 구축 

​

비용 예측

하드웨어 대여 서비스 

하드웨어 설계 자동화 

공정/품질 개선

​

- 클라우드 배포환경을 위한 클라우드 서비스 조합 추천

- 클라우드 사용전 비용 예측 

- open stack 기반 cloud 구축 template 탬플릿 

첫 번째 template : 기업/연구소를 위한 데이터 관리에 특화된 클라우드 

​

​

개발언어 : 



# AWS 야학 5일차 - 웹의 기초 (다시 안봐도 됨) 
Textedit - 맥 <br>
gedit - 리눅스 <br>

html 파일 열기 <br>
command + o <br>
control + o <br>

저장 <br>
command + s <br>
Control + s <br>
https://www.youtube.com/watch?v=aUtnyev_1vg&list=PLORxAVAC5fUWLRAQ88k6iFvFb2u4HNDGJ&index=12

## 웹 페이지들이 몇 개의 html 태그로 이뤄져 있는지, popular tag rankings
https://www.advancedwebranking.com/html/#faq

## tags 
```html
<strong> : 강조
<u> : 밑줄
<br> : 줄바꿈 (닫는 태그 따로 없다.) 
<p> : 단락 (닫는 태그 있음)
<img source="coding.jpg" width="100%"> : 이미지 추가 
<img width="400" src="coding.jpg"> : 이미지 추가 
<ul> : 번호 자동 매김 없음 
  <li>
<ol> : 번호 자동 매김 
  <li>
    
<table>
  <tr> 
    <td>head</td>
    <td>98.1%</td>
  </tr>
  ...
<table>
  
<a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 speiclal">Hypertext</a>
  
<!doctype html>
<html>
<head>
  <meta charset="utf-8">
  <title>
<body>
```
<p>
코드에서 엔터 두 번 하는 거 의미 없음 <br>
단락을 쓸거면 p tag 쓸것. 단락을 정보로서 가치있게 만들기 떄문(검색용이) <br>
br은 띄우고 싶은 만큼 넣으면 됨 <br>
p 단점 : 정해져 있는 여백 만큼 벌어지니 자유도 떨어짐 <br>
  
## attribute 
source="coding.jpg" 같은거 <br>
attribute 끼리는 순서가 바뀌어도 무관 

해결 : 
```html
<p style=”margin-top:40px;”>
```
</p>

HTML을 의미에 맞게 정확하게 사용하는게 중요 (검색에 노출되기 위해서) <br>
accesibility.(장애인) <br>
예쁘게 하려고 문자까지 넣어서 통으로 이미지로 만들면 시각장애인에게는 없는 정보가 된다. <br>
추천 : <strong>unsplash.com</strong> : 저작권에 구애받지 않는 무료 이미지 다운가능 

## 11강 
부모 자식 관계에 있는 태그 있다. 꼭 같이 써야 하는 거 있다. <br>

한번에 여러개 수정 <br>
atom 기준, command(ctrl) + 클릭 <br>
태그는 반드시 부모 태그를 갖고 있다. <br>

그 항목이 어디서부터 어디까지가 서로 연관된 항목인지를 <br>
경계를 짓기 위한, 그룹핑을 하기 위한 부모 태그가 필요한 것이죠 <br>

그래서 li 태그는 반드시 부모 태그를 갖고 있다 <br>
그리고 부모 태그인 ul 태그는 반드시 자식 태그를 가지고 있다. <br>  
마지막 - 링크되는 웹 사이트 만듦 <br>

공 https://www.w3.org/TR/html51/ <br>

# AWS 야학 6일차 - S3를 서버로 활용하기 (마지막 2개 강의를 다시 보기) 
https://www.youtube.com/playlist?list=PLORxAVAC5fUWwD0ueuPNmFuu2OaIohK8u

s3 를  웹서버로 활용하기 

cloudfront = 
cache server (웹 서버 부담 경감) + 
cdn (세계화, 컨텐츠 신속 배달) 

http://web1-html-internet-heesun.s3-website.ap-northeast-2.amazonaws.com/

dsuqwuqbq9rch.cloudfront.net

(수업에는 ec2 이용, 나는 s3 로 cloudfront 로 만듦) 

# AWS 야학 7일차 - cloudfront를 이용해서 전세계에 배포하기 - 7일차 
https://www.youtube.com/playlist?list=PLORxAVAC5fUU_gsWiwA9KprDxIxR_M7eg

6일차 문제 : origin은 바뀌었는데 distribution 에는 바로 반영 안되는 문제 
지금 cache control 로 해결 

# 앞으로 해볼 만한 거 
cache 강의 수강
ec2 기반으로 Cloudfront 만들어 보기 

