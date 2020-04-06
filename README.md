# HTML
  - 화면구면
  

1. web Version

  - web 1.0
    - 정적인 검색 서비스 (초기)
    - 동적인 검색 서비스 제공(현재 가장 많이 사용)   동적인 검색 및 사용자의 참여,공유, 개방  

  - web 2.0  
    - 지능형 웹서비스
    - 사용자의 패턴을 분석하여 개인별 맞춤 정보 검색 서비스 제공 1>2로 넘어가는중..

2. HTML(Hyper Text Markup Language)
  - 웹에서 정보를 표현할 목적으로 만든 마크업 언어
  
3. HTML5 의 특징
  1. 구조적 설계 지원(시멘틱 태그)
    시멘틱 이름만 보고도 역할을 짐작할 수 있는것
  2. 그래픽 및 멀티미디어 기능 강화
  3. CSS3/JAVAScript 지원
  4. 다양한 API 제공
  5. 모바일 웹 지원 / 장치 접근 가능(배터리정보,카메라,GPS 등)
  6. 인터넷이 연결되지 않은 상태에서도 어블리케이션 동작

4. HTML의 구성 요소
  - <p align = 'center'> HTML/CSS </p>  
  시작태그 속성     속성값    내부문자  종료태그    
    
  |구성요소|설명
  |:----:|:----:|
  |태그|<와>로 묶인 명령어 시작태크와 종료태그가 한쌍으로 이용|
  |요소|시작태그와 종료태그로 이루어진 모든 명령어 하나의 html문서는 요소들의 집합|
  |속성|요소의 시작태그에만 사용/명렁어 구체화 역할    여러개의 속성을 사용할 수 있으며 공백으로 구분|
  |속성 값|속성이 가지는 값, 입력 시'''' 또는 ''를 이용|
  |내부문자|태그와 속성을 이용하여 표현할 문자|
  
5. HTML 주의사항
  1. 태그는 대소문자를 구분하지 않음(소문자 권장)
  2. 시작태그로 시작하면 반드시 종료태그로 종료
    - 종료태그가 없는 일부 태그를 제외하고는 반드시 종료해야함
  3. 파일 확장자는 반드시 html, htm으로 설정
  4. 문자의 공백은 한 개만 인식
    - 공백을 추가로 하기위해선 특수기호를 사용 (&nbsp;)등
    
6. HTML 기본구조

```
문서유형 <!doctype html>
        <html lang="ko">
                  <head>
         머리      문서의 각종 정보와 문서 자체에 대한 설명 내용
                  <tltle>,<meta>,<link>,<style>,<scipt> 등 사용
                  </head>
                  <body>
                  화면에 출력해서 보여주는 모든 정보/내용
         몸체      head들어가는 태그를 제외하고 모든 태그를 사용
                  </body>
        </html>
```  
- <html><html>
   - html 문서 시작,끝을 표시
   - lang 속성은 이 페이지가 어느 나라 언어로 되어 있는지 표시를 의미  
   - 검색엔진이 페이지 검색 시 참고, 검색사이트에서 특정언어 제외 시 사용   
   ```
   우리나라는 <html lang="ko">
   ```
  

  
HTML 태그 

- <meta ~>
  - 헤더 내부에 사용하는 태그로 메타 데이터로 html문서가 가지고 있는 유용한 정보를     담아 두는 곳, 문서 정보를 검색엔진에 전달  
  - 작성법 <meta name/http-equiv:"속성명" content="속성내용">
  
# meta 

  속성
  - http-equiv : meta 요소에 정의 된 된 명령을 먼저 실행 후 후 페이지를 로딩 문서의     초기정보를 나타냄
  
|속성명|설명|
|:--:|:--:|
|content-language|기본 언어 설정|
|content-type|MIME 설정 및 및 문서의 문자셋 설정(encoding)|
|X-UA-compatiable|호환성 설정|
|refresh|페이지 리로드하거나 다른 페이지로 이동|
|Content-Script-Type|스크립트 형식 지정(javascript/Vbscript)|
|Content-Style-Type|스타일 시트 형식 지정(css)|  
  
- <meta ~>
  속성
  - name : http-equiv랑 랑 같은 의미 
|속성명|설명|
|:--:|:--:|
|application-name|웹어플리케이션 이름|
|author|페이지 저자|
|description|페이지를 설명하는 내용|
|generator|페이지를 생성한 프로그램 표시|
|keywords|검색어로 사용 가능,‘,’로 로 구분하여 여러 단어 가능|
|robots|검색로봇의 검색 제한|  

```
<title></title> : 페이지의 제목읅 나타내는 태그
  
작성법
<title>이름 </title>
```  
  
# SCRIPT
  - 페이지에서 스크립트를 사용하기 위해 사용
  - head와 body 두 곳에서 사용 가능  
  
```
작성법
<script> 스크립트 내용</script>
사용 예
<script>
alert(“ 스크립트 테스트”);
</script>
```

속성
```
|속성명|설명|
|:--:|:--:|
|src|외부 스크립트 파일을 문서에 포함할 때 때 사용|
|async|스크립트 비동기적 실행|외부스크립트
|defer|페이지 파싱 이후 스크립트 실행|외부스크립트|
|type|스크립트 언어 데이터 포맷 지정|
|charset|외부 스크립트 자원의 문자를 인코딩|
```  

# LINK
  - 문서를 외부 문서와 연결하기 위해 사용
  → CSS 파일이나 웹 웹 폰트 사용할 때 때 주로 연결
```  
작성법
<link rel=“ 관련속성” type=“MIME” href=“ 문서위치”>
```

|속성명|설명|
|:--:|:--:|
|href|결한 파일의 경로 지정|
|rel|링크가 형성하는 관계를 지정|
|media|연결문서가 표시될 장치 또는 미디어 유형|
|type MIME|타입 지정|

<style></style>
  - 태그의 스타일을 지정해주는 태그, CSS 속성들을 HTML 내에 직접 쓸 쓸 때 때 사용
  
```
작성법
<style>
css 구문
</style>
```  

<base>  

  - 페이지의 링크가 상대경로로 되었을 때 때 그 그 기준이 될 될 경로를 지정
  - 링크를 어떻게 오픈 할 할 것인지 결정
```
작성법
<base href=“ 경로” [target=“ 키워드”]>
```
|키워드|설명|
|:--:|:--:|
|_self| 그 그 위치에서 열기|
|_parent |링크의 바로 상위 페이지에서 열기|
|_top| 최상위 페이지에서 열기|
|_blank| 새 새 창으로 열기|

  

|태그|쓰임|
|:--:|:--:|
|<h?></h?>|제목을 입력할때 사용하는 태그,폰트 크기가 태그에 따라 정해져있다.    숫자로 구분 1~6|
|<br>|문장의 줄 개행|
|<hr>|페이지 가로로 밑줄을 만들어줌|
|<pre> </pre>|입력한 그대로 출력할 떄 사용   띄어쓰기,들여쓰기,줄바꿈이 입력된 그대로 출력|
|<b> </b>|문자를 굵게 만들어줌|
|<em> </em>|문자를 기울여준다.|
|<blockquote> </blockquote>|다른 블로그나 사이트글을 인용할때 사용   자동들여쓰기가 된다.|
|<q> </q>|blockquote와 흡사, 인용 문구에 ''''표시가 됨|
|<mark> </mark>| 배경 부분이 노란색이 되며 형광펜 표시와 비슷함|
|<u></u> |범위에 해당하는 글자 아래에 수평으로 줄을 표시|
|<small></small>| 원 문자보다 작은 글씨로 표시|
|<sub></sub> |아래 첨자|
|<sup></sup>| 윗 첨자|
|<s></s> |취소선|
|<addr></addr>| 약자표시와 함께 마우스가 문자에 있으면 출력(title속성 사용)|
|<cite></cite>|웹 문서나 포스트에서 참고할 때 사용    기울임과 큰 차이는 없으나 나중에 찾기가 편리함|

