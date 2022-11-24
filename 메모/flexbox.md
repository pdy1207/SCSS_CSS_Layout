### flexbox / inline-box

 - `inline` : 같은 직선에 있다, 글이다 즉 너비와 높이를 못씀.
 - `flexbox` : box의 위치를 바꾸고 싶을때 box가 아닌 box의 바로 위 부모(parent)의 속성을 조절해야함.
 - `flex-direction`  
 1. row (행) 기본값 === 가로 
 2. column (열) 세로 3. reverse (반대로~!)

flex-flow === flex-direction / flex- wrap 
ex)) flex-flow: align-items: 

### 잊지말자!!! 

 `justify-content == main axis`
`align-items == cross acxis`

>display: flex 기준으로서,
flex-direction의 defult 값은 row(가로) 화면으로서 생각을해보자 div 아닙니다. <br>
row 방향일때 : main axis = 가로(justify-content) / Cross axis = 세로(align-items) <br>
column방향일때: main axis = 세로(justify-content) / Cross axis = 가로(align-items) <br>
