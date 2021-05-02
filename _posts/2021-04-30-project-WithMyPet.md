---
layout: post
title:  "위드마이펫 (With My Pet)"
date: 2021-04-30
desc: "반려동물 산책 및 통합 웹 사이트"
keywords: "Lyim, Pet, Java, Spring, Ajax, Project, WebSocket"
categories: [Project]
tags: [Java,Web,Project,Spring,WebSocket,Pet,Ajax]
icon: icon-html
---



***

<center>
<br>
<img style="width:10%;" src="\static\assets\img\blog\project\withMyPet\footprint.png"><br><br><br>
<h2><b>프로젝트 개요</b></h2><br>
<img style="width:60%;" src="\static\assets\img\blog\project\withMyPet\team.jpg"><br><br><br>
<p style="font-size:1.8rem;">: <b>위드마이펫</b> 은 총 6명의 팀원이 함께 구현한 파이널 프로젝트로,<br>&nbsp; 반려인들이 쉽게 동네에서 산책 친구를 구하고 쇼핑, 커뮤니티 등<br>다양한 서비스를 사용할 수 있도록 기획한 반려동물 통합 웹 애플리케이션 입니다.</p><br><br><br>
<img style="width:70%;" src="/static/assets/img/blog/project/withMyPet/stack.jpg"><br><br><br>
<p> * <b>프로젝트 형태</b> : 함께해조 팀, 총 6명, 팀장</p>
<p> * <b>프로젝트 기간</b> : 21년 1월 ~ 21년 3월</p>
<p> * <b>📂GitHub</b> : <a href="https://github.com/Limy-901/WithMyPet">Repository</a></p>
<p> * <b>✨담당 파트</b> : <a href="#walking">1.산책,</a>&nbsp;&nbsp; <a href="#admin">2.관리자</a></p>
<p> * <b>🔗프레젠테이션</b> : <a href="https://drive.google.com/file/d/1OBVH8dNmR0AI3Y4h1XBVWe9_EoPdy4I4/view?usp=sharing">PDF 다운로드</a></p>
</center><br><br>
<hr>
<center><br><br>
<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;초기 흐름&nbsp;</b></code>
<br><br>
<img style="width:70%;" src="\static\assets\img\blog\project\withMyPet\flow.jpg">
<p style="margin-bottom:10%;"></p>
<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;DB 설계&nbsp;</b></code>
<br><br>
<img style="width:70%;" src="\static\assets\img\blog\project\withMyPet\DB.jpg">
<p style="margin-bottom:10%;"></p>
<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;시연 영상&nbsp;</b></code>
<br><br>
<div class="embed-container">
<iframe style="width:100%" src="https://www.youtube.com/embed/E7_hEN3_wmA" title="YouTube video player" frameborder="0" onLoad="setIFrameHeight(this)" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen ></iframe>
</div><p style="margin-bottom:10%;"></p>


<hr><br><br>
<code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;1. 산 책&nbsp;</b></code>
<br><br>
<p><p style="font-size:2rem; font-weight:600">1-1 산책 목록</p><br>
<p>
<img style="width:50%;" src="\static\assets\img\blog\project\withMyPet\login.JPG"><br>
<img style="width:50%;" src="\static\assets\img\blog\project\withMyPet\walking.JPG"><br>
<img style="width:50%;" src="\static\assets\img\blog\project\withMyPet\make.jpg"><br>
<br>
<iframe style="width:100%"  src="\static\assets\img\blog\project\withMyPet\1-walklist.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe></p><br><br>
    <p>
        <b>산책 개설 및 검색</b> : (로그인 서비스) 지역, 제목, 내용, 전체로 검색 가능<br>
        <b>Kakao Map API</b> : 원하는 지역 검색하여 개설<br>
        <b>날짜 표기</b> : 타임스탬프 타입에서 년/월/일/시 표기법으로 변환(SimpleDateFormat)<br>
        <b>페이지네이션</b> : 한 페이지마다 5개의 산책글 확인 가능<br>
        <b>산책 데이터</b> : 회원(마이페이지) 테이블과 JOIN하여 회원 사진 불러오기<br>
        <b>참가자 여부</b> : 참가 테이블과 JOIN - 참가자 0명인 경우, '기다리고 있어요!' 태그 부착<br>
        <b>Kakao 공유 API</b> : 메시지로 상세페이지로 이동하는 URL 전송<br>
        <b>Ajax</b> : 검색 기능 사용시 검색 결과 비동기 갱신<br>
    </p>
</p>
<p style="margin-bottom:15%;"></p>