# <table></table>

```  
<table> : 테이블 표를 생성함
<tr> : 테이블의 한 행을 삽입해줌
<td> : 테이블의 내용..
<th> : 열의 제목을 표시하는 테그
<caption> 
<border> 태그의 속성으로 표의 테두리 두께를 조절
<rowspan> 과 <colspan> 테그의 속성으로 지정한 행만큼 병합하거나 열을 병합
</table> : 테이블을 닫음
```

```
TABLE 구조를 나누는 태그
|태그|설명|
|:--:|:--:|
|<thead></thead>|테이블 구조를 나누는 태그로 테이블 당 한 개만     존재가능|
|<tbody></tbody>|테이블 구조를 나누는 태그로, 몸체를 의미하며 테이블에    여러 개 존재 가능|
|<tfoot></tfoot>|테이블 구조를 나누는 태그로, <thead> 태그 뒤에 있어야    하며 테이블 당한 개만 존재 가능|
```

# 영역 태그  

|속성|설명|
|:---|:----:|
|width/height|페이지 크기 설정|
|name|인라인 프레임 이름|
|src|페이지 경로|
|seamless|태그의 테두리를 없애는 속성|
   
__블록요소__

  - 한줄 전채를 차지하는 요소로 한 줄에 여러 요소가 올 수 없음
  - 기본적으로 가로폭 전체의 넓이를 가지는 직사각형 형태의 요소
  - 자동으로 줄이 개행되며, 크기조절이 가능
  - 블록요소는 모든 인라인 요소를 포함할 수 있고 다른 블록요소도 포함이 됨
  - 제목테그(h1~h6), 목록태그, 테이블태그 .. 등


