# HTML(Hyper Text Markup Language)
    Hyper Text : 하이퍼링크를 통해 어떤 문서에서 다른 문서로 접근할 수 있는 텍스트
    Markup : (콘텐츠를) 표시하다
    Language : 언어

    - 웹브라우저를 통해 표시되는 웹페이지의 콘텐츠를 정의하기 위해 사용하는 언어이다.
    - HTML 코드는 HTML 파일에 작성한다. 확장자는 *.html 또는 *.htm 이다.
    - 텍스트 에디터에서 작성한 HTML 코드는 웹브라우저를 통해 표시할 수 있다.

# 개발자 도구
    웹사이트 개발용 도구로, 대부분의 최신 브라우저에는 개발자 도구가 탑재되어 있다. HTML CSS 코드 확인, 모바일 모니터링, 네트워크 상태 점검, 스크립트 명령어 확인 등 다양한 기능을 통해 개발자에게 편의를 제공한다.

# 코드 에디터
    프로그래머가 프로그램 소스 코드를 편집하기 위해 사용하는 소프트웨어이다.

# HTML 코드 기본 문법
    태그 : HTML 코드에서 정보(콘텐츠)를 정의하는 형식이다.
        <>와</>를 사용해 콘텐츠의 시작과 끝을 표시한다.
        그러나 경우에 따라 시작과 끝을 구분할 필요가 없는 태그도 존재한다.-> 단일 태그

        속성 : 태그의 부가적인 기능을 정의하는 것으로 선택사항이다.
        ex) <태그명 속성명="속성값">내용</태그명>

        주석 : 사람에게 보이지만, 컴퓨터(웹브라우저)에게는 보이지 않은 코드이다.
        ex) <!--주석으로 처리한다.-->
    
# HTML 문서 기본 구조
    <!DOCTYPE html> : 문서의 첫 부분에서 문서 유형(웹브라우저에게 처리요청)을 지정하는 단일 태그이다.

    <html>~</html> : 문서 유형을 지정한 후 실제 문서가 시작되고 끝나는 것을 나타내는 태그이다. 이 태그의 내부에 다양한 태그들이 포함되어 문서의 내용을 구성한다.

    <head>~</head> : 웹 브라우저 화면에는 보이지 않지만 웹 브라우저가 알아야 할 정보들을 모두 작성한다.
        <meta 태그>
            항상 head 태그의 안에 들어가며 일반적으로 문자 세트, 페이지 설명,문서의 작성자 및 뷰포트 설정을 지정하는 데 사용된다.

            웹페이지에 대한 정보를 제공하므로 검색엔진이 페이지를 검색할 때 참고할 수 있고, 검색 결과에도 반영할 수 있다.
                
                charset : 문자 세트
                http-equiv : 콘텐츠 속성 정보에 대한 http 헤더를 제공
                name : 문서 정보
                content : 메타데이터 내용


        <title>~</title> : 문서의 제목을 나타낸다. 콘텐츠는 브라우저 탭에 표시된다.
    
    <body>~</body> : 실제 브라우저 화면에 표시될 내용을 입력하는 태그이다.
        -텍스트, 이미지, 각종 사용자 인터페이스(버튼, 입력란 등)을 나타낸다.
    
    <p></p> : 문단 요소를 나타내는 태그로써, 가장 많이 사용되는 텍스트 태그이다. 문단과 문단 사이에는 공백이 있다.

    <h></h> : 제목(표제) 요소를 나타내는 태그이다. 숫자와 함께 사용되며, 숫자 1일 때 가장 크고 6일 때 가장 작다.

    <hr> : 수평선을 표시하는 태그이다. 수평선은 주제 변경 또는 내용 구분을 위해 주로 사용된다.

    <br> : 줄바꿈 태그이다. 공백을 두 번 이상 표시하고자 할 때는 &nbsp;를 사용한다.

