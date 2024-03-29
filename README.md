# **FinalProject_MusicStage**
## 음악통합커뮤니티 MusicStage

### :raising_hand_woman: Project Team Member :raising_hand_man:
> :thumbsup: Team Leader : 이서영 <br>
> :v: Team Member : 김형준, 정규동, 최하윤, 김연우<br>

### :hammer_and_wrench: Project Part
> :sunny: 서영<br>
게시판 FeedType<br>
게시판 Modal<br><br>
> 	:star: 형준<br>
회원가입/로그인<br>
아이디/비밀번호찾기<br>
전문가 등록<br><br>
> :zap: 규동<br>
회원가입/로그인<br>
마이페이지/정보수정<br>
회원탈퇴<br><br>
> :crescent_moon: 하윤<br>
게시판 BoardType<br>
게시판 상세보기<br>
사이드바 Menu<br>
글쓰기/글수정<br>
댓글입력/삭제<br><br>
> :snowflake: 연우<br>
관리자페이지<br>
홈페이지 알람<br>
채팅<br>


### :building_construction: Development schedule (2020.09.21 ~ 2020.12.21)
> 프로젝트 기획 : 2020.09.21 ~ 2020.09.26<br>
> UI회의 / 설계 : 2020.09.27 ~ 2020.10.11<br>
> DB회의 / 설계 : 2020.10.12 ~ 2020.10.16<br>
> UI제작 / DB검토 : 2020.10.17 ~ 2020.11.09<br>
> 프로젝트 구현 : 2020.11.09 ~ 2020.12.11<br>
> 통합 테스트 : 2020.12.06 ~ 2020.12.21<br>

### :computer:  Development Environment
> Development Tool : Eclipse 4.15.0, sqlDeveloper<br>
> Server : Apache Tomcat 9.0<br>
> Database : Oracle 11g<br>
> Development Language : JAVA , HTML5, CSS3, JavaScript, jQuery, SQL, JSP, Servlet<br>
> Team Coop : GitHub, ERDCloud, kakaoOven<br>
> API : Kakao Maps API, Kakao Login API, Daum(Kakao) Map PostCode API, bxSlider API<br>

### :mag: Development Background
> #### 음악 대통합 커뮤니티<br>
> 코로나 19로 인하여 뮤지션의 무대가 줄어들고,<br>
> 공동 작업에 어려움이 생겨 오프라인이 아닌<br>
> 온라인 작업 환경의 중요도가 증가하였습니다.<br>
> 이러한 배경을 가지고 온라인에서도 오프라인과 같은 활동 공간이 주어진다면<br>
> 이 시기를 이겨낼 수 있지 않을까? 하는 생각으로 개발하게 되었습니다.<br>

###  Implementation Goal
> - 소셜 기반 게시판과 메신저를 이용한 자유로운 소통입니다.<br>
> 게시판 내 댓글과 쪽지로만 회원간의 소통이 이루어져 소통하는데 답답함이 따르는 문제를 해결하고자 했습니다.
> - 관심 분야에 따른 친구 매칭 서비스 입니다.<br>
> 관심 분야를 선택함으로써 비슷한 관심 분야인 회원을 추천받고,
> <br> 관심 분야에 맞는 게시글을 선택해 사이트를 효율적으로 이용할 수 있도록 했습니다.
> - 현재 SNS UI를 차용한 감각있는 사이트입니다.<br>
> 개인 작업물을 보기 좋은 형식으로 보관하고 공유할 수 있도록 UI를 구현하고자 했습니다.