__인라인요소__

  - 내부의 컨텐츠가 끝나는 지점까지를 넓이로 가지게 되며, 한줄에 여러 요소가 올수 있음
  - 자동으로 줄이 개행되지 않으며, 한줄에 여러 요소가 오기에 크기조절 불가
  - 반드시 블록요소 안에 포함되어 있음
  - 글자 형식 테그.. 등등  
  
```
<div> </div>  
block 형식의 공간을 분할(수직으로 공간 분할)  
```
```
<span></span>  
  - inline 형식의 공간을 분할(수평으로 공간 분할)
```  

html4와 html5  

html4 페이지 구조
  - <div>,<span> 태그를 이용하여 구역을 설정하고 id 값을 부여하여 구분
  - 개발자 마다 id를 를 부여하는 방식이 달라 구조를 이해하기 어려움
  - 구조 파악이 어려워 유지보수가 어렵고, 검색엔진이 확인할 때에도 구별이 어려움
  
html5의 의 페이지 구조

- __시멘틱 태그__ 를 사용
- 웹 웹 접근성 용이
→ 장애인, 고령자 등이 웹 웹 사이트에서 제공하는 정보에 비 비 장애인과 동등하게 접근하고 이
해할 수 수 있도록 보장하는 것


__시멘틱 태그__

- 페이지 구조를 특정 기능에 맞는 태그를 사용하여 구분
- 페이지 구조를 쉽게 파악하고 좀 더 정확한 정보를 검색 할 수 있게됨

  1. <header> </header>   
    - 특정부분의 머리말로 쓰임    
  2. <nav>
    - 다른 사이트나 페이지로 이동하는 태그를 모아 놓은 태그(네비게이션)
    - 특정 태그에 종속되지 않고 어느 곳에서나 사용할 수 있음
    - 주로 메뉴, footer의 사이트 링크 모음에 많이 쓰임
  3. <section> </section>
    - 웹 웹 문서에서 컨텐츠가 들어가는 영역, 컨텐츠를 주제별로 묶을 때 사용
    - <section>태그 안에 <section>태그를 넣을 수 있음
    - 주제별로 article을 묶어주는 태그  
  4. <article> </article>  
    - 웹 페이지의 내용이 들어가는 영역
    - 이 태그 영역은 다른곳으로 배포하거나 재사용 가능  
    - 검색 로봇은 이 태그가 사용된 컨텐츠는 배포할 수 있는 컨텐츠로 인식
  5. <asid> </asid>  
    - 사이드바라고 불림
    - 본문 외의 기타내용을 담고 있는 영역
    - 주로 광고를 달거나 링크모음 등을 표현
  6. <footer> </footer>
    - 웹페이지 맨 아래쪽에 위치하며, 회사소개, 저작권, 연락처 등의 정보 표시 
    - <footer>에는 <header>,<section>,<article>등 다른 레이아웃 사용 가능


# 멀티미디어 태그
  