# HTML 문서 요소
    블록 레벨 요소 : 자기가 속한 영역의 너비를 모두 차지하여 블록을 형성한다.
        {width: 100%; height: auto;} 와 같은 css 속성을 default로 가짐. div,h1,p등이 있다.

    인라인 요소 : 필요한 만큼의 공간만 차지한다.
        {width: auto; height: auto;}와 같은 css 속성을 default로 가짐. span, img 등이 있다.

# 이미지 태그
 img 태그는 이미지를 표시할 때 사용하는 단일 태그이다. 콘텐츠를 적어주는 대신 표시할 이미지에 대한 정보를 속성으로 지정해주어야 한다.
 기본 형태) <img src="표시할이미지파일" alt="이미지설명"/>

    src 속성은 표시할 이미지의 위치정보와 파일명을 입력받는 속성이다. 즉, 이미지의 url을 입력받는다.
    
    alt 속성은 대체 텍스트 여할을 한다. 이미지가 로딩되기 전이나 실패한 경우 이미지 대신에 대체 텍스트가 표시된다.

# 컨테이너 태그
    콘텐츠나 레이아웃에 아무런 영향도 주지 않고 단지 다른 요소 여럿을 묶어 관리하기 편하게 만드는 역할을 하는 태그이다.
    콘텐츠 내용을 구분하거나, 공통적인 스타일을 적용하고자 할 때 쓰인다.
    <div></div> : 블록 레벨 컨테이너
    <span><span> : 인라인 컨테이너

# 전역 속성
    id : 요소에 고유한 이름을 부여하는 식별자 역할 속성.
    class : 요소를 그룹 별로 묶을 수 있는 식별자 역할 속성.
    style : 요소에 적용할 CSS 스타일을 선언하는 속성.
    title : 요소의 추가 정보를 제공하는 텍스트 속성.

# 링크
    a 태그 요소는 href 속성을 통해 다른 페이지 url로 연결할 수 있는 링크를 만든다. 인라인 요소이며, 콘텐츠를 주로 링크의 목적지를 나타낸다.

    탭 설정 : target
        현재 탭에서 오픈: _self
        새 탭에서 오픈 : _blank

# 목록
    순서 없는 목록 : <ul></ul>
    순서 있는 목록 : <ol></ol>

    <li> 태그는 목록에 들어가는 항목을 표시할 때 사용하는 태그이다. 항목들을 감싸는 태그가 무엇이냐에 따라 기호가 달라진다.

# 입력
    - input : 사용자로 부터 값을 입력받을 수 있는 대화형 컨트롤을 나타낸다.
    type 속성 값이 달라짐에 따라 적용할 수 있는 추가 속성의 종류도 조금씩 차이가 있다.

    - select : 다수의 옵션(선택지)를 포험할 수 있는 선택 메뉴이다. option 태그를 사용해 표시한다. value 속성을 지정할 수 있다.

    - textarea : 여러 줄의 일반 텍스트를 입력 할 수 있는 입력요소이다.

# Form
    사용자가 입력한 데이터(입력값)을 서버(정보를 제공하는 호스트)로 보내기 위해 사용하는 태그이다.
    
    form의 내용(입력값)을 제출하기 위해 input 태그의 submit타입을 이용한다.

    Form의 속성
        action : 입력값을 전송할 서버의 url
        method : 입력한 데이터를 어떤 식으로 전송할지(GET or POST)
            GET은 서버에 요청을 보내어 응답을 받아낸다. 서버로부터 정보를 가져오겠다는 요청이다.
            POST는 서버에 요청을 보내어 작업을 수행한다. 서버에 있는 데이터를 추가/수정/삭제한 후에 응답을 받아낸다. 서버의 정보를 조작하겠다는 요청이다.

# 뷰포트(Viewport)
    배율 조정 현상에 대응하기 위해 메트 태그를 사용해 뷰포트 관련 설정을 추가 할 수 있다.

# CSS(Cascading Stlye Sheets)
    HTML, XHML, XML 같은 문서의 스타일을 꾸밀 때 작성하는 코드이다. 
    CSS 문서는 독립적으로 존재할 수 있지만, HTML 문서가 없는 CSS는 의미가 없다.

