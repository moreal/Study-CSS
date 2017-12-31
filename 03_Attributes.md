# Attributes

### color
  글씨의 색을 조정할 수 있는 속성이다.
  black, white, lightgray 등의 여러 색 영어표현을 사용가능하며  
  \#을 이용하여 rgb 색의 16진수 표현도 사용가능하다.  
  혹은 rgb 혹은 rgba 을 통해서 색을 지정해 줄 수도 있다.   
  rgba 는 alpha 값으로 투명도를 지정해 줄수 있다.

```css
  span {
    color: white;
  }

  p {
    color: #fff;
  }

  .test {
    color: rgb(255,255,255);
  }
```  

### background-color
  배경식의 색을 조정할 수 있는 속성이다.  
  color 와 같은 방식으로 색 설정이 가능하다.

```css
  span {
    background-color
  }
```

### text-align
문자의 정렬을 조정 가능한 속성이다.  
left, center, right가 가능하며 각각 좌측, 중앙, 우측 정렬이 된다.

```css
  span {
    text-align: center;
  }
```

### border
테두리 선에 대한 속성이다.  
border 를 이용해서 네모틀의 테투리를 만들기 등이 가능하다.  

##### Syntax
- border-width ex) 10px...
- border-style ex) solid, double, dotted..
- border-color ex) white, black..

```CSS
  div {
    border: 10px solid black;
  }

  .test {
    border-width: 10px;
    border-style: solid;
    border-color: black;
  }
```

### border-radius
테두리의 모서리를 둥글게 만들 수 있다.  
Syntax의 갯수에 따라 모서리에 적용되는 것이 달라진다.

##### Syntax
- four : 각각 왼쪽 위부터 시계방향으로 적용
- three : 왼쪽위, 오른쪽 모서리, 왼쪽 아래
- two : 왼쪽위와 오른쪽 아래, 오른쪽 위와 왼족 아래
- one : 모두 동일하게 적용

```css
  div {
    border-radius: 10px;
  }
```

### display
해당 구역에 대한 속성을 지정.

##### Exammple
- block (div form의 기본 포맷)
- inline-block (clear 가 left로 설정되어 있는 듯하다. inline에 width와 height plus)
- inline (css 기본 포맷)
- list-item (list 에서 사용되는 속성이다. li 등)  
  만약 li에 list-item 속성이 지정되어 있지 않다면 list-style과 관련된 속성이 적용되지 않는다.
- none  
  **레이아웃에 영향을 끼치지 않게 제외한다.**  
  visibility:hidden 의 경우에는 화면상 렌더링에서는 제외 되지만 존재는 하기에 레이아웃에 영향을 미친다.

### clear
다음 요소에 대한 정렬을 철할 수 있다.  
**float**로 설정했던 정렬을 컨트롤 하는데 유용할 것 같다.