<img>  
  - 웹페이지에 사진이나 그림을 삽입할 때 사용하는 태그  
  - 닫는 태그가 존재하지 않음  

|속성|설명|
|:--:|:--:|
|src|삽입할 이미지 경로를 지정하는 속성|
|alt|이미지 설명을 해주는 텍스트 속성    이미지가 출력이 안되면 표시됨||
|height/width|이미지의 크기를 설정하는 속성|



|이미지확장자|설명|
|:-----:|:----:|
|GIF|파일 크기가 작아 작은 아이콘이나 블릿 기호에 많이 사용 투명한 배경이나 움직이는 이미지를 만들수 있음|
|JPG/JPEG|사진을 위해 개발,저장을 반복하다보면 화질이 떨어질수 있다.|
|PNG|네트워크용으로 개발되어 최근 많이 이용|   
  
  - **최근 벡터 이미지인 SVG확장자의 활용빈도도 높아지고 있다.**  
  
 - http://maschek.hu/imagemap/imgmap/ 수업용 사이트
 
<map></map>, <area>
  - 이미지를 구역 별로 나누어 링크를 걸어주는 태그
  - <img>태그에 usemap속성을 지정해야 사용 가능
  
|속성|설명|
|:-----:|:----:|
|alt |대체 텍스트 지정|
|cords |분할할 지역 좌표 지정( 시작, 끝)|
|href |링크 페이지 경로 지정|
|media |링크 페이지 최적화 미디어 지정|
|rel |현재 페이지, 링크페이지 관계 지정|
|shape |링크로 사용할 영역 형태 지정|
|target |링크페이지가 열릴 위치( 새창, 현재창, 부모창, 최상위창)|
|type |링크 페이지의 미디어 유형 지정|

```
<img src=‘ 경로’ usemap=‘#tt’>
<map name=‘tt’>
<area shape=‘ 모양’ cords=‘00,00( 시작),00,00( 끝)’ href=‘ 링크경로’ target=‘ 위치’>
<area shape=‘ 모양’ cords=‘00,00( 시작),00,00( 끝)’ href=‘ 링크경로’ target=‘ 위치’>
</map>
```

<audio> </audio>  
  - 웹 브라우저에서 플러그인의 도움 없이 음악을 재상할 수 있게 만들어주는 태그   <크롬에서 autoplay 지원 x>
 
|속성|설명|
|:--:|:--:|
|src |음악파일의 경로 지정|
|controls |재생도구 출력 지정|
|autoplay |자동 재생여부 지정( 모바일에서 적용X)|
|loop |반복여부 지정|
|preload|none : 재생 전 전 미리 다운로드 하지 않음      metadata : 기본정보만 가져옴( 크기, 첫프레임, 오디오길이 등)      auto : 미리 다운로드 함|


<video></video>
 - 웹 브라우저에서 플러그인의 도움 없이 미디어를 재생할 수 있게 만들어주는 태그  
 
|속성 |설명|
|:--:|:--:|
|src |음악파일의 경로 지정|
|controls |재생도구 출력 지정|
|autoplay |자동 재생여부 지정( 모바일에서 적용X)|
|loop |반복여부 지정|
|preload |재생시 모두 불러올지 지정|
|poster |재생전 출력할 이미지 경로 지정|
|width/height |미디어 크기 지정|
  
  
# 하이퍼링크 태그  

<a></a>
  - 웹 웹 페이지에서 해당 부분을 클릭하면 지정된 페이지로 이동하는 태그
  - 외부 사이트 연결, 문서 내부에서 이동 가능  

|속성|설명|
|:--:|:--:|
|href |링크한 페이지의 id 값이나 사이트 주소 지정|
|target|링크 페이지가 표시될 위치 지정( 새창, 현재창)    _blank : 새창 / _self 현재창   _parent : 상위창 / _top : 최상위창|
|download |링크한 페이지를 표시하지 않고 다운로드 하는 것|
|rel |현재 페이지와의 관계지정|
|hreflang |링크한 페이지의 언어를 지정|
|type |페이지의 파일 유형 지정 |

  - <a></a> 태그 작성 – 기본 작성
  - <a href=‘ 이동할 페이지 경로’> 링크 표시 문구</a>
  - <a></a> 태그 작성 – 이미지 클릭 시 시 이동
  - <a href=‘ 이동할 페이지 경로’><img src=‘ 이미지 경로’></a>
  - <a></a> 태그 작성 – 현재 문서 내부 이동
  - <a href=‘# 이동할태그id’> 링크표시문구</a>
  - <a></a> 태그 작성 – target 사용
  - <a href=‘ 이동할 페이지 경로’ target=‘ 창선택 옵션’> 링크표시문구</a  
  