###  Implementation Screen
#### :punch: Logo <br>
![STAGE로고](https://user-images.githubusercontent.com/66005208/103438161-61c23680-4c73-11eb-8435-3176b412d837.png)<br>
음악커뮤니티 답게 로고를 높은음자리표를 이용해서 오선지에 글자를 넣어 제작하였습니다<br><br>

#### :punch: Side Bar<br>
![사이드바](https://user-images.githubusercontent.com/66005208/105624787-b702f980-5e67-11eb-99b9-68a5266d73fa.jpg)<br>
화면이 아닌 기능만 구현하였으며 사이드 바는 home / 소식 / 팔로우 / 보관함 / 팔로우 목록 / footer로 이루어져 있습니다.<br>
메뉴들은 클릭하면 맞는 게시판으로 넘어가게 되고 팔로우 목록은 사용자가 팔로우 한 사용자의 YouStage(마이페이지)로 넘어가게 됩니다.<br>
더보기 버튼을 클릭시 사용자가 팔로우한 목록이 한꺼번에 나타나게 됩니다.<br><br>


#### :punch: Board - Tumbnail Type<br>
![팔로우](https://user-images.githubusercontent.com/66005208/105624794-c8e49c80-5e67-11eb-9e3d-088ac7e5de3a.jpg)<br>
각 게시판별로 FeedType과 Thumbnail Type으로 나뉘게 되는데 제가 맡은 부분은 Thumbnail Type입니다.<br>
썸네일과 제목 작성자프로필사진과 닉네임, 조회수가 나타나게 됩니다.<br>
1에서 6번째의 게시물만 받아 온 후 스크롤을 내릴때 처음 가져온 값들 제외 리스트가 남아있을 경우<br> 
ajax를 이용해서 남은 게시글 6개를 더 가져오게 됩니다.<br>
반복적으로 리스트가 남아있지 않을 경우까지 진행하여, 만약 게시글이 남아있지 않을 경우<br>
더 이상 표시할 게시글이 없습니다 라는 팝업창을 띄우게 됩니다.<br><br>


#### :punch: Search<br>
![검색](https://user-images.githubusercontent.com/66005208/105624802-d69a2200-5e67-11eb-9484-c69a44a8f0b6.jpg)<br>
검색기능은 원하는 카테고리와 원하는 제목검색어를 입력 후 검색아이콘을 클릭하면 BoardType으로 게시글 목록이 나타나게 됩니다.<br> 
처음화면에는 6개의 게시물만 나타나게 되고 스크롤바를 내릴 시 검색한 게시글의 목록이 남아있으면 나타나게 됩니다.<br><br>


#### :punch: Board Write<br>
![글쓰기1](https://user-images.githubusercontent.com/66005208/105624806-e31e7a80-5e67-11eb-8b85-ba822911d3cb.jpg)
![글쓰기2](https://user-images.githubusercontent.com/66005208/105624809-e580d480-5e67-11eb-90ea-44846092309c.jpg)
![글쓰기3](https://user-images.githubusercontent.com/66005208/105624810-e6b20180-5e67-11eb-9e7b-bb2641d406d1.jpg)
![글쓰기4](https://user-images.githubusercontent.com/66005208/105624812-e9145b80-5e67-11eb-8e79-9cce5c9d34a0.jpg)<br>
제목과 카테고리와 설명은 무조건 작성해야합니다.<br>
썸네일은 등록을 무조건 해야 하지만 만약 등록하고 싶지 않을 시<br>
등록버튼을 클릭했을 때 기본이미지로 등록이 된다는 confirm창이 뜨고 확인버튼을 클릭하면 기본이미지로 등록이 됩니다.<br>
이미지와 음악파일은 선택적으로 등록할 수 있습니다. 이미지는 각 한칸 당 한 사진만 등록할 수 있으며 이미지확장자만 등록이 가능합니다.<br> 
음악파일은 여러 개 등록이 가능며 음원확장자만 등록이 가능합니다.<br>
영상파일과 커리큘럼도 선택적으로 등록할 수 있습니다. <br>
영상파일은 음악파일과 마찬가지로 여러 개 등록이 가능하며 영상확장자만 등록이 가능합니다.<br> 
커리큘럼은 텍스트만 입력이 가능합니다.<br>
마지막으로 장소와 제공형식 역시 선택적으로 등록이 가능합니다.<br> 
장소는 주소검색버튼을 클릭 시 주소 입력창이 나타나게 되고 검색 후 선택하게 되면 화면에 장소가 나타나게 됩니다.<br>
제공형식은 원하는 키워드로 콤마를 사용해서 입력해야 합니다.



#### :punch: Board Detail<br>
![상세보기1](https://user-images.githubusercontent.com/66005208/105624817-ef0a3c80-5e67-11eb-97cf-c731add411af.jpg)
![상세보기2](https://user-images.githubusercontent.com/66005208/105624819-f0d40000-5e67-11eb-8576-89e9e6972f25.jpg)
![상세보기3](https://user-images.githubusercontent.com/66005208/105624820-f16c9680-5e67-11eb-9e0a-478d60d91c9b.jpg)<br>
맨 위 상단은 선택한 카테고리가 나타납니다. 썸네일과 제목 작성일 조회수가 나타나고<br>
바로 밑엔 작성자 프로필사진과 닉네임이 나타납니다. 작성자가 로그인 유저일 경우 삭제와 수정버튼이 나타나고<br>
작성자가 로그인 유저가 아닐경우 신고하기와 메시지보내기와 YouStage버튼이 나타납니다.<br> 
설명에는 작성했던 설명텍스트가 나타납니다. 밑에는 등록한 사진과 음악파일과 영상이 나오게 제작하였습니다.<br>
사진은 최대 4개가 나오게 되며 영상과 음악파일은 등록한 갯수만큼 나오게 됩니다.<br>
음악파일은 등록 시 플레이어가 나타나도록 구현하였으며 영상파일은 가로가 720px로 고정되어 나오게 구현하였습니다.<br>
장소는 사용자가 등록했던 위치가 마커로 표시되며 그 위에는 주소가 함께 나오게 하였습니다.<br> 제공형식은 등록했던 키워드로 나타납니다.<br>
마지막으로 댓글은 댓글 입력한 사용자의 프로필사진과 닉네임 댓글내용이 나오게 구현하였습니다.<br> 
처음 댓글 등록시에는 댓글등록이라는 버튼이 나타나며 클릭 시 대댓글 작성이 가능합니다.<br><br>


#### :punch: Category Search<br>
![카테고리 필터](https://user-images.githubusercontent.com/66005208/105624836-0cd7a180-5e68-11eb-8e53-270d84e8025d.jpg)<br>
각 카테고리 별로 카테고리에 맞는 하위카테고리가 나오게 구현하였습니다.<br> 
소셜은 나타나지 않으며 버튼 클릭 시 게시글작성 할 때 지정한 카테고리에 맞는 게시물들이 나타나게 구현하였습니다.<br><br>


#### :punch: STAGE<br>
화면만 제작을 하였으며 인스타그램을 차용하여 닉네임과 팔로우 팔로잉, 자기소개를 나타나게 구현하였습니다.<br>
하단에는 각 카테고리 별로 작성한 게시글들이 나오게 됩니다.<br>
