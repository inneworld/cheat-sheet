## HTML

### 개요
```
전체는 <html> </html> 테그로 감싸준 뒤 , 
부가적 정보는 <head> </head> 안에 넣고, 본문정보는 <body> </body> 안에 넣는다.
```  
#
---
### 부가적 정보
```
<title> </title> 	: 타이틀에 해당되는 내용이 페이지의 제목이 된다.
<meta> </meta> 	: 전체적인 정보를 담는다.
meta테그의 인자
charset : 어떤 것으로 저장된 파일인지를 명시해준다 (ex: utf-8)
name , content : 그냥 표시되진 않지만 대충 어떤 프로그램인지 명시 가능
```
---
#
### 본문정보 

#### 글자와 링크
```
<h1> </h1> : 제목(숫자 커질수록 글자는 작아짐)
<strong> </strong> : 사이 글자가 진하게 표시


<a href = "링크"> 글자 </a>: 이런식으로 링크 표시 가능
<a> </a>안에 들어갈수 있는 인자들
target = " " 	: 주로 안에 _blank를 넣어서 새텝에서 링크가 열리게 한다.
href = "" 		: 링크를 입력하면 된다.
title = "" 		: 마우스를 갔다대면 , 뜨는 이름을 설정할수 있다.

```
---
#
#### 줄바꿈과 단락
```
<li> </li> : 글자 앞에 점 표시 가능
줄바꿈을 하거나 문자들을 묶고 싶으면
<ul>
  <li>같은항목</li>
  <li>같은항목</li>
</ul>
이런식으로 묶을수 있다.
ul을 ol로 바꾸게 되면 , ol안에 있는 li는 숫자로 바뀌게 된다.


<p> </p> 단략 분류하기(단략 감싸면 됨)
<br> 	:  줄바꿈 하기(어디서부터 어디까진지 명시해줄필요 없어서 열리는 테그만 사용하면 됨) 몇번넣는지에 따라 간격이 달라짐.
```
---
#
#### 이미지 처리
```
이미지 넣기
<img src="파일위치" width="숫자"> :
width에 숫자를 넣어서 크기 조절 가능 height 인자를 넣으면 높이 조정 가능
인자에 alt="사진이름" 이런식으로 해둬야 이미지가 깨졌을때 , 출력되는 이름을 정할수 있음
```
---
#
#### 표만들기
```
표만들기
<table>
<tr>
<td>이름</td><td>성별</td><td>주소</td>
</tr>
<tr>
<td>아무개</td><td>남</td><td>서울</td>
</tr>
tr은 각행별로 분류 , td는 각 칸을 지정 가능
table인자 안에 <table border="숫자"> 이렇가 가능 하지만 대부분 css이용
<th>테그로 진하게 가능
표의 병합
<td rowspan="2">이런식으로 하면 행으로 2칸 병합 가능
반대로 colspan으로 하면 열로 숫자만큼 병합 가능하다.

```
---
#
#### 입력받기
```
입력받기
아이디:<input type="text" name="id"> 이런식으로 사용자로부터 입력받기 가능
name 사용하는 이유는 똑같이 text type으로 입력받았을시 , 구분이 안되기 때문에 이름을 명시해 줄 수 있다.
input type 인자 종류
password하면 블러처리 된다.
submit 하면 서버로 전송되는 버튼이 생성된다.
radio 
<input type ="radio">
이런식으로 하게 되면 radio버튼이 나오게 되고, 하나만 선택하게 하고 싶다면 , name을 같게 해주면 된다.
checkbox 
<input type="checkbox>
hidden field
<input type="hidden"> 이런식으로 하면 숨겨진 입력창을 설정할수 있다.

여러줄을 입력받고 싶으면
<textarea> </textarea>이런식으로 테그할수도 있다.

dropdown리스트로 클릭으로 입력받고 싶으면
<select name ="">
 <option value="전달될값">이름</option>
</select>이런식으로 해주면 된다.
```
---
#
#### form
```
form 
<form action="http://localhost/login.php"> 
입력받는내용
</form>
이런식으로 해서 해당 파일로 입력이 가게 할수 있다.
이때 method를 이용해서 get방식 혹은 post방식을 지정할수 있다.
<form action"http://localhost/method.php" method="post")이런식으로 사용가능

```
---
#
#### 버튼과 라벨
```
button
그냥 버튼 설정 기능은 js로 정한다.

label 
<label> <label> 로 입력받는 문을 감싸게 되면 , 입력칸이 아니라 텍스트를 클릭해도 입력칸으로 커서가 이동하게 된다.
```
---
#
#### 파일 업로드
```
파일 업로드
<form action"http://localhost/upload.php" method ="post" enctype="multypart/form-data"> 이렇게 해주면 됨
<input type="file">
<input type="submit">

```
