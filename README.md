[책갈피](#책갈피)


# html

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
  
# script

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

# link
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

__<table></table>__

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


# 시멘틱 태그

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

# css

__style과 stylesheet__
  
  - style은 정해진 속성을 입력하여 웹페이즈를 꾸미는 것  
  - stylesheet는 웹페이지에서 반복적으로 쓰는style을 모아 놓은 것  
  
```
P { color : red;  } 
선택자  속성  값  
```   
 
__stylesheet 종류  __

  1. 내부 스타일 시트
  
    - html문서 내부의 <style></style>에 스타일 정보를 저장하는 방법
    
  ```
  <style>
    p { color :red; }
  </style>
  ```  
  
  2. 외부 스타일 시트  
  
    - 외부에 css 파일을 작성하고 <link>태그를 이용하여 읽어와서 스타일 적용  
     
   ```
   <link href="css파일 경로" rel="stylesheet" type="text/css">
   ```  
   
 3. 인라인 스타일 시트  
 
   - 태그 내부에 스타일 정보를 지정하는 방법 
   
 ```
 <p style="color:red">test</p>
 ```
 
 
# css 선택자

__선택자__

  - html문서 내부에서 스타일을 적용하기 위한 요소를 선택하는 것
  - html문서를 꾸미기 위해서는 각 요소별로 스타일을 적용하기 위해 선택자를    이용하여 요소를 선택
  
```
h1{
  color: red;
}

ul>li:first-child{
  color: red;
}
``` 

__선택자의 종류__

|구분 |내용|
|:--:|:--:|
|전체 선택자 | * |
|태그 선택자 |태그이름(h1, p, li 등등)|
|아이디 선택자| # 아이디명|
|클래스 선택자| . 클래스명|
|후손 선택자| 선택자 선택자|
|자손 선택자| 선택자 > 선택자|

<table>
  <tr>
    <td rowspan="3">속성선택자</td>
    <td> 선택자[ 속성= 값] / 선택자[ 속성~= 값] </td>
  </tr>
  <tr>
    <td>선택자[ 속성|= 값] / 선택자[ 속성^= 값</td>
  </tr>
  <tr>
    <td>선택자[ 속성$= 값] / 선택자[ 속성*= 값]</tr>
  </tr>
  <tr>
    <td>동위선택자 </td>
    <td>선택자 + 선택자 / 선택자 ~ 선택자</td>
  </tr>
  <tr>
    <td rowspan="4>구조 선택자</td>
    <td> 선택자:first-child / 선택자:last-child</td>
  </tr>
  <tr>
    <td>선택자:nth-child( 수열) / 선택자:nth-last-child( 수열) </td>
  </tr>
  <tr>
    <td> 선택자:first-of-type / 선택자:last-of-type</td>
  </tr>
  <tr>
    <td>선택자:nth-of-type( 수열) / 선택자:nth-last-of-type( 수열)</td>
  </tr>
  <tr>
    <td> 반응 선택자 </td>
    <td> 선택자:active / 선택자:hover </td>
  </tr>
  <tr>
    <td> 상태 선택자 </td>
    <td> :checked / :focus</td>
  </tr>
  <tr>
    <td>속성선택자 </td>
    <td>:enabled / :disbled </td>
  </tr>
  <tr>
    <td> 링크 선택자 </td>
    <td> :link / :visited </td>
  </tr>
  <tr>
    <td rowspan="2">문자 선택자</td>
        <td> ::first-letter / ::first-line </td>
  </tr>
  <tr>
    <td>:after / ::before / ::selection</td>
  </tr>
  <tr>
    <td> 부정 선택자 </td>
    <td> 선택자:not(선택자) </td>
  </tr>
  <tr>
    <td> 전체 선택자 </td>
    <td> *{ 설정내용;}</td> 
</table>

태그 선택자

  - 특정 태그에 적용되는 스타일  
  
기본 형식
태그명 { 설정내용; }

  - 여러 개의 태그에 동시에 적용하려고 하는 경우 ‘,’( 콤마)로 로 구별
  
예 예 : p,a,h1{ 설정내용;}


# 텍스트 스타일


__CSS 단위 구성__

<table>
  <tr>
    <th>구분</th>
    <th>단위</th>
    <th>내용</th>
  </tr>
  <tr>
    <td rowspan="3">상대 크기<td>
    <td>em</td>
    <td>부모 요소의 크기가 기준 배수를 의미   1배 = 1em = 100% (부모요소 크기 기준)
  </tr>
  <tr>
    <td>rem</td>
    <td>최상위 부모 요소의 크기가 기준으로 배수</td>
  </tr>
  <tr>
    <td>%</td>
    <td>기본 설정된 크기에서 상대적으로 크기 설정 초기 설정 100%     </td>
  </tr>
  <tr>
    <td rowspan="2">절대크기</td>
    <td>px</td>
    <td rowspan="2">기본 지정된 크기</td>
  </tr>
  <tr>
    <td>pt</td>
  </tr>
</table>
      
__CSS 색상 표현__

|표현방법|내용|
|:--:|:--:|
|영문색 이름|영문으로 색 이름 작성    red,white,blue ...|
|16진수 표현 | rgb 값을 기준으로 16진수로 작성   ...|
|rgb|rgb값을 0~255의 숫자로 표현   rgb(255,0,0),rgb(0,0,0)...|
|rgba|rgb방식과 동일하며 맨 마지막에 투명도를 0~1로  표현 rgba(255,0,0,0.5)    0~1로 갈수록 투명-> 불투명|

__font-family__
 
  - 폰트의 글꼴을 설정해주는 속성
  - 글꼴 이름1이 없으면 글꼴2,글꼴3으로 선택되어 설정
  - 글꼴이 모두 없으면 브라우저 기본 글꼴로 적용

```
기본형식
선택자 {
font-maily:글꼴1[, 글꼴2,글꼴3];
}
```   

__font-size__

  - 글자의 크기를 조절하는 속성
  - 단위 : em,px,pt,ex   
  & ex:현재 소문자 x의 배수의 크기를 설정   

```
기본 형식
선택자 {
font-size : 숫자단위;
}
```

__font-weight__

  - 글자의 굵기를 조절하는 속성
  
```  
기본 형식
선택자 {
font-weight : 속성 값;
}
```

|속성 값|내용|
|:--:|:--:|
|normal|기본형태|
|bold|굵게 표시|
|bolder|더 굵게 표시|
|lighter|더 가늘게 표시|
|100~900|굵기의 정도를 숫자로 표시|


__font-variant __
 
  - 영어를 작은 대문자로 표시해 주는 속성
    
```
선택자 {
  font-style:normal 또는 italic 또는 oblique;
}
```

__font-style__

  - 글자를 이텔릭체로 표시하는 속성
  
  
```
선택자 {
  font-style : normal 또는 italic 또는 oblique;
}
``` 

  - italic : 처음부터 기울어진 글자가 존재
  - oblique : 기본 글자를 기울여서 표시  → italic 을 주로 사용
 
__font__

  - 글꼴 속성을 모아서 표현할 수 수 있는 스타일 속성  

```
기본 형식
선택자 {
font : font-style font-variant font-weight font-
size/line-height font-family;
}
```


  
__color __
    
    - 글자색을 하는 속성
    
```
선택자 {
  color : 색상;
```


__text-decoration__
  
    - 글자에 밑줄을 긋거나, 취소선을 긋거나, 윗선을 긋거나 밑줄을 표시하지 않는 속성
    
```
선택자 {
  text-decoration: 속성값;
}
```

|속성 값 |내용|
|:--:|:--:|
|none 줄 줄 삭제|
|underline 밑줄 표시|
|overline 윗줄 표시|
|line-through 취소선 표시|


__text-shadow__   
   
   - 텍스트에 그림자 효과를 주는 속성
    
```
선택자 {
  text-shadow: none 또는 (가로 또는 새로번짐 색상);
}
```   
  
__white-space__  
  
    - 공백을 리해 주는 속성   

|속성 값 |공백 여러개 |개행 처리 |영역 이탈|
|:--:|:--:|:--:|:--:|
|normal |하나로처리 |개행 하지 않음 |자동 줄 줄 바꿈|
|nowrap |하나로처리 |개행 하지 않음 |한줄로 표시|
|pre |여러 개로 처리 |개행 처리 함 |한줄로 표시|
|pre-line| 하나로처리 |개행 처리 함 |자동 줄 줄 바꿈|
|pre-wrap |여러 개로 |처리 개행 처리 함 |자동 줄 줄 바꿈|

__letter-spacing / line-spacing__

  - letter-spacing : 낱개 글자의 간격을 조정하는 속성
  - word-spacing : 단어와 단어 사이 간격을 조정하는 속성

```
기본 형식
선택자 {
letter-spacing : 숫자( 단위);
word-spacing : 숫자( 단위);
}
```

# 문단스타일

__direction__

  - 글자 쓰기 방향 지정 속성
  
```
선택자 {
  direction : Itr 또는 irl
}
```

|속성 값|내용|
|:--:|:--:|
|itr|왼쪽에서 오른쪽으로 텍스트 표시|
|rtl|오른쪽에서 왼쪽으로 텍스트 표시|


__text-align__  

  - 문자 위치를 조정(정렬)하는 속성  
  
|속성 값|내용|
|:--:|:--:|
|left|왼쪽에 맞추어 정렬|
|right|오른쪽에 맞추어 정렬|
|center|가운데 맞추어 정렬|
|justify|양쪽에 맞추어 정렬|

__text-indent__

  - 문장을 들여쓰기 하는 속성   
  
```
선택자 {
  text-indent:숫자(단위);
}
```

__line-height__

  - 문장끼리의 줄 간격을 조정하는 속성
  
```
선택자 {
  line-height:숫자(단위);
}
```

__text-overflow__

  - 영역을 벗어나는 텍스트 표시 속성
  
```  
선택자 {
text-overflow : clip 또는 ellipsis;
}
```

|속성 값|내용|
|:--:|:--:|
|clip|영역을 넘어가는 텍스트를 자름|
|ellipsis|말 줄임으로 잘린 텍스트 표현|


__list-style-type__

  - 목록의 기호의 스타일을 지정하는 속성
  
__list-style-image__

  - 기호 대신 이미지 삽입
  
```  
기본 형식
선택자 {
list-style-image : url( 이미지경로);
}
```

__list-style-position__

  - 목록 기호 들여쓰기
  
선택자 {
  list-style-position : inside 또는 outside;
}

|속성 값|내용|
|:--:|:--:|
|inside|블릿이나 숫자를 안쪽으로 들여 씀|
|outside|블릿이나 숫자를 밖으로 내어씀(default)|

__list-style__

  - 목록 스타일을 한 번에 지정하는 속성
  
```
선택자 {
  list-style : type 값 position값 image값;
}
```

# 배경 스타일 

__background-color__

  - 배경색을 지정하는 속성
  
```
선택자 {
  background-color:색상표현;
}
```

__background-clip__

  - 배경 범위 조절
  
|속성 값|내용|
|:--:|:--:|
|border-box|박스 모델의 가장 외곽이 테두리까지 적용|
|padding-box|테두리를 제외한 패딩범위까지 적용|
|content-box|내용 부분만 적용|

__background-img__

  - 요소에 배경을 이미지로 지정
  
```
선택자 {
  background-ing:url(경로);
```

__background-repeat__

  - 배경 이미지 반복 출력
  
|속성 값|내용|
|:--:|:--:|
|repeat|브라우저에 가득 찰 때까지 가로/세로 반복|
|repeat-x|넓이만큼 반복(가로)|
|repeat-y|높이만큼 반복(세로)|
|no-repeat|이미지 한 번만 출력|

__background-size__

  - 배경 이미지의 크기를 조절하는 속성
  
|속성 값| 내용|
|:--:|:--:|
|auto|원래 배경이지미 크기만큼 표시|
|contain|요소 안으로 이미지가 들어올 수 있게 확대 축소|
|cover|요소의 범위를 이미지가 덮을수 있도록 확대/축소|
|크기값(px)/백분율|수치화된 값으로 표현|


__background-position__

  - 배경 이미지의 위치를 조정하는 속성
  
|구분|속성값|
|:--:|:--:|
|수평위치|left/center/right|
|수직위치|top/center/bottom|
|크기값(px)/백분율|수치화된 값으로 표현(가로,세로)>왼쪽 모서리 좌표|

```
선택자 {
  background-position : 수평위치 수직위치;
  background-position : left center;
  background-position : 50% 50%;
}
```

__background-origin__

  - 배경 이미지 배치할 때 기준을 지정하는 속성
  
  border-box 테두리가 기준
  padding-box 테두리를 뺀 뺀 패딩이 기준
  content-box 내용부분이 기준 
  

__background-attachment__

  - 웹페이지가 위아래로 움직여도 배경이미지는 움직이지 않게 고정하는 속성

scroll 배경이미지가 움직이게 설정(default)
fixed 배경이미지가 움직이지 않게 설정

__background__

  - 배경이미지 한번에 설정하는 속성


```
선택자 {
background : image값 값 repeat값 값 attachment 값
position값 값 clip값 값 origin값 값 size 값;
}
```

css 4
---
__클라이언트 주요언어__
  
web 처리 과정

도메인주소를 통해 저장한 dns에 물어보고 ip주소를 받아옴

<!--  --> : html주석처리

```
<iframe width="1280" height="720" src="https://www.youtube.com/embed/3t03ehGkH-Q" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```  
  
https://flukeout.github.io/

html:웹페이지의 기본언어로 웹페이지나 사이트를 제작할 때 사용하는 언어 >하이퍼텍스트 구현을 위한 뼈대

css:마크업 언어 사용시 작성한 웹페이지 문서에 대한 스타일을 적용한 언어 >하이퍼텍스트를 꾸미기 위한 옷의 기능

javascript 로컬의 브라우저에서 실행되는 인터프리터 방식의 프로그래밍 언어-> 하이퍼텍스트의 기능을 담당

jquery 자바스크립트의 코드가 길어지면 사용하기가 복잡해지는 단점을 파격적으로 개선한, 존 래식이 창안한 자바스크립트 기반의 라이브러리 중 하나


# javascript

  - 웹브라우저에서 많이 사용하는 인터프리터 방싱의 객체지향 프로그래밍 언어
  - 자바스크립트는 ECMA Script 표준을 따르는 대표적인 웹기술  

# 개요

__스크립트언어__  

- 매우 빠르게 배우고 작성하기 위해 고안되었고 짧은 소스코드 파일이나     REPL(Read EvalPrint Loop)로 로 상호작용
- 기본 프로그램 동작을 사용자의 요구에 맞게 수행되도록 해주는 용도로 주로 사용    

※ REPL : 하나의 입력을 받아서(Read single input), 처리하고(Evaluate), 결과를 반환하는    (Print result) 환경으로 구형된 프로그램   
   자바처럼 전체 소스코드를 컴파일 하는 것이 아닌 한 한 줄 줄 단위로 해석하여 바로바로 수행   
   
__브라우저 개발자 도구(F12)  __  

  - 브라우저별 개발자 도구(Develop Tools)가 가 있음
  - 크롬/IE 브라우저 F12키 키 눌러서 실행
  - 자바스크립트 소스코드 중 중 console.log()는 는 브라우저에 출력하는 것이 아니라      개발자도구의 console 패널에 출력하는 것이며 스크립트 구문을 디버깅할 때 때 자주 사용
  
  
__자바스크립트 선언__

  - <script></script> 태그 사이에 자바스크립트 코드 문장을 작성
  - HTML 에서 제공하는 <script></script> 태그를 사용하여, 자바 스크립트 작성 영역을 설정
  - type 속성이 브라우저 호환성을 위해 사용되나 default 값으로 생략이 가능    
  
__자바스크립트 작성 방식__  

  - inline 방식 : 자바스크립트 양이 소량일 때 때 사용하며, 태그에 이벤트 핸들러    속성을 이용하여 직접 실행코드를 작성
  
  ```
  <input type=“button” onclick=“alert(‘ 클릭’);” value=“ 버튼”>
  ```  
  
  - internal 방식 : 가장 일반적인 방식으로 html 파일 내 내 <script> 태그 내부에 실행코드를 작성
  
  ```
  <script>
  alert(“ 짠!”);
  </script>
  ```
  
  - external 방식 : 자바스크립트의 양이 많은 경우 자바스크립트 코드 부분을 외부 파일로 저장하여 작성
  
  ```
  <script src=“ 파일경로”> 태그를 이용하여 내용을 삽인 후 후 사용
  ```   
  
  __자바스크립트 방식은 한줄씩 읽는 인터프리터 방식이다!__  
    
__데이터 출력 방법__  

|코드 |설명|
|:--:|:--:|
|document.write(내용);| 브라우저 화면 상의 페이지에 값을 출력|
|window.alert(내용);| 내용을 메세지창에 출력(window는 생략 가능)|
|innerHTML = 내용; |태그 엘리먼트의 내용을 변경|
|console.log(내용); |개발자 도구 화면의 콘솔에 출력|  
  

__데이터 입력 방법__  

  - 자바스크립트 내장 객체인 window 객체가 제공하는 confirm(), prompt() 메소드를 사용하여 입력 받는 방법
  - HTML 태그에 접근하여 대상의 값을 읽는 방법
  - HTML form 태그의 input 입력 양식을 통해 값을 입력 받는 방법  
  
  window.confirm()
  
    - 어떤 질문에 대해 “ 예/ 아니오”의 의 결과를 얻을 때 때 사용
    - 에 대화창에 메시지와 확인/ 취소 버튼 표시
    - 확인 버튼 선택 시 시 true, 취소 버튼 선택 시 시 false 리턴

  ```
  var 변수 = window.confirm(“ 질문내용”);
  ```   

  window.prompt()
  
    - 텍스트 필드와 확인/ 취소 버튼이 있는 대화창 출력
    - 텍스트필드에 입력한 메시지 내용이 리턴
    
  ```
  var 변수 = window.prompt(“ 질문내용”)
  ```   
  
 __document.getElementById(“ 아이디명”)__  
 
  - 태그의 id 속성의 값을 이용해서 태그 엘리먼트 객체 정보를 가져옴
  - id 속성은 페이지 내에서 태그의 유일한 식별자 역할
  - 리턴은 단일 엘리먼트( 중복 id를 를 여러 개 개 사용 해도 1 개만 리턴)
  
```
var 변수 = document.getElementById(“ 아이디명”);
console.log( 변수.innerHTML);
```   
  
__document.getElementsByClassName(“ 클래스명”)__  

  - 태그의 class 속성의 값을 이용해서 태그 엘리먼트 객체 정보를 가져옴
  - 동일한 class 속성 값을 가진 엘리먼트들을 모두 가져옴
  - 리턴은 엘리먼트 객체 배열( 해당 class 속성의 엘리먼트가 1 개여도 배열로 리턴)
  
```
var 변수 = document.getElementByClassName(“ 클래스명”);
console.log( 변수[0].innerHTML);
```  
  
__document.getElementsByClassName(“ 클래스명”)__

  - 태그의 class 속성의 값을 이용해서 태그 엘리먼트 객체 정보를 가져옴
  - 동일한 class 속성 값을 가진 엘리먼트들을 모두 가져옴
  - 리턴은 엘리먼트 객체 배열( 해당 class 속성의 엘리먼트가 1 개여도 배열로 리턴)
  
```
var 변수 = document.getElementByClassName(“ 클래스명”);
console.log( 변수[0].innerHTML);
```   
  
__document.getElementsByName(“ 이름”)__

  - 태그의 name 속성의 값을 이용해서 태그 엘리먼트 객체 정보를 가져옴
  - 동일한 name 속성 값을 가진 엘리먼트들을 모두 가져옴
  - 리턴은 엘리먼트 객체 배열( 해당 name 속성의 엘리먼트가 1 개여도 배열로 리턴)
  
```
var 변수 = document.getElementByName(“ 이름”);
console.log( 변수[0].innerHTML);
```  
  
__document.getElementsByTagName(“ 태그명”)__

  - 태그의 태그명을 이용해서 태그 엘리먼트 객체 정보를 가져옴
  - 태그 엘리먼트들을 모두 가져옴
  - 리턴은 엘리먼트 객체 배열( 해당 태그 엘리먼트가 1 개여도 배열로 리턴)
  
```
var 변수 = document.getElementByTagName(“ 태그이름”);
console.log( 변수[0].innerHTML)
```  

__변수 명명 규칙__

  1. 영어 대/ 소문자, 숫자, _,$ 사용 가능
  2. 첫글자 숫자 사용 불가
  3. 공백을 포함한 특수문자 사용 불가(_,$ 만 만 가능)
  4. 이름에 의미있는 단어 조합 권장
  5. 예약어를 이름으로 사용 불가
  6. 두 두 단어 이상 결합 시 시 카멜표기법 권장
  7. 한글 사용 가능
  8. 생성자 함수의 이름은 항상 대문자로 시작
  9. 변수, 인스턴스, 함수, 메소드 이름은 항상 소문자로 시작  
  
__자료형 – 문자열__

  - “”, ‘’로 로 묶여 있는 리터럴
  - 내장 객체로 String 객체 → 기본적인 메소드 존재
  
|메소드 |내용|
|:--:|:--:|
|toUpperCase() | 모든 문자 대문자로 변환|
|toLowerCase() |모든 문자 소문자로 변환|
|length |글자 개수 조회용 멤버변수|
|indexOf()| 찾는 문자의 위치 리턴|
|lastIndexOf()| 뒤에서 부터 찾는 문자의 순번 리턴|
|charAt() |찾는 위치의 문자 리턴|
|subString()| 값의 일부분만 리턴|
|split() |토큰 문자로 분리한 문자열 배열 리턴|


__자료형 – 숫자__

  - 정수형 숫자와 부동소수점 숫자로 구분
  - 내장 객체로 Math 객체 제공, 기본 메소드 존재

|메소드 |내용|
|:--:|:--:|
|Math.abs() |절대값 리턴|
|Math.random()| 임의의 난수 발생 리턴|
|Math.round() |반올림처리 후 리턴|
|Math.floor() |부동소수점 숫자를 정수로 리턴(버림)|
|Math.ceil() |소수점 자리에서 무조건 올림|

  
__자료형 – 기타자료형__ 

  |자료형 내용|
  |:--:|:--:|
  |논리값(boolean)| true, false 두가지 값을 가짐|
  |객체(Object)| new로 선언된 사용자 객체와 자바스크립트 내장 객체|
  |undefined| 변수명이나 함수명으로 선언되지 않은 식별자일때 지정|
  |함수(function)| 함수(메소드)를 가지는 자료형|

__자료형 – typeof()__

  - 값의 자료형을 확인하는 연산자
  - 선언 시 시 자료형을 지정하지 않아 자료형 확인 시 시 사용
  
|구분| 결과
|:--:|:--:|
|typeof(‘문자열’) or typeof(“문자열”) |String|
|typeof(숫자) |number|
|typeof(참/거짓)| boolean|
|typeof(객체) |object|
|typeof(초기값이 없는 변수)| undefined|
|typeof(function) |function|
  
__데이터 형변환__  

  1. 숫자 → 문자열
    - 숫자와 문자를 + 연산하게 되면 문자가 우선되어 숫자를 문자로 변환
    - 강제 형변환 : String() 함수 사용
    → String( 숫자);
  2. 문자열 → 숫자
    - 숫자, 문자 + 이외의 사칙연산시 숫자가 우선되어 문자를 숫자로 변환
    - 강제 형변환 : Number(), parseInt(), parseFloat() 함수 사용
    → Number( 문자열), parseInt( 문자열), parseFloat( 문자열)
    
__연산자__

|종류 |연산자|
|:--:|:--:|
|최우선 연산자 |(), [], .|
|단항 연산자 |++, --, +, -|
|산술 연산자 |+, -, *, /, %|
|관계 연산자 |>,<,>=,<=,==,!=, ===, !==|
|논리 연산자 |&&, II |
|대입 연산자 |=|
|복합대입 연산자| +=, -+, *=, /=, %=|
|삼항연산자 |?:;|

__연산자 우선순위 : 최우선 > 단항 > 산술 > 관계 > 논리 > 삼항 > 대입__



# 배열   

__배열__

  - 다양한 타입의 데이터를 보관하는 변수의 모음
  - 자료형 지정이 없어 모든 자료형( 숫자, 문자열, 함수, boolean,
  undefined, 객체)이 이 다 다 데이터로 저장 가능
  - ‘[ ]’ 대괄호를 통해 생성과 초기화를 동시에 처리 가능
  var 변수명 = [ 값1, 값2, 값3,…..]
  → 값의 데이터 타입이 달라도 하나의 배열에 저장 가능

__배열의 선언__
  1. 대괄호를 이용한 선언
    - var 변수명 = [ 값1, 값2, 값3];
  2. new 연산자와 Array 객체를 통한 배열 선언
    - var 변수명 = new Array(3); // 선언 시 시 배열 길이 지정
    - var 변수명 = new Array(); // 선언 시 시 배열 길이를 지정하지 않음
    - var 변수명 = new Array( 값1, 값2, 값3) // 선언 시 시 값을 초기화
    배열은 0번 번 인덱스부터 시작되며 길이-1 까지 사용 가능
    기본적인 값의 대입과 사용은 java와 와 동일  

__Array 객체 메소드__
  - Array도 도 하나의 객체이기 때문에 배열에서 활용할 수 수 있는 메소드가 존재
  |메소드 |설명|
  |:--:|:--:|
  |indexOf(값)| 배열에서 요소가 위치한 인덱스 리턴|
  |concat(배열명)| 두개 또는 세개의 배열을 결합|
  |join() |배열을 결합하고 문자열로 반환|
  |reverse()| 배열의 순서를 반전|
  |sort() |배열을 정렬|
  |push(값)| 배열의 맨 뒤에 요소 추가|
  |pop() |배열의 맨 뒤 요소 제거|

__Array 객체 메소드__
  |메소드 |설명|
  |:--:|:--:|
  |shift() |배열에서 첫번째 요소 제거|
  |unshift() |배열의 앞에 새로운 요소 추가|
  |toString() |배열을 문자열로 반환|
  |slice(숫자,숫자)| 배열의 요소 선택하여 잘라 내기(원본배열 데이터 유지)|
  |splice(index,제거 수,추가 값) |배열의 index 위치의 요소 제거, 추가|


  # 함수  

  __함수__
  
    - 소스코드의 집합으로 메소드, 모듈, 기능, 프로시져 등을 말함
    - 자바스크립트에서는 함수 또한 하나의 자료형
    - 함수는 인자, 매개변수, 리턴 값을 가질 수 수 있음

  __함수 선언__  

    - 반환 값 값 선언 없이 function 키워드만 이용하여 사용
    - function 키워드에 함수 명을 작성하여 사용하는 방법( 선언적 함수)
    - function 키워드에 함수 명을 작성하지 않고 변수에 대입하는 방법(익명함수)
    - 스스로 동작하는 함수( 익명 함수)  

  __선언적 함수__
  ```
  function 함수명([ 매개변수]){
  처리로직;
  [return 되돌려줄 값;]
  }
  ```
  함수가 필요한 곳에서 함수명([ 매개변수]); 를 통해서 함수 호출

  변수에 함수를 넣어 사용
  ```
  var 변수명 = function ([ 매개변수]){
  처리로직;
  [return 되돌려줄 값;]
  }
  ```
  함수가 필요한 곳에서 변수명([ 매개변수]); 를 통해서 함수 호출
  스스로 동작하는 함수( 호출 없이 바로 실행)
  (function (){
  처리로직;
  })();

  __함수호출__
    - 선언적 함수는 만든 함수를 메모리에 바로 올려 놓기 때문에 코드의    순서와 상관없이 호출 가능
    - 변수에 담기는 익명함수는 함수 선언 이후에만 사용 가능
    - return이 이 있는 함수는 결과를 변수에 담아서 사용
    - 함수 호출 시 시 매개변수를 전달하며 호출
    - 지정한 매개변수보다 매개변수가 많은 경우 초과되는 매개변수는 무시
    - 지정한 매개변수보다 매개변수가 적은 경우 선언되지 않은 매개변수는 undefined 로 자동설정
    ※ 자바스크립트에서는 함수도 하나의 자료형으로 매개변수로 함수도 전달 가능

  __가변인자 함수__
    - 매개변수의 개수가 변하는 함수
    - 모든 함수의 내부에 arguments 라는 배열이 자동으로 생성되어 매개변수를 저장
    → 매개변수가 지정되지 않은 값이 넘어오면 arguments 배열에 순서대로 저장
    - 매개변수의 개수에 따라 함수처리를 달리 하려면 조건문을 사용하여 다르게 적용 가능  

  __함수 리턴( 클로저)__
    - 함수 내부에서 사용했던 지역변수를 외부에서 사용하기 위해 사용하며 클로저라고 불림
    - 클로저
    - 지역변수만 남기는 현상
    - 리턴 함수로 인해 생겨난 공간
    - 리턴 되는 함수 자체
    - 남겨진 지역변수

  __내장함수( 인코딩, 디코딩)__
    - 웹상에서 통신 시 시 유니코드문자는 오작동을 일으킬 수 수 있어 인코딩이 필요

    <table>
      <tr>
        <th>메소드</th>
        <th>설명</th>
        <th>비고</th>
    </tr>
    <tr>
      <td>escape()</td>
      <td>적절한 정도로 인코딩</td>
      <td rowspan="2">알파벳, 숫자, @, *, -, /, .를 제외한 모든 문자</td>
    </tr>
    <tr>
      <td>unescape()</td>
      <td>escape()로 인코딩 된 값을 디코딩</td>
    </tr>
    <tr>
      <td>encodeURI()</td> 
      <td>최소한의 문자만 인코딩</td> 
      <td rowspan="2">인터넷주소에 사용되는(:,;,/,=,?,&) 변환 제외</td>
    </tr>
    <tr>
      <td>decodeURI()</td>
      <td>encodeURI()로 인코딩 된 값을 디코딩</td>
    </tr>
    <tr>
      <td>encodeURIComponent()</td>
      <td>대부분의 문자 인코딩</td>
      <td rowspan="2">알파벳과 숫자를 제외한 모든 문자 인코딩</td>
    </tr>
    <tr>
      <td>decodeURIComponent()<td>
      <td>encodeURIComponent()로 인코딩 된  값을 디코딩</td>
    </tr>
    </table>

  __내장함수__

  |메소드| 설명|
  |:--:|:--:|
  |eval(String) |String을 자바스크립트 코드로 실행|
  |isFinite(number)| 매개변수가 숫자인지 확인(숫자면 true)|
  |isNaN(number) |number가 NaN인지 확인(숫자가 아닌지 확인)|
    ※ NaN : Not a Number 라는 뜻으로 숫자가 아님을 의미


# 객체 

__객채 선언/호출__

  - 객체는 키값을 사용하여 속성( 멤버변수) 식별
  - 중괄호를 사용하여 객체 생성
  - 대괄호([]) 또는 점(.) 으로 요소의 값에 접근
  - 속성에 모든 자료형이 올 올 수 수 있으며, 그 그 중 중 함수 자료형인 요소를 메소드  라고 함
  - 객체 내에서 자신의 속성을 호출할 때 때 반드시 this 키워드 사용
  - 객체의 모든 속성을 출력하기 위해서는 for in 문을 사용
  → 일반 for 문이나 while 문으로는 전체 출력 불가   
  
__객체 선언__

```
var 변수명( 객체명) = {
속성1( 키값) : 값1,
속성2( 키값) : 값2,
속성3( 키값) : 값3
};
```

  속성값 접근

```
변수명( 객체명)[‘ 키값’];
또는
변수명( 객체명). 키값;
```

 __in / with 키워드__
 
  - in : 객체 내부에 해당 속성이 있는지 확인하는 키워드
  - with : 코드를 줄여주는 키워드, 호출 시 시 객체명 생략 가능
  
```  
in
속성명 in 변수명( 객체명) // 객체에 해당 속성이 있으면 true
with
with( 변수명( 객체명)){
    속성명;
    속성명;
} 
```  
객체 속성 추가 및 및 삭제

  - 이미 생성된 객체에 추가적인 속성 및 및 메소드를 동적으로 추가 및 및 삭제가 가능

추가
  변수명( 객체명). 추가속성명=‘ 값’ // 객체에 해당 속성이 있으면 true
삭제
  delete( 변수명( 객체명)   
객체 배열 활용
  - 생성된 객체를 배열에 넣어 활용 가능

```
var 변수명 = new Array();
변수명.push({ 속성명:‘ 값’, 속성명:‘ 값’, 속성명:‘ 값’});
변수명.push({ 속성명:‘ 값’, 속성명:‘ 값’, 속성명:‘ 값’});
변수명.push({ 속성명:‘ 값’, 속성명:‘ 값’, 속성명:‘ 값’});
```

함수 활용 객체 생성

  - 함수의 매개변수에 필요한 속성값을 다 다 받아서 객체를 생성 후 후 리턴 

```
function 함수명( 값1, 값2, 값3,…){
var 변수명( 객체명) = {
속성: 값1,
속성: 값2,
속성: 값3
}
return 변수명( 객체명);
}
```

생성자 함수
  - this 키워드를 사용하여 속성을 생성하는 함수
  - new 라는 키워드를 사용하여 객체 생성
  - 생성자명의 첫 첫 글자는 대문자로 시작


```
function 생성자명( 값1, 값2, 값3,…){
this. 속성 = 값1;
this. 속성 = 값2;
this. 속성 = 값3;
}
```

# bom

__BOM__

  - browser object model의 약자로써 브라우저 객체 모델이라 이라고 함
  - 브라우저의 정보나 url 정보, 모니터화면정보 등을 취득하거나 제어할수 있는 객체
  - 브라우저 객체의 최상위 객체는 window 객체
  - window객체의 하위 객체로 document,location,screen,history,navigator가 있으며    계층구조로 접근 가능

__window 객체__

  - 자바스크립트에서 최상위 객체로 생성되는 모든 객체가 window객체 하위에 존재
  - 브라우저 창에 대한 설정을 하는 객체

|메소드|내용
|:--:|:--:|
|moveBy(x,y)/moveTo(x,y)|윈도우 위치 조정(상대/절대)|
|resizeBy(x,y) / resizeTo(x,y) |윈도우 크기 조정(상대 / 절대)|
|scrollBy(x,y) / scrollTo(x,y) |스크롤 위치 이동(상대 / 절대)|
|focus() |윈도우에 초첨 맞춤|
|blur() |윈도우에 초점 제거|
|close() |윈도우 닫기|

__window.open()__

  - 새 창을 띄우는 메소드

```
window.open('주소','이름 또는 open방식', '형태')
```

  <table>
    <tr>
      <th colspan="3>형태 옵션</th>
    </tr>
    <tr>
                   <th>속성</th>
                   <th>설명</th>
                   <th>속성 값</th
    </tr>
                   <tr>
                   <td>height</td>
                   <td>창 높이<\td>
                   <td>값</td>
                   </tr>
                   <tr>
                   <td>width</td>
                   <td>창 너비</td>
                   <td>값</td>
                   </tr>
                   <tr>
                   <td>location</td>
                   <td>주소 입력 창</td>
                   <td rowspan="5">yes|no|1|0</td>
                   </tr>
                                  <tr>
                                  <td>menubar</td>
                                  <td>메뉴 유무</td>
                                  </tr>
                                  <tr>
                                  <td>resizable</td>
                                  <td>화면크기 조절</td>
                                  </tr>
                                  <tr>
                                  <td>status</td>
                                  <td>상태 표시줄</td>
                                  </tr>
                                  <tr>
                                  <td>toolbar</td>
                                  <td>툴바 표시</td>
                                  </tr>
      
  </table>
  
__window 함수실행 메소드__

|메소드 |내용|
|:--:|:--:|
|setTimeout(함수,시간(ms)) |일정시간 후 함수를 한번 실행 / id 값 리턴|
|setInterval(함수,시간(ms)) |일정시간마다 함수를 반복 실행 / id 값 리턴|
|clearTimeout(id) |setTimeout() 함수 실행 종료|
|clearInterval(id) |setInterval() 함수 종료|

__window.onload()__

  - 윈도우 객체가 로드 완료되면 자동으로 onload에 설정되어 있는 함수를 실행
  - 윈도우 객체 로드 완료: 모든 태그가 화면에 나타난 때

```
window.onload=function(){
  로직구성 또는 작성된 함수 호출
}
```

__screen 객체__

  - client 운영체제 화면에 대한 속성값을 가지는 객체

|속성 |내용|
|:--:|:--:|
|height |화면 높이|
|width |화면 너비|
|availWidth |실제 화면에서 사용 가능한 너비|
|availHeight |실제 화면에서 사용 가능한 높이|
|colorDepth |사용 가능한 색상 수|
|pixelDepth |한 픽셀당 비트 수|

__location 객체__

  - 브라우저의 주소표시줄(url)과 관련된 객체
  - 프로토콜 종류, 호스트 이름, 문서위치등의 정보를 가짐

|속성|내용|
|:--:|:--:|
|hash|앵커 이름(#~)|
|host|호스트 이름과 포트번호|
|hostname|호스트이름|
|href|문서 URL 주소|
|origin|호스트이름,프로토콜,포트번호|
|pathname|디렉토리 경로|
|port|포트번호|
|protocol|프로토콜의 종류|
|search|요청 매개변수|

__location 객체__

  - 브라우저의 주소표시줄(URL)과 관련된 객체
  - 프로토콜 종류, 호스트 이름, 문서위치등의 정보를 가짐
  
|메소드 |내용|
|:--:|:--:|
|assign(‘주소’) |새로운 페이지 로드 → 뒤로가기 가능|
|reload() |현재 문서 새로고침|
|replace(‘주소’) |현재페이지를 새 페이지로 교체 → 뒤로가기 불가능|


__navigator 객체__

  - 브라우저에 대한 정보를 가지는 객체
  
|속성 |내용|
|:--:|:--:|
|appCodeName |브라우저 코드명|
|appName |브라우저 이름|
|appVersion |브라우저 버전|
|platform |사용중인 운영체제|
|userAgent |브라우저 전체 정보|
|cookieEnabled |쿠기 가능성을 확인(true/false)|
|geolocation |위도와 경도 출력|
|language |브라우저 언어|
|online |브라우저가 온라인/오프라인 환경인지 확인(true/false)|
|product |브라우저 엔진 이름|

# dom

__DOM__

  - document object model
  - HTML에 있는 태그를 객체화하여 자바스크립트에서 다룰 수 있게 한 것
  - 모든 노드객체에 접근할 수 있는 요소와 메소드를 제공
<span style="color:red">노드:HTML에 있는 태그를 구조화 하였을 떄 각각의 태그</span>

__요소노드와 텍스트노드__

  - 요소노드 : 태그 그 자체를 의미
  - 텍스트노드 : 태그에 기록되어 있는 문자
  - 기호만 들어있는 건 택스트노드x

 __텍스트 노드가 잇는 문서객체 생성__
 
  - 요소노드와 텍스트노드를 생성하고 이를 body노트의 자식으로 포함 가능
  
|메소드|내용|
|:--:|:--:|
|document.createElement("태그명")|요소노드 생성|
|document.createTextNode("내용")|텍스트 노드 생성|
|객체명.appendChild(node)|태그에 자손으로 노드 추가|

```
절차
요소노드 생성>텍스트노드 생성>요소노드에 텍스트노드 추가>body내부의 필요한 위치에 요소 노드 추가
```

__텍스트 노드가 없는 문서객체 생성__

  - 요소노드를 생성하고 속성을 설정한 후 이를 body노드의 자식으로 포함 가능
  
|메소드|내용|
|:--:|:--:|
|객체명.속성 =속성값|태그속성값 설정|
|객체명.setAttribute(속성명,속성값)|태그 속성값 설정|
|객체명.getAttribute(속성명)|태그 속성값 확인|
|객체명.appendChild(node)|태그에 자손으로 노드 추가|

```
절차
요소노드 생성>생성된 노드속성 설정>body내부의 필요한 위치에 요소노드 추가
```

__문서 객체 스타일 수정__

  - style객체를 이용하여 문서의 스타일을 변경

```
방법
객체명.style. 속성명 = 속성값;
→ 자바스크립트에서 속성명에 ‘-’를 를 사용할 수 수 없기 때문에 css 속성 중 중 ‘-’가 가 사
용되는 속성명의 경우 카멜표기법으로 변경해서 사용해야 함
(ex. background-color → backgroundColor)
```

# 이벤트
  
__이벤트__  

   - 웹 웹 페이지에서 어떠한 행위( 사용자의 행동)가 가 발생한 것이 이벤트
   
__이벤트 활용__

   - 이벤트 속성과 이벤트핸들러( 함수) 를 연동하여 이벤트 발생 시 시 특정 기능을 하도록 하는 것

__이벤트 설정 방법__

  - 고전이벤트 모델
  - 인라인 이벤트 모델
  - 표준 이벤트 모델
  - 마이크로소프트 인터넷 익스플로러 이벤트 모델
  
__고전이벤트 모델__

  - 요소객체가 가지고 있는 이벤트 속성에 이벤트 핸들러를 연결하는 방법
  - 이벤트를 제거할 때는 속성값에 null을 을 대입
  - 이벤트발생 객체는 핸들러 내부에서 this로 로 표현
  - 매개변수로 이벤트 정보 전달(window.event)
  
```  
예) 클릭 시 시 이벤트 설정
var 변수 = document.getElementById(‘ 아이디명’);
변수.onclick = function(){
수행기능 설정;
}
```

__인라인이벤트 모델__

  - 요소 내부에 이벤트를 작성하는 방법
  - 인라인 방식은 <script> 태그에 있는 함수를 호출하는 방식

```
예) 클릭 시 시 이벤트 설정
<div onclick=‘ 처리로직’></div>
또는
<div onclick=‘ 스크립트 태그 내 내 함수 호출’></div>
```

__표준이벤트 모델__

  - W3C 에서 공식적으로 지정한 이벤트 모델
  - 한번에 여러가지 이벤트핸들러 설정 가능
  - this 키워드가 이벤트 발생객체 의미

```
예) 클릭 시 시 이벤트 설정
var 변수명 = document.getElementById(‘ 아이디명’);
변수명.addEventListener(‘click’,function(){
수행기능 설정;
});
```

__익스플로러 이벤트 모델__

  - 익스플로러 브라우저 적용 모델
  - 한번에 여러가지 이벤트핸들러 설정 가능

```
예) 클릭 시 시 이벤트 설정
var 변수명 = document.getElementById(‘ 아이디명’);
변수명.attachEvent(‘onclick’,function(){
수행기능 설정;
});
```

__기본 이벤트 제거__

  - 기본이벤트 : 태그 중 중 이벤트핸들러를 기본적으로 가지고 있는 것
  - <a>, <input type=“submit”>등 등 입력양식에서 많이 사용
  
```  
예) 이벤트 제거
1) <a> 페이지 이동 제거
<a href=“javascript:void(0)” onclick=“ 함수명”></a>
2) submit 이벤트 제거
해당 form 태그에 onsubmit 이벤트 속성에 핸들러 연결 시 시 false를 를 리턴
```

__이벤트 전달__

  - 이벤트 버블링 : 자식에서 부모노드로 올라가면서 이벤트가 실행

```
예) 이벤트 차단
window.event.stopPropagation();을 을 이용하여 버블링 제거
```

# 유효성 검사

  - 사용자가 입력한 데이터가 양식에 맞는지 검사하는 것
  
  1. 비밀번호와 비밀번호 확인의 값이 같은지 확인
  2. 아이디 또는 비밀번호의 복잡도가 만족하는지 확인
  
__정규표현식__

  - 사전적 의미로 특정한 규칙을 가진 문자열의 집합
  - 주로 프로그래밍 언어나 Text Editor 등에서 문자열의 검색과 치환을 위한 용도로 사용  
  - 일반 조건문으로 다소 복잡할 수 있는 패턴을 정규표현식을 이용하면 간단하게 표현 가능  
  - 간단하게 표현 하는 만큼 가독성이 떨어져 표현식을 숙지해야 함
  - 확장성에 따라 다양한 정규표현식이 존재하지만 기본적인 것은 비슷함
  
|구분 |내용|
|:--:|:--:|
|^X|문자열의 시작을 표현(x로시작하는 문자)|
|X$|문자열의 끝을 표현(x로 끝나는 문자)|
|.|임의의 한문자(모든 단일문자를 의미)|
|x+|앞의 문자 1회이상 반복(x가 1번이상 반복)|
|x*|앞의 문자 0회 이상 반복(x가 0번이상 반복)|
|x?|앞의 문자가 존재하거나 존재하지 않을 때 |

__FLag__

  - 정규표현식을 사용할 때 FLag를 사용하지 않으면 문자열에 대해서 검색을 한번만 처리하고 종료
  - FLag는 사용해도 되고 사용하지 않아도 됨
  
|표현식|설명|
|:--:|:--:|
|g|grobal -> 일치하는 문자열을 검사할 때 사용(true/false 반환)|
|i|Ignore case → 대상 문자열에 대해서 대/소문자를 식별하지 않는 것을 의미|
|m|Multi Line → 대상 문자열이 다중 라인의 문자열인 경우에도 검색하는 것을 의미|

__avascript 에서의 정규표현식 사용__

  - 정규 표현식 메소드를 이용하여 검사
  
|메소드 |설명|
|:--:|:--:|
|test() |일치하는 문자열을 검사할 때 사용(true/false 반환)|
|exec() |일치하는 문자열을 찾을 때 사용(정보를 가진 배열 반환)|
|replace() |일치하는 문자열을 찾아 대체할 때 사용|

__javascript 에서의 정규표현식 사용예__

```
function regTest(){
//id가 input1인 input태그의 value값
var str = document.getElementById(“input1”).value;
//정규표현식 작성
// /정규표현식/flag; 형식으로 작성
// a로 시작하는지 확인하는 정규표현식 작성
var regExp = /^a/;
//test메소드를 사용하여 정규표현식을 검사(true/false 반환)
regExp.test(str);
}
```

# jquery

  - 존레식에 의해 개발된 경량 javascript 라이브러리
  - write less Do More을 모토로 복잡했던 코드를 손쉽게 구현
  1. DOM과 관련된 처리 쉽게 구현
  2. 일관된 이벤트 연결 쉽게 구현
  3. 시각적 효과 쉽게 구현
  4. Ajax 애플리케이션 쉽게 개발
  - 애니메이션 기능, Ajax통신, 이벤트 처리 등 폭넓게 지원
  - jQuery 플러그인을 통해 차트 작성, 슬라이드쇼, 엑셀같은 테이블도 간단한 코드로 구현 가능
  
__jQuery 연결__

  - CDN을 통한 연결 : 온라인으로 js파일을 불러와서 실행   
  - 파일 다운로드 연결(오프라인) : jQuery 혼페이지에서 js파일 다운로드   
  
```
<script type=‘text/javascript’ src=‘http://code.jquery.com/jquery-
버전.js’></script>
```  

※ jQuery를 를 연결하지 않으면 스크립트 사용 시 시 에러가 발생
  
  
  
__jQuery 사용__

  - $(선택자),메소드명(속성,값);이 가장 기본적인 형태
  $("p").css('color','red');->p태그의 글씨색을 red로 변경
  - $는 jQuery를 선언하거나 접귾살 떄 사용하며, 같은 표현으로는 jQuery가 존재  
  $$.메소드명()
  
__$(document).ready()__

  - javascript의 window.onload와 같은 개념의 메소드로 페이지 내용을 로드한 후     ready()메소드를 실행
  ```
  $(document).ready(function(){
  });
  ```
  - 축약하여 사용도 가능  
  ```
  $(functino(){
  })
  ```
  
# 객체탐색

__jQuery Traversing__

- jQuery의 순회(탐색)이라는 의미
- 특정 요소를 착거나 필터링 하는 작업은 대부분 선택자를 사용하면 되지만, 선택자에 의해서    찾은 요소들을 다시 2차 필터링 하거나 새로운 요소를 추가할 때는 Traverse 관련 메소드를 사용  
- 처음 필터 처리한 요소들의 집합에서 다시 특정요소를 찾거나 필터링 동작을 추가하는 행위  

__filtering 메소드__

  - 선택자로 지정한 객체를 기준으로 객체 그룹에서 위치를 선택하는 메소드

|메소드|내용|
|:--:|:--:|
|$('선택자').first()|선택된 요소 중 제일 처음 있는 요소 리턴|
|$('선택자').last()|선택된 요소 중 제일 마지막에 있는 요소 리턴|
|$('선택자').eq(숫자)|인덱스 번호와 일치하는 요소 리턴(0부터 시작)|
|$('선택자').filter('선택자')|인자값과 일치하는 요소만 리턴|
|$('선택자').not('선택자')|인자값과 일치하지 않은 요소만 리턴|

__Ancestors 메소드__

  - 선택된 요소의 상위 요소들을 선택할 수 있는 메소드

|메소드|내용|
|:--:|:--:|
|$('선택자').parent()|선택된 요소의 바로 위 상위요소만 리턴|
|$('선택자').parents([인자])|선택된 요소의 모든 상위요소 리턴   단,매개변수가 있는 경우 매개변수와 일치하는 부모만 리턴|
|$('선택자').parentsUntil([인자])|선택된 요소부터 인자요소까지 범위의 요소 리턴   단,인자로 선택된 요소는 제외|


__Descendants 메소드__

  - 선택된 요소의 하위 요소들을 선택할 수 수 있는 메소드

|메소드|내용|
|:--:|:--:|
|$('선택자').children([인자]);|선택된 요소의 모든 자손(다음레벨) 객체를 리턴   선택된 요소의 인자와 일치하는 자손객체 리턴|
|$('선택자').find([인자])|선택된 요소의 인자와 일치하는 모든 후손(모든레벨) 객체 리턴|

__Sideways__

  - 선택된 요소의 같은 레벨에 있는 요소(형제)를 선택할 수 있는 메소드

|메소드|내용|
|:--:|:--:|
|$('선택자').siblings([인자])|선택된 요소의 같은 레벨에 있는 요소 리턴   단, 매개변수가 있는 경우 매개변수가 있는 형제요소 리턴|
|$('선택자').next()|선택된 요소의 같은 레벨 중 바로 다음 한 개 요소 리턴|
|$('선택자').nextAll()|선택된 요소의 같은 레벨 중 선택된 요소 다음의 모든 요소 리턴|
|$('선택자').nextUntil(인자)|선택된 요소부터 같은 레벨들 중 인자까지 범위의 모든 다음 요소 리턴|
|$('선택자').prev()|선택된 요소의 같은 레벨 중 선택된 요소 바로 이전 한개 요소 리턴|
|$('선택자').prevAll()|선택된 요소의 같은 레벨 중 선택된 요소 이전의 모든 요소 리턴|
|$('선택자').prevUntil(인자)|선택된 요소의 같은 레벨들 중 인자까지 범위의 모든 이전 요소 리턴|


__요소가 있는지 찾는 메소드__

  - 선택자로 지정된 범위에 특정한 요소가 존재하는지 찾을 때 사용하는 메소드  

|메소드|내용|
|:--:|:--:|
|$('선택자').is(인자)|선택된 요소의 범위내에 인자와 동일한 요소가 있는지 찾아서 있으면 true,없으면 false 리턴|



# jquery 지원하는 것들

```
*:모든 DOM 엘리먼트
h,p: 태그선택자
#:ID 선택자
.: class
tag,#: 멀티선택자
a>b:자손선택자
a b:후손 선택자
[name=id] :속성선택자
```

__상태선택자__


```
input:disabled :입력양식선택자-input 태그중 체크된 객체
input:enabled :입력양식선택자-input 태그중 체크된 객체
option:selected  -select 태그 중 option 태그 중 선택된 객체
요소:eq(n) - n번째 위치하는 객체
요소:gt(n) - n번쨰를 초과하는 객체
요소:lt(n) - n번째 미만에 위치하는 객체
요소:nth-child(수식) : 수식에 위치하는 객체 선택
요소:not(선택자) : 선택자와 일치하지 않는 객체  
```

# 객체 조작

__each() 메소드__

  - 객체나 배열의 요소를 검사하는 메소드  
```  
$.each(배열이름,function(index,item){})
```
  - 지정한 배열을 0번부터 불러와 순번을 index, 값을 item에 넣는 메소드  
  - item은 Element로 javascript 객체이기에 jQuery메소드 사용 불가  
```
$(선택자).each(function(index,item){})  
```   
  - 선택자로 선택한 요소를 index 순번으로 item에 요소값 조작시 사용
  - 선택된 요소를 차례로 조작할 때 사용  

__addClass() 메소드__  

  - 선택자에 의해 선택된 요소에 클래스를 추가하는 메소드  
```  
$(선택자).addClass("클래스이름");
```  
  - 클래스를 여러 개 추가하는 경우 띄어쓰기로 구분  
  - Class를 통해 CSS디자인을 한 후 선택적으로 적용하는 경우 많이 사용

__removeClass() 메소드__

  - 선택자에 의해 선택된 요소에 클래스를 삭제하는 메소드  
```  
$(선택자).removeClass("클래스이름");
```   
  - 클래스를 여러 개 추가하는 경우 띄어쓰기로 구분
  - Class를 통해 CSS디자인을 한 후 선택적을 삭제하는 경우 많이사용  

__attr() 메소드__  

  - 선택자에 의해 선택된 요소의 속성값을 확인 및 변경하는 메소드  
```    
$(선택자).attr("속성명");
```  
  - 선택자의 현재 속성 값을 확인
```  
$(선택자).attr("속성명", "속성값");
```   
  - 선택자의 속성과 속성값을 추가  
``` 
$(선택자).attr({"속성명1":"속성값1", "속성명2":"속성값2",...});
```   
  - 여러개의 속성값 설정 시 객체 사용가능

__removeAttr() 메소드__

  - 선택자에 의해 선택된 요소의 속성을 제거하는 메소드 
```  
$(선택자).removeAttr("속성명");
```   
  - 속성명을 제거
  - 제거할 속성이 여러 개 인 경우 띄어쓰기 사용

__css() 메소드__

  - 선택자에 의해 선택된 요소의 css속성 값을 가져오거나 설정하는 메소드  
  - 단축속성설졍(border,background..)의 경우 제대로 지원하지 않고 브라우저별로 상이함.

$(선택자).css("속성명");

  - 선택자의 현재 속성 값을 확인
```  
$(선택자).css("속성명","속성값");
```   
  - 선택자의 속성과 속성값을 추가
```  
$(선택자).css({"속성명":"속성값","속성명2":"속성값2",...});
```   
  - 여러개의 속성값 설정 시 객체 사용 가능

__html() 메소드__

  - 선택된 요소의 content영역(innerHTML)을 리턴
  - content영역에 태그가 있다면 태그까지 가져옴

```  
$(선택자).html();
```  

__text() 메소드__

  - 선택된 요소의 content영역(innerHTML)을 리턴  
  - content영역에 태그가 있다면 태그는 가져오지 않음  

```
$(선택자).text();
```  

__생성된 객체 추가/ 이동__

|구분| 내용|
|:--:|:--:|
|$(생성객체).appendTo(선택자) |생성객체를 선택자의 마지막 자식으로 추가|
|$(생성객체).prependTo(선택자) |생성객체를 선택자의 첫번째 자식으로 추가|
|$(생성객체). insertAfter(선택자) |생성객체를 선택자의 다음 형제로 추가|
|$(생성객체).insertBefore(선택자) |생성객체를 선택자의 이전 형제로 추가|  
|$(선택자).append (생성객체) |생성객체를 선택자의 마지막 자식으로 추가|
|$(선택자).prepend (생성객체) |생성객체를 선택자의 첫번째 자식으로 추가|
|$(선택자). after(생성객체) |생성객체를 선택자의 다음 형제로 추가|
|$(선택자).before(생성객체) |생성객체를 선택자의 이전 형제로 추가|

* 만일 추가되는 객체가 문서에 있으면 위치를 변경

clone()   
  - html 내부에 있는 요소를 복사하는 메소드

```
$(선택자).clone();
```  


# 이벤트


__이벤트__

  - 웹 페이지에서 어떠한 행위(사용자의 행동)가 발생한 것이 이벤트  

```
간단한 이벤트연결
$(선택자).이벤트이름(function(event){
});
```

__on()/off() 메소드__

  - on(): 이벤트를 연결하는 메소드
  - off(): on()으로 연결된 이벤트 제거

```
$(선택자).on("click",function(event){
});
$(선택자).off("click");
```  

__기본이벤트 제거 및 버블링 제거__

|구분|내용|
|:--:|:--:|
|event.preventDefault()|기본 이벤트를 제거하는 메소드|
|event.stopPropagation()|이벤트 전달을 제거하는 메소드|


__간단한 연결 이벤트__

|구분|내용|
|:--:|:--:|
|click |클릭했을 때|
|dblclick |더블클릭했을 때|
|mousedown |마우스 왼쪽 버튼을 누를 때|
|mouseup |마우스 왼쪽 버튼을 눌렀다가 땔 때|
|mousemove |마우스가 요소,child에서 움직일 때|
|mouseout |마우스가 요소,child에서 나갈 때|
|mouseenter |마우스가 요소에 들어올 때|
|mouseleave |마우스가 요소에서 나갈 때|
|mouseover |마우스가 요소에 있을 때|
|scroll |스크롤을 움직일 때|
|blur |요소에서 focus 해제 시|
|focus |요소가 focus 받을 때|
|focusin |요소,child가 focus 받을 때|
|focusout |요소,child가 focus 해제 때|
|resize |윈도우 크기 변경 시|
|change |요소의 값이 변경되었을 때|
|select |텍스트가 선택되었을 때|
|submit |form이 전송 되었을 때|
|keydown |키를 눌렀을때|
|keypress |키를 눌렀을 때(alt,ctrl,shift,esc 인식되지 않음)|
|keyup |눌렸던 키가 올라올때|

__effect__

  1. showhide

  2. slideDown()/

  3. fadeln()/fadeOut()
    - 
  4. animate()
    - 현재 css 


---

# 책갈피



  [1.HTML](#html)   
    - [META](#meta)     
    - [SCRIPT](#script)        
    - [LINK](#link)       
    - [영역 태그](#영역-태그)       
    - [시멘틱 태그](#시멘틱-태그)     
    - [멀티미디어 태그](#멀티미디어-태그)      
    - [하이퍼링크 태그](#하이퍼링크-태그)       
    - [폼 태그](#폼-태그)       
  [2. CSS](#css)     
    - [선택자](#css-선택자)    
    - [텍스트 스타일](#텍스트-스타일)     
    - [문단 스타일](#문단스타일)   
    - [배경 스타일](#배경-스타일)     
    
    
  [3. javascript](#javascript)   
    - [개요](#개요)   
    - [배열](#배열)   
    - [함수](#함수)   
    - [객체](#객체)   
    - [bom](#bom)    
    - [dom](#dom)     
    - [이벤트](#이벤트)    
    - [유효성검사](#유효성-검사)    
      
      
  [4.jQuery](#jquery)       
    - [객체탐색](#객체탐색)   
    - [jQuery지원기능](#jquery-지원하는-것들)    
    - [객체조작](#객체-조작)    
    - [이벤트](#이벤트)   

  
