# 1교시 시작 전 준비할 것
* Ctrl + J 터미널 실행 -> git bash 환경 확인
* 경로 우측 끝이 깃으로 연결된 저장소가 맞는지 확인(브랜치명 유무로 체크)
* 경로가 맞지 않으면 반드시 `cd 경로명` 작성해서 브랜치위치로 접속하기
* 전 날 집에서 작업한 파일이 있다면 `git pull origin main` 이용 내려받기
# 파일명 규칙
* `파일명.html`
* 파일명은 공백, 한글, 특수문자 금지
# 자주쓰는 단축어
* `html:5` 쓰고 Tap 키 누르기
* `Ctrl+/` 한줄 주석
* `Shift+Alt+A` 선택영역 주석
# HTML 생성 후 구조태그 작성 순서
1. `html:5` 쓰고 Tab 자동완성
2. `lang="en"`을 `"ko"`로 변경하기
3. `title`제목 작성하기
4. `meta`작성하고 자동목록 중 `kw`선택하고 키워드 작성하기
5. `meta`작성하고 자동목록 중 `desc`선택하고 요약 작성하기
6. `body`내부에 앱의 주요 내용 작성할 준비하기
7. * 파비콘 무조건! <head>안에 link:favicon
# 태그
## 다양한 문서 태그
* 'h1~h6' : 블록, 제목(대중소)
* 'p' : 블록, 내용(1줄, 여러줄)
* 'hr' : 블록, 구분선(디자인선 아님 주의)
* 'br' : 인라인, 강제줄바꿈
* 'em' : 인라인, 특정 문맥 강조
* 'strong' : 인라인, 경고&할인 강조
* 'code' : 인라인, 프로그래밍 코드 구분용
* 'sup','sub' : 인라인,  위첨자 sup&아래첨자sub
* `q', 'blockquote' : 인라인(q) 짧은 인용, 블록(blockquote) 긴 인용
* 's', 'del' : 인라인, s-유효하지 않은 내용, del-교체되거나 삭제된 내용
#특수문자태그
* '&' : 특수문자태그의 시작기호
* ';' : 특수문자태그의 종료기호
* 'lt', 'gt' : 왼쪽꺽쇠(<>), 오른쪽꺽쇠(>)
* '&copy;' : ⓒ copyright 저작권기호
# 속성
* '태그 속성="값"></태그>
* 'class' : 반복되는 의미명, 2개 이상 적용 가능
* 'id' : 단 한번만 작성하는 반복되지 않는 고유명칭
* class, id는 모든 태그에 구분없이 사용 가능!
#git 
*git clone 깃주소붙여넣기
* 링크태그
* 동영상 태그 : autoplay, muted, controls, loop 동영상 속성
    //비디오를 작성하는 방법1
    <video src="동영상경로" autoplay muted controls loop></video>
    //비디오를 작성하는 방법2
    <video autoplay muted controls loop>
        <source src="동영상경로" type="동영상타입1">
        <source src="동영상경로" type="동영상타입2">
    </video>
* 파비콘 무조건! <head>안에 link:favicon
* alt+z :자동줄바꿈
* src="절대경로?playlist=뒤의동영상이름복붙&속성=값&속성=값&속성=값"
    예시 <iframe width="587" height="1043" src="https://www.youtube.com/embed/vYuER_3og_M?playlist=vYuER_3og_M&autoplay=1&loop=1&mute=1" title="개발자 빡치게 하는 법" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
* alt +위 아래 방향키: 이동
* <!-- shift + alt + a -->
* shift + | > 구분선
* window + . >이모지
* ctrl + h >같은 글자 찾기
* 이동하고 싶은경우 <a href="#"> #<-여기에 경로 넣기
* &copy; : ⓒ
# 다양한 문서 태그-2
## blog tag
* `div` : 2개 이상 자식을 묶는 그룹, class 또는 id 필수
* `ul-li` :ul(비순차 그룹), li(목록) 엄격한 부모-자식 관계
* `ol-li` :ol(순차 그룹), li(목록) 엄격한 부모-자식 관계
* `dl-dt-dd` : dl(정의형그룹), dt(정의형제목), dd(정의내용)
    * 검색키워드로 사용하지 않는 소제목과 내용 `h-p`를 dt-dd로 대체 가능
* `a`:  블록의 부모로 사용 시 링크 <div등 그룹 대체 가능>
## inline tag
* `span` : 인라인 그룹, 디자인이 다른 요소를 묶기
* `a`: 인라인의 형제로 사용 시 링크
### 비슷한 의미의 대체 태그들
* `h1~h6`vs `dt`
    * 중요도가 높고 검색키워드로서 사용되어야 한다면 h태그
    * 제목-내용이 바로 연결되고 중요도가 낮으며 키워드로서 사용가치가 낮을 때 dt태그
* `p`vs `li` vs `dd` vs `span`
    * 제목 하단에 단순 단락으로 구성된 내용 표시 p 태그
    * 2개 이상 연속된 목록 구성 시 li태그
    * 중요도와 키워드가 낮은 제목 dt 옆 내용을 감쌀땐 dd
    * 인라인으로 추가로 감싸야하는 내용이 있을 때 span
    `div`vs `ul` vs `ol` vs `dl` vs `span`
    * div-2개 이상의 블록 or 인라인이 자식으로 있을 때 그룹 
    * ul-순서가 없는 목록이 2개 이상있을 때 그룹
    * ol-순서가 있는 목록이 2개 이상있을 때 그룹
    * a -링크로 선택되는 태그가 2개 이상 있을 때 그룹
    * dl - 중요도가 낮은 제목-내용(dt-dd)가 있을 때 그룹
    * span - 2개 이상의 인라인을 묶어야 할 때 그룹