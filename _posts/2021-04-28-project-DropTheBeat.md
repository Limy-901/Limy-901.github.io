---
layout: post
title:  "드랍더비트 (Drop the Beat)"
date: 2021-04-28
desc: "드랍더비트"
keywords: "Lyim, Java, EditPlus, Project, Game, Socket"
categories: [Project]
tags: [Java,Game,TCP]
icon: icon-html
---



***

<center>
<br>
<h2 style="font-weight:400">🤸 Only 자바로 만든 음악 가사 타이핑 게임 🎵</h2><br><br>
<p> 드랍 더 비트는 자바만 활용하여 만든 타이핑 게임입니다.<br>&nbsp;참가자들은 즐겁게 채팅을 하며, 랜덤하게 흘러나오는 음악을 듣게 됩니다. <br> 해당하는 노래의 가사를 가장 먼저 타이핑하여 맞추는 사람이 승리하고 점수를 가져가게 됩니다.</p><br><br><br>
<h2><b>✨프로젝트 개요</b></h2><br>
<p><img style="width:600px;" src="\static\assets\img\blog\project\dropTheBeat\team.jpg"></p>
<img src="\static\assets\img\blog\project\dropTheBeat\dropthebeat-stack.jpg"><br><br><br>
<p> * <b>프로젝트 형태</b> : 비트 조, 총 4명, 팀장</p>
<p> * <b>프로젝트 기간</b> : 20.11.21 ~ 20.11.27</p>
<p> * <b>📂Git hub</b> : <a href="https://github.com/Limy-901/Project_1st">Repository</a></p>
<p> * <b>✨담당 파트</b> : <a href="">서버-클라이언트 TCP 통신, 디자인</a></p>
</center><br><br>

<hr>

<center>
<br><br>
<h1 style="font-weight:400">게임 시연 영상</h1><br>
<iframe width="944" height="531" src="https://www.youtube.com/embed/0RPn5Eq7_Sk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><br><br><br>
<hr><br><br><br>

<h2><b>통신 프로토콜</b></h2><br><br>
<img style="width:800px" src="\static\assets\img\blog\project\dropTheBeat\protocol.PNG"><br>
<p><b> 서버와 클라이언트간 소통할 프로토콜</b><br>- 채팅, 게임 시작, 끝, 게임초기화, 장르 선택자, 점수 카운트 등</p><br><br>
<hr>

<h2><b>게임 접속</b></h2><br><br>
<img style="width:800px" src="\static\assets\img\blog\project\dropTheBeat\drop0.PNG"><br><br>
<img style="width:700px" src="\static\assets\img\blog\project\dropTheBeat\game0.PNG"><br>
<p style="font-size:1.8rem;"><b>서버소켓, 소켓, 스레드</b></p>
<p>- 서버가 오픈되어 있을 시, 다수의 클라이언트가 접속하여 게임 시작 가능<br>
- 최대 인원 수, 게임 중 참여 불가 등 조건 있음</p><br><br>
<hr>

<h2><b>게임 시작</b></h2><br><br>
<img style="width:700px" src="\static\assets\img\blog\project\dropTheBeat\drop1.PNG"><br><br>
<img style="width:700px" src="\static\assets\img\blog\project\dropTheBeat\start0.PNG"><br><br>
<p style="font-size:1.8rem;"><b>전원 Ready, 랜덤 클라이언트 선정, 랜덤 음악 재생</b></p>
<p>- 참여자 전원이 Ready 해야 게임 시작<br>
- 참여자 중 랜덤으로 한 명 선정하여 장르 선택<br>
- 선택 된 장르의 음악 중 랜덤으로 한 곡 선정<br>
- 해당 곡의 음원 재생 + 문제 + 해당 아티스트 이미지</p><br><br>
<hr>

<h2><b>정답 및 카운트 & 반복</b></h2><br><br>
<img style="width:700px" src="\static\assets\img\blog\project\dropTheBeat\drop2.PNG"><br><br>
<p style="font-size:1.8rem;"><b>채팅 창에 정답 입력 > 체크 > 카운트 > 랜덤 재생</b></p>
<img style="width:600px" src="\static\assets\img\blog\project\dropTheBeat\check.PNG"><br>
<p>- 참여자가 채팅창에 입력하면, 정답인지 채팅인지 구분<br><br>
<img style="width:600px" src="\static\assets\img\blog\project\dropTheBeat\answer2.PNG"><br>
<p style="margin-bottom:15%;">- 정답일 때, 해당 참여자에게 점수 + 1, 이후 다시 랜덤 재생<br></p>