<p style="font-size:2rem; font-weight:600">1-2 산책 모집글, 공유하기</p>
<br>
<p><iframe style="width:100%"  src="\static\assets\img\blog\project\withMyPet\2-look&share.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\3-share2.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<p>
    <b>산책글</b> : (작성자인 경우) 수정, 삭제 가능<br>
    <b>주최자 정보</b> : 회원, 반려동물 상세정보, 총 산책 횟수(통계), 팔로우, 팔로워 수, 최근 받은 리뷰<br>
    <b>Kakao Map API</b> : 작성된 지역으로 MAP 위치 표시
</p>
</p><p style="margin-bottom:15%;"></p>

<p style="font-size:2rem; font-weight:600">1-3 참가 신청자 보기, 좋아요, 참가 신청</p>
<br>
<p><iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\4-look1.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\5-heart.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\6-join.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br>
<p>
    <b>좋아요</b> : 로그인 시에만 좋아요 가능, 좋아요 테이블 INSERT<br>
    <b>참가자 / 신청자</b> : 신청 > 작성자 승인 > 참가의 순서, 해당 회원의 정보 표기<br>
    <b>산책 참가 신청</b> : 하단 버튼 클릭 후 메시지 작성 > 참가 테이블에 INSERT<br>
    <b>Ajax</b> : 좋아요 및 참가 신청 Ajax로 비동기 갱신<br>
</p>
</p><p style="margin-bottom:15%;">

<p style="font-size:2rem; font-weight:600">1-4 메시지 기능</p>
<br><p>
<img style="width:25%;" src="\static\assets\img\blog\project\withMyPet\socket.jpg">&nbsp;&nbsp;<img style="width:45%;" src="\static\assets\img\blog\project\withMyPet\socket2.jpg"><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\7-search.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\8-socket.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe>
<br><br>
<p>
    <b>WebSocket</b> : 로그인 시, 세션 아이디로 소켓 연결되어 매 페이지 연동(실시간 메시지 알림)<br>
    <b>(좌측) 메시지 상대 검색</b> : 사용자 명으로 메시지 상대 검색 가능<br>
    <b>(좌측) 최근 메시지 기록</b> : 대화 상대, 마지막 메시지 경과시간, 내용, 읽음 여부 표시<br>
    <b>(우측)</b> : 상대 선택시, 나눈 대화 리스트, 첫 메시지의 경우 첫 메시지임을 알려줌<br>
    <b>Toastr</b> : 메시지 수신 시, 우측 상단에 알림 표시 라이브러리<br>
    <b>Ajax</b> : 모든 Message 페이지 Ajax로 비동기 갱신
</p>
</p><p style="margin-bottom:15%;"></p>

<p style="font-size:2rem; font-weight:600">1-5 산책 약속 잡기, 후기 남기기</p>
<br><p>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\9-joinchat.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\10-review.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br>
<p>
    <b>주최자에게 메시지</b> : 산책글에서 버튼 클릭시, 해당 회원과의 메시지로 바로 이동, 구체적 약속 잡기<br>
    <b>후기 작성 알림</b> : 상대와의 미작성 산책이 있을 경우에만 알림 (산책 테이블, 후기 테이블 JOIN)<br>
    <b>산책 한줄평</b> : 상대의 산책 정보에 입력 될 한줄평 입력<br>
    <b>SweetAlert2</b> : 한줄평 작성 Modal, 확인 Modal<br>
</p>
<p style="margin-bottom:15%;"></p></p><br><hr>

<br><br><code style="background-color:#7fa6ef; font-weight:100; font-size:2em; color:white" class="language-plaintext highlighter-rouge"><b>&nbsp;2. 관리자&nbsp;</b></code>
<br><br><br>
<p style="font-size:2rem; font-weight:600">2-1 메인 통계</p>
<br><p>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\11-admin.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<p>
    <b>통 계</b> : 일일 전반 통계, 산책 매칭 확률, 주간 그래프, 인기 판매 목록, 최근 판매 내역<br>
    <b>Chart.js</b> : 그래프 표시 - 산책, 판매(Line), 인기리스트(Doughnut)
</p>
<p style="margin-bottom:15%;"></p></p><br>

<p style="font-size:2rem; font-weight:600">2-2 회원 관리</p><br><p>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\12-member.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<p>
    <b>Ajax</b> : 회원 강제 탈퇴, 산책 포인트 지급 후 Ajax 통신으로 비동기 갱신<br>
    <b>SweetAlert2</b> : 산책 포인트 지급 Modal
</p>
<p style="margin-bottom:15%;"></p></p><br>

<p style="font-size:2rem; font-weight:600">2-3 산책 현황, 문의 답변, 서비스 통계</p>
<br><p>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\13-recentwalk.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\15-question.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<iframe style="width:100%" src="\static\assets\img\blog\project\withMyPet\16-statistics.gif" frameborder='0' scrolling='no' width='640px' height='360px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe><br><br>
<p style="margin-bottom:15%;"></p></p><br>