# 폼 태그  
  
<form></form>   
  - 사용자가 력한 data를 보내는 방식과 처리할 프로그램을 정하는 태그  
  
|속성|설명|
|:--|:---|
|method|get:url창에 데이터를 보내는 방식,크기제한 있음,눈으로 확인가능  post:http 헤더에 데이터를 넣어 보내는 방식,크기제한x 눈에보이지 않음|
|name|<form>태그의 고유이름지정(<form>을 구분하기위함)|
|action|데이터를 처리할 프로그램(페이지)지정|
|target|action속성을 어떻게 열 것인지 지정|
|autocomplete|이전 입력내용 출력하는 기능(생략하면 자동 on)|
  
<fieldset></fieldset>, <legend></legend>  
  - 폼 요소를 그룹으로 묶는 태그, 묶은 폼 요소에 명칭을 붙이는 태그

<input>   
  - 사용자로부터 데이터를 입력받기 위한 태그  
  - form 태그를 통해서 데이터 전송 시 해당 form 태그 내부에 있는 input 태그에 작성된 내용만 전송  
  
|속성|설명|
|:--:|:--|
|ype |입력창의 타입을 결정하는 속성(text,checkbox,radio 등)|
|value input |요소의 기본값 입력( 사용자 입력 값이 value가 가 됨)|
|name|input을 을 구별 할 할 수 수 있는 명칭    ( 데이터를 받는 곳에서 name 속성의 값으로 구분)|
|min/max/step |허용하는 범위 최소값/ 최대값/ 값의 증감값|
|autocomplete |자동완성기능|
|height/width |입력창의 높이와 넓이|
|readonly |읽기전용필드|
|accept |파일타입에 대해 사용자에게 알려주는 기능|
|multiple |여러 개의 값을 입력 가능|
|placeholder |사용자 입력전 입력창 표시글( 사용자 입력 시 사라짐)|
|autofocus |입력창 커서 표시|
|required |필수입력 필드 지정|
|size |화면에서 표현하는 글자 수|
|maxlength |사용자가 입력할 수 있는 글자 수의 제한|
|minlength |최소입력 글자 지정|
|list |<datalist>의 의 옵션값을 <input> 안에 나열|

type속성의 기본 값들
|속성 |설명|
|:--:|:--:|
|text |한  줄 짜리 텍스트 입력창이 생김|
|password |비밀번호 입력창, 입력 시•••로 로 표시됨|
|hidden|사용자에게 보이지는 않지만 값을 넣을 수 있는 창,    데이터를 숨겨서 전송할 때 때 사용|
|button |버튼 생성, 자체기능은 없고, script를 를 통해 함수 연결 가능|
|checkbox |체크박스생성( 다중 항목 선택)|
|radio |라디오버튼생성( 단일 항목 선택)|
|file |파일입력 양식|
|submit |입력한 데이터를 <form> 태그의 action의 의 페이지로 전송|
|reset |입력한 내용을 지우는 기능|
|image |이미지 형태 생성|
  
text속성 값들  

|속성 |설명|
|:--:|:--:|
|name |input의 의 구분자/ 명칭|
|size |사용자 화면에 보여줄 문자 수|
|value |input 요소에 들어가 값( 설정하지 않으면 빈값)|
|maxlength |최대 입력 갯수|
|minlength |최소 입력 갯수|

checkbox
```
<input type=‘checkbox’ name=‘ 명칭’ value=‘ 값’ [checked]>
<input type=‘checkbox’ name=‘ 명칭’ value=‘ 값’ [checked]>
```
→ 같은 checkbox 그룹은 name이 이 같아야 함
→ value 속성은 체크 시 시 전달할 값
→ checked 속성은 선택사항으로 입력 시 시 자동으로 check 되어 있음(default : 지정 안됨)  

