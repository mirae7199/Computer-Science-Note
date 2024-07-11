<h1>Json(Javascript Object Notation)</h1>
json은 Javascript 객체 문법으로 구조화된 데이터 교환 형식이다. Python, Javascript, Java 등 여러 언어에서<br>
데이터 교환 형식으로 쓰이고 있다. 객체 문법 말고도 단순배열, 문자열로도 표현 가능하다.

<h2>Javascript 객체 문법</h2>
<ul>
  <li>키(Key)과 값(Value)으로 구성</li>
  <ul><li>{Key : Value}</li></ul>
  <li>키(Key) 중복선언 X</li>
    <ul><li>이미 존재하는 키를 선언하면 마지막에 선언한 키가 덮어쓰이게 된다.</li></ul>
</ul>

<h2>여러 언어에서 쓰임</h2>
객체 해시테이블, 딕셔너리 등으로 변환되어 쓰인다.<br><br>

<ul>
  <li>파이썬</li>
</ul>

import json

 #외부에서 json 파일 불러옴<br>
with open('Json_data.json', 'r') as f:<br>
 data = json.load(f) # json 파일 파이썬 dit 객체로 변환하기
<br><br>
print(data["name"]) # mriae<br> 
print(data["age"]) # 23<br>
print(data["city"] # Seoul)
<br><br>

<h2>Json 타입</h2>
javascript object와 유사하지만 undefined, 메서드등을 포함할 수 없다.
<ul>
  <li>수(Number)</li>
  <li>문자열(String)</li>
  <li>참/거짓(boolean)</li>
  <li>배열(array)</li>
  <li>객체(Object)</li>
  <li>null</li>
</ul>

<h2>JSON 직렬화, 역직렬화</h2>
<ul>
  <li>직렬화</li>
    <ul><li>직렬화는 외부의 시스템에서 사용할 수 있도록 바이트(byte)형태로 변환하는 기술이다.</li></ul>
  <li>역직렬화</li>
    <ul><li>역직렬화는 직렬화의 반대를 의미한다.</li></ul>
</ul>
문자열 ==> 객체 -JSON.parse() 역직렬화<br>
객체 ==> 문자열 -JSON.stringify() 직렬화

<h2>JSON의 활용</h2>
JSON은 프로그래밍 언어와 프레임워크 등에 독립적이므로, 서로 다른 시스템간에 데이터를 교환하기에 좋다.<br>
주로 API의 반환형태, 시스템을 구성하는 설정파일에 활용된다.<br>
  <blockquote>요즘에는 API에 XML보다 주로 JSON이 더 많이 쓰이고 설정파일에 XML이 쓰인다..</blockquote>
 


