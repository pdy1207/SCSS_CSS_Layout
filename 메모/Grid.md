## Grid

CSS 그리드 레이아웃은 웹페이지를 위한 이차원 레이아웃 시스템입니다. <br>
이 기능을 통해 콘텐츠를 행과 열에 배치할 수 있으며 복잡한 레이아웃을 직접 직관적으로 구축할 수 있는 많은 기능이 있습니다. <br>
[링크](https://developer.mozilla.org/ko/docs/Learn/CSS/CSS_layout/Grids)

### 그리드 레이아웃이란? 
그리드는 수평선과 수직선으로 이루어진 집합체로, 디자인 요소를 정렬할 수 있는 대상 패턴을 생성한다.  <br>
이 디자인은 페이지에서 페이지로 이동할 때 요소가 널뛰거나 너비가 바뀌지 않는 디자인 생성에 도움을 주어 웹 사이트의 일관성을 높여준다. <br>
[링크](https://developer.mozilla.org/ko/docs/Learn/CSS/CSS_layout/Grids#what_is_grid_layout)


flexbox에서 좌우배치, 중앙배치는 쉽지만 grid형태를 만드는게 어려움 <br>
=> grid를 배우는 이유 <br>

● column-gap: (column 사이 공간 크기); <br>
● row-gap: (row 사이 공간 크기); <br>
● gap: 10px; ▷ column과 row 사이에 10px의 공간을 줘라. <br>
● grid-template-rows: (각 row의 크기와 개수); <br>


● grid-column: (start) / (end); <br>
● grid-row: (start) / (end); <br>

● -1, -2, -3, ··· ▷ 끝에서부터 line 세기 <br>
● (start) / span (cell 수) ▷ 시작점과 끝점을 적는걸 대신한다. <br>


<hr> 

### `fr?`
  
  fr ?? fraction(부분) <br>
  fraction은 grid에서 사용 가능한 공간 fr값 비율로 공간을 나눈다. 
  
  `grid-template` 
  "이름" (row크기) <br>
  "이름" (row크기) / (각 coumn의 크기) <br>
  
#### `grid-template은 이 모든것을 정의하는 바로 가기임.` 

      grid-template-areas
      grid-template-columns
      grid-template-rows
  
  grid-template-columns: repeat(4, 1fr); 4번 똑같이 나누자~! 뜻
  
  
  
  
  
  