file
```
<input type=‘file’ name=‘ 명칭’ 
[multiple] accept=‘ 허용할 확장자들’>
``` 

→ 파일을 입력하기 위한 특수한 형태로 클릭 시 시 전송 할 할 파일 선택 가능  
→ multiple 속성 추가 시 시 한번에 여러 파일 선택 가능( 기본은 1 개만 가능)  
→ accept 속성에 확장자를 넣으면 해당 확장자만 보여주며, 콤마(,)를 를 통해 구분  
→ value 속성을 통한 기본값 설정이 불가능  

submit / reset
```
<input type=‘submit’ value=‘ 전송’> , 
<input type=‘reset’ value=‘ 초기화’>
```
→ submit : <form> 태그 내부에 있는 <input> 태그들의 값을 모두 전송하는 버튼
→ reset : <form> 태그 내부에 있는 <input> 태그들의 값을 모두 비우는 버튼
→ value는 는 버튼에 보여질 값  
  
<label></label>
  - <input> 태그에 레이블( 명칭)을 붙이기 위한 태그
  - 레이블 : 입력창 옆에 붙여 놓은 문구 (예 예 : 비밀번호, 아이디 등)   
  
|속성 |설명|
|:--:|:--:|
|for |label로 묶을 id|
|form |label이속한 form의 id|

