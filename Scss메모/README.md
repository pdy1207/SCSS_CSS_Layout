
<p align="center">
  <img src="https://heropy.blog/css/images/vendor_icons/sass.png" height="150" width="300">
</p>

## SCSS:

- [x] Variables
- [x] Nesting
- [x] Mixins
- [x] Extend
- [x] Responsive Mixins

### Scss ? `Syntactically Awesome Style Sheets, Sass`
  
    CSS 내 반복되는 내용은 줄이고 보다 효율적으로 스타일시트를 관리해야하므로, 문법적으로 어썸한 스타일 시트 
    
 - css & Scss 와 다르다
 - Scss는 css로 작업할 때 표준이 되었다.
 - Scss == Sassy css를 의미한다고 말할 수 있다.

<hr>

### `Variables`

SCSS 파일을 만들때 _을 넣는건 css로 변환되지 않길 원하는 것들을 저장함 <br>
ㄴ $을 붙여서 사용 <br>
ㄴ $bg: #e7473c;

- color
- style
- shadow
- font-size , family....  
  
### `Nesting(둥지)`

부모 내 자식 요소들의 CSS를 굳이 class를 주지 않아도 된다. <br>
ㄴ매우 큰 장점이라고 생각함<br>
      a {
        margin-bottom: 10px;
        &:nth-child(odd) {
          @include link("odd");
        }
        &:nth-child(even) {
          @include link("even");
        }
      }

    그런 active, hover 같은 활동적인 CSS를 넣어주고 싶다!?
    ㄴ& 넣기


### `mixins`

 - mixins => 여러가지 css 효과를 넣어서 다른 element에 적용시켜 줄 수 있음 재활용이 가능하다는게 큰 장점 

사용방법 
@import 해온 다음 쓸려는 element에  <br>
@include mixin이름 <br>
SCSS mixin에선 @if @else문도 사용 가능 <br>
(SCSS에서는 @을 붙여줘야 한다)

<hr>

### `extend`
extend를 사용할 수 있는 scss 는 '%' 사용 <br>

css파일을 한눈에 알아보기 쉽게 하기 위해 <br>
1. 관련 없는 태그들의 속성 지정은 mixins 사용이 좋은것 같습니다.
2. 연관된 태그들의 속성 지정은 extend를 사용하시면 될 것 같습니다.

#### `@mixins`: css 스타일을 함수처럼 만들 수 있음. <br> 
예시) @mixins function($param) <br>

#### `@include` : @mixin 함수 에 variable(argument) 를 전달 함으로써 재활용 가능하게 해줌. <br>
예시) @include function(argument) <br>

#### `@content`: css 스타일을 다른 css 스타일에 추가 가능하게 해줌. <br>
- @include로 호출해서 { .... } 내에 추가적인 스타일 코드 입력 하면 content 에 더해짐.  <br>

예시)

        @include function("iPhone") {
        color: blue;
        }

        @mixin function($device) {
        font-size: 28px;
        @if $device == "iPhone"
        @content; // color: blue;

<hr> 

> 이러한 것을 정리한 깃허브로서 Bourbon , Sass MediaQueries , Animate.css `@include` 하면됨!! 

#### 내가 정말 좋아하는 라이브러리 찾기! 

