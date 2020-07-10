# **현대사 디지털아카이브(Moredern_History_Digital_Archive)**

대한민국역사박물관의 현대사 디지털아카이브의 데이터를 토대로 만든 jQuery 기반의 웹앱.

현대사 디지털아카이브의 OPEN API(xml 방식)를 통해 데이터를 받아와 박물관 홍보용 웹앱을 제작하였다.

jQuery강의를 한 학기를 수강하면서 jQuery Mobile에 대해 흥미가 생겨서 jQuery Mobile을 기반으로 한 웹앱을 주제로 삼게 되었다.

출처(대한민국역사박물관 현대사 디지털아카이브) : http://archive.much.go.kr/index.do
  


## 파일 실행 전 반드시 실행할 것

(실행 시 Chrome 브라우저로 실행할 것)

1. Chrome 브라우저 바로가기 아이콘 우클릭 후 "속성" 클릭
2. "바로 가기" 탭에서 기존의 "대상" 항목의 오른쪽에 "--disable-web-security --user-data-dir=c:\my\data" 추가 후 "확인"
3. 이 과정은 Chrome에서 동일한 출처 정책을 사용 중지하는 것으로 실행하지 않을 경우 OPEN API를 사용할 수 없음

  

## 참고사항

* 파일 실행 시 외부링크를 통해 이동하여 <script>가 실행되는 경우 때때로 실행이 되지 않을 때가 있음

  (기존에는 'F5'키를 반드시 입력해야 제대로된 화면이 출력되었으나 <body> 태그 안에 <script>를 입력함으로써 불편함을 줄이도록 수정하였음)

* 하지만 같은 상황에서도 때때로 실행이 될 때가 있고 되지 않을 때가 있음

  (작성자의 개발환경 문제일 수도 있고, 작성자의 코딩 문제일 수도 있음)

* **만약 제대로 실행이 되지 않을 경우 'F5' 키를 입력하여 새로고침 시 올바른 화면이 출력됨**

 

### 기능 설명

1. 가장 먼저 main.html을 실행하면 메인 화면을 통해 사용자가 메뉴를 선택할 수 있도록 함

2. 단 화면 우측상단에 있는 로그인 버튼을 통해 로그인에 성공했을 경우 메뉴를 선택할 수 있음

   (현재 DB에 연동되어 있지 않아 회원의 아이디와 비밀번호 조회가 불가능하므로 ID 텍스트박스와 PW 텍스트박스가 입력되어 있으면 로그인 성공 처리하였음)

3. 로그인 성공 시 각 메뉴(링크)를 선택하면 해당 기능 출력(외부링크를 통해 다른 html 파일로 이동)

4. '소개' 메뉴는 해당 웹앱에 어떤 정보들이 있는지 소개되어 있음.

5. 각 메뉴들은(소개, 홍보영상 제외) 현대사 디지털아카이브의 OPEN API를 xml 방식으로 받아와 각자 모두 다른 데이터를 가지고 있으며 해당 리스트 선택 시 액션시트를 통해 자세한 정보를 볼 수 있고 링크를 클릭하면 정보의 출처(현대사 디지털아카이브)로 이동함

6. 마지막 '홍보영상' 메뉴는 "Youtube_Iframe_API"를 통해 유튜브 플레이어로 대한민국역사박물관 홍보영상을 시청할 수 있도록 함

7. 화면 좌측상단의 '메뉴' 버튼을 클릭하면 메뉴들이 나타나고 그 메뉴들을 선택 시 마찬가지로  해당 html 파일로 이동

8. 화면 우측상단의 '로그아웃' 버튼을 클릭하면 메인 화면으로 이동하고 다시 로그인하도록 함