type 속성 html5 양식
|속성|설명|
|number |숫자를 입력하는 창 생성|
|range |슬라이드 막대로 숫자 지정|
|search |검색어를 입력하는 창 출력|
|tel |전화번호를 입력하는 창 창 출력|
|email |@를 포함하여 작성하여야 하는 창 생성(@가 가 있는지 확인)|
|url |주소값을 입력하는 창 출력(http:// 확인)|

color
```
<input type=‘color’ name=‘ 명칭’ value=‘ 색상값’ >
→ 선택한 색의 rgb 값이 전송
```

date/datetime/datetime-local/month/week/time
```
<input type=‘ 타입명’ name=‘ 명칭’ min=‘ 최소표시 날짜 지정’ max=‘ 최대표시 날짜 지정’
step=‘ 간격’ value=‘ 날짜’>
```  
→ date : yyyy-mm-dd / datetime:yyyy-mm-dd00:00 / month : yyyy-mm / week :yyyy-W
→ step의 의 경우 클릭을 통해 증/감 감 시키는 경우 증감 간격을 의미  

number / range  
```
<input type=‘ 타입명’ name=‘ 명칭’ min=‘ 최소값’ max=‘ 최대값’ step=‘ 증감값’ value=‘ 초기 표
현값’ >
```
→ number는 는 직접 입력 및 및 클릭을 통한 증감을 통해 숫자 입력
→ range는 는 진행 바를 이용하여 숫자 입력  
  
  
search / url / email / tel
```
<input type=‘ 타입명’ name=‘ 명칭’ value=‘ 초기값’>
```  

→ url은 은 입력 값에 http://가 가 있어야 정상적인 입력으로 판단
→ email은 은 입력 값에 @가 가 있는지 확인   
  
<form> 태그 내부에서 여러 값을 표현 하는 태그  
  
|속성 |설명|
|:--:|:--:|
|select |드롭다운 목록으로 값을 입력|
|option |list 옵션값으로 지정|
|optgroup |list 목록을 그룹으로 묶을 때 사용|
|datalist |input 태그를 리스트 형식으로 할 때 사용|
|textarea |여러 줄을 입력하는 텍스트 영역  |

<select></select>, <option></option>
```
<select name=‘ 명칭’ size=‘ 숫자’ [multiple]>
<option value=‘ 값’> 표시내용</option>
<option value=‘ 값’> 표시내용</option>
<option value=‘ 값’ [selected]> 표시내용</option>
</select>
```  

<select></select>
→ size : 화면에 표시될 항목 개수 지정
→ multiple : 여러 항목 선택 지정, ctrl 누른 상태에서 선택
<option></option>
→ value : 옵션 선택 시 시 넘겨질 값
→ selected : 기본으로 선택된 값

<optgroup></optgroup>
```
<select name=‘ 명칭’ size=‘ 숫자’ [multiple]>
  <optgroup label=‘ 목록이름1’>
  <option value=‘ 값’> 표시내용1</option>
  <option value=‘ 값’> 표시내용2</option>
  </optgroup>
  <optgroup label=‘ 목록이름2’>
  <option value=‘ 값’> 표시내용3</option>
  <option value=‘ 값’> 표시내용4</option>
  </optgroup>
</select>
```

<optgroup></optgroup>
→ label : 목록 제목으로 출력될 내용

<datalist></datalist>
```
<input type=‘text’ name=‘ 명칭’ list=‘datalist id 값’>
<datalist id=‘id’>
  <option value=‘ 값’>
  <option value=‘ 값’>
  <option value=‘ 값’>
</datalist>
```
→ <input> 태그의 값으로 사용될 리스트

<textarea></textarea>
```
<textarea rows=‘ 보여질 행의 수’ cols=‘ 보여질 열의 수’ name=‘ 명칭’>
</textarea>
```

→ 사용자가 마우스를 이용하여 크기를 조절 할 할 수 수 있음
→ 크기조절을 방지하기 위해서는 CSS를 를 사용해야 함

# CSS

style과 stylesheet  
  
  - style은 정해진 속성을 입력하여 웹페이즈를 꾸미는 것  
  - stylesheet는 웹페이지에서 반복적으로 쓰는style을 모아 놓은 것  
```
 P { color : red;  }  
```   
 선택자  속성  값  
 
 
 
stylesheet 종류  

  1. 내부 스타일 시트
    - html문서 내부의 <style></style>에 스타일 정보를 저장하는 방법
    
    
- 선택자

__CSS 단위 구성__

<table>
  <tr>
    <th>구분</th>
    <th>단위</th>
    <th>내용</th>
  </tr>
  <tr>
    <td rowspan="3">상대 크기<td>
    <td>
</table>
      
      
      
  <table>
    <tr>
      <th>표현방법</th>
      <th>내용</th>
    <tr>
    <tr>
      <td>영문색 이름</td>
      <td>영문으로 색 이름 작성<br>red,white,blue...</td>
      <td>16진수 표현</td>
      <td>rgb값을 기준으로 16진수로 작성<br></td>
 </table>   
    
    
 - font-family  
    - 폰트의 글꼴을 설정해주는 속성
    - 글꼴 이름1이 없으면 글꼴2,글꼴3으로 선택되어 설정
    - 글꼴이 모두 없으면 브라우저 기본 글꼴로 적용

    ```
    기본형식
    선택자 {
      font-maily:글꼴1[, 글꼴2,글꼴3];
    }
    ```   

 - font-size  
    - 글자의 크기를 조절하는 속성
    - 단위 : em,px,pt,ex   

    & ex:현재 소문자 x의 배수의 크기를 설정

    |속성 값|내용|
    |:--:|:--:|
    |normal|기본형태|
    |bold|굵게 표시|
    |bolder|더 굵게 표시|
    |lighter|더 가늘게 표시|
    |100~900|굵기의 정도를 숫자로 표시|

 - font-variant  
    - 영어를 작은 대문자로 표시해 주는 속성
    ```
    선택자 {
      font-style:normal 또는 italic 또는 oblique;
    }
- font-style  
  - 글자를 이텔릭체로 표시하는 속성
  ```
  선택자 {
    font-style  
    
텍스트 스타일
  
  color 
    - 글자색을 하는 속성
    
  text-decoration
  
    - 글자에 밑줄을 긋거나, 취소선을 긋거나, 윗선을 긋거나 밑줄을 표시하지 않는 속성
    
  ```
  선택자 {
    text-decoration: 속성값;
  }
  ```
  
  text-shadow   
    - 텍스트에 그림자 효과를 주는 속성
    
  ```
  선택자 {
    text-shadow: none 또는 (가로 또는 새로번짐 색상);
  }
  ```   
  
  white-space  
    - 공백을 리해 주는 속성   
  
  text-align  
    - 
    
  text-overflow
    - 영역을 벗어나는 텍스트 표시 속성
  
  
  [HTML](#HTML)   
  [META](#meta)   
  [SCRIPT](#SCRIPT)   
  [LINK](#LINK)   
  [영역 태그](#영역-태그)   
  [멀티미디어 태그](#멀티미디어-태그)
