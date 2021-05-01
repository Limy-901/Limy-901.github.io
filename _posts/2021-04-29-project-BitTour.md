---
layout: post
title:  "비트투어 (Bit Tour)"
date: 2021-04-29
desc: "여행 상품 패키지 예약 웹 서비스"
keywords: "Lyim, Trip, Java, Eclipse, Project"
categories: [Project]
tags: [Java,Eclipse,Project]
icon: icon-html
---



***

<center>
<br><h2 style="font-weight:400">🛫 여행 상품 패키지 예약 웹 서비스 🌍</h2><br>
<img style="width:20%;" src="\static\assets\img\landing\pj-2.jpg"><br><br><br>
<p>: 비트 투어는 학원에서 진행된 세미 프로젝트입니다.<br>&nbsp;처음으로 서버와 클라이언트를 나누고 MVC 모델을 익히는 단계에서 진행 된 프로젝트로,<br>코로나 시대 여행에 대한 그리움을 달래보고자 진행하였습니다.</p><br><br><br>

<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;프로젝트 개요&nbsp;</b></code><br><br>
<p><img style="width:40%;" src="\static\assets\img\blog\project\dropTheBeat\team.jpg"></p>
<img style="width:40%;" src="\static\assets\img\blog\project\bitTour\stack.jpg"><br><br><br>
<p> * <b>프로젝트 형태</b> : 비트 조, 총 4명, 팀장</p>
<p> * <b>프로젝트 기간</b> : 20.12.08 ~ 20.12.15</p>
<p> * <b>📃데이터베이스 설계</b><br><img style="width:50%;" src="\static\assets\img\blog\project\bitTour\erd.png"></p>
<p> * <b>📂Git hub</b> : <a href="https://github.com/Limy-901/Project_2st">Repository</a></p>
<p> * <b>✨담당 파트</b> : 랜딩 페이지, 상세 페이지, 답변형 문의 게시판</p>

</center><br><br>
<hr>
<center><br><br>

<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;시연 동영상&nbsp;</b></code><br><br>
<iframe width="760" height="398" src="https://www.youtube.com/embed/hXfMJq8fkvA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<p style="margin-bottom:10%;"></p>
<hr>
<br><br><br><br><code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;랜딩 페이지&nbsp;</b></code><br><br>
<img style="width:80%;" src="\static\assets\img\blog\project\bitTour\1.png"><br><br>
<p><b>디자인</b> : HTML5와 CSS3를 이용하여 화면 구성</p>
<p><b>상단 메뉴</b> : 서비스 목록, 로그인 기능</p>
<p><b>여행지 선택</b> : 해당 여행지 상세 설명 페이지로 이동</p>
<p style="margin-bottom:10%;"></p>
<hr>

<br><br><br><br><code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;상세 페이지&nbsp;</b></code><br><br>
<img style="width:10%;" src="\static\assets\img\blog\project\bitTour\2-1.png">
<img style="width:10%;" src="\static\assets\img\blog\project\bitTour\2-3.png">
<img style="width:10%;" src="\static\assets\img\blog\project\bitTour\2-2.png"><br><br><br>
<p><b>디자인</b> : Semantic UI 라이브러리를 활용하여 화면 구성</p>
<p><b>예약 버튼</b> : 로그인 시에만 예약 서비스로 이용 가능</p>
<p style="margin-bottom:10%;"></p>
<hr>
<br><br><br>
<div style="width:80%;">
<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;답변형 문의 게시판&nbsp;</b></code></div><br><br><br>

<h3 style="font-size:2.5rem; color:#7fa6ef;">1. 게시글 리스트</h3>
<img style="width:80%;" src="\static\assets\img\blog\project\bitTour\3-1.jpg">
<p><b>회원 여부 체크</b> : (Session 체크) 로그인 시에만 접근 가능한 게시판</p>
<p><b>문의글 / 답변글 구분</b> : (게시글의 Level 체크) 답변 글은 좌측에 답변 아이콘과 작성자에 관리자 이름이 붙음</p>
<p><b>페이지네이션</b> : (Select By ROWNUM) 페이지 당 5개의 게시글을 볼 수 있음</p><br>

<br><br><h3 style="font-size:2.5rem; color:#7fa6ef;">2. 회원 - 문의글 작성</h3><br>:
<img style="width:80%;" src="\static\assets\img\blog\project\bitTour\3-2.png">
<p><b>작성자</b> : (Session에 담긴 회원정보) 현재 세션의 로그인 되어 있는 회원명</p>
<p><b>작성일</b> : 현재 시스템 시간</p><br>


<br><br><h3 style="font-size:2.5rem; color:#7fa6ef;">3. 관리자 - 답변글 작성</h3><br>
<img style="width:80%;" src="\static\assets\img\blog\project\bitTour\3-3.png">
<p><b>문의글 내용</b> : (클릭한 문의글 내용) 답변시에 참고할 수 있음</p>


<br><br><h3 style="font-size:2.5rem; color:#7fa6ef;">4. 관리자 - 답변글 확인</h3><br>
<img style="width:80%;" src="\static\assets\img\blog\project\bitTour\3-4.png">
<p><b>수정 & 삭제</b> : (게시글 CRUD) 답변이 완료 된 게시물에 대하여 수정, 삭제가 가능</p>
<p style="margin-bottom:5%;"></p>


