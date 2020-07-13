<p>This is what I created while learning 'WEB1 - HTML & Internet' lecture of www.opentutorials.org</p>
<p>www.opentutorials.org의 'WEB1 - HTML & Internet' 강의를 학습하면서 만든 내용입니다.</p>

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