# CSS 기본 문법

    선택자{
        속성명: 속성값;
    }

    선택자 : 어떤 요소에 스타일을 적용 할지에 대한 정보이다.
    {} : 선택한 요소에 적용할 스타일을 정의하는 영역이다.
    속성명 : 어떤 스타일을 정의하고 싶은지에 대한 정보(색상,크기 등)이다.
    속성값 : 어떻게 정의하고 싶은지에 대한 정보이다.

# HTML에 CSS 적용
    인라인 스타일 : 태그에 직접 style 속성을 추가하여 요소에 직접적으로 정의하는 방식이다. 웹 콘텐츠와 스타일시트를 분리하기 위해서는 사용하지 않는 편이 좋다.

    스타일 태그 : HTML 문서에 <style></style> 태그를 추가하여 그안에 CSS 코드를 작성하는 방식이다.

    문서 간의 연결 : 확장자가 *.css인 스타일시트 파일을 생성해 그 안에 CSS코드를 작성하고, HTML문서에 이를 연결해줄 수 있다. 이 때는 <link> 태그를 사용한다.
        ex) <link href="css 경로 주소" rel="외부소스종류">

            href : 연결하고자 하는 외부 소스의 url을 기술하는 속성
            rel : 현재 문서(HTML)와 외부 소스의 연관 관계를 기술하는 속성
    
    -> <link> 태그는 head 내부에서 사용해야 한다.

# CSS 선택자의 종류
    1.전체 선택자 : *(모든 요소)
    2.태그 선택자 : 주어진 이름을 가진 요소가 다수일 경우, 해당 요소들을 모두 선택한다.
    3.클래스 선택자 : 주어진 class 속성값을 가진 요소를 선택한다.
        ex) .class{}
    4.아이디 선택자 : 주어진 id 속성값을 가진 요소를 선택한다. 고유한 식별자 역할을 하는 전역 속성이다.
        ex) #id{}
    5.그룹 선택자 : 다양한 유형의 요소를 한꺼번에 선택하고자 할 때 사용한다. 쉼표(,)를 이용해 선택자를 그룹화한다.

    *선택자가 겹치는 경우, 기본적으로 나중에 작성된 스타일이 적용된다.
     선택자가 다르지만 요소가 겹치는 경우, 선택자 우선순위에 의해 적용될 스타일이 결정된다. 
        - 선택자 우선순위 : 아이디 선택자 > 클래스 선택자 > 태그 선택자

# 텍스트 관련 CSS 속성
    font-family : 글꼴을 정의한다.
        여러 개의 글꼴을 연달아 기입하여 우선 순위를 지정할 수 있다.(폰트가 지원되지 않을 경우 후순위를 둔다.)
    font-size : 글자 크기를 정의한다.
        px: 모니터 상의 화소 하나 크기에 대응하는 절대적인 크기
        rem: <html>태그의 font-size에 대응하는 상대적인 크기(배수만큼 조절)
        em: 부모태그(상위태그)의 font-size에 대응하는 상대적인 크기
    text-align : 정렬 방식을 정의한다.
        left/right, center, justify(양쪽정렬)
    color : 글자 색상을 정의한다.
        키워드 : 색상별 키워드를 사용한다.(red,blue)
        RGB 색상 코드 : # + 여섯자리 16진수 값 형태로 지정한다.(#000000:검정)
        RGB 함수 : RED,GREEN,BLUE 수준을 각각 정의해 지정한다.(RGB(0%,0%,0%))

# display & border CSS 속성
    display : 요소를 블록과 인라인 요소 중 어느 쪽으로 처리할지 정의한다.
    border : 요소가 차지하고 있는 영역에 테두리를 그릴 수 있다.

# 박스모델(Box-Model)
    브라우저가 요소를 렌더링 할 때, 각각의 요소는 기본적으로 사각형 형태의 영역을 차지하게 된다. 이 영역을 '박스'라 표현하며, CSS는 박스의 크기, 위치, 속성을 결정할 수 있다.
        콘텐츠 영역 : width, height
        안쪽 여백 : padding
        바깥쪽 여백 : margin
        테두리 : border-width



    
    








