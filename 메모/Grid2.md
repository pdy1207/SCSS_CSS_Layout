
# ※ GRID를 공부하려면 #2부터 그냥 다시 듣자....!!!


barkshihun21 year ago <br>
● justify-items <br>
● align-items <br> 
● place-items: (수직) (수평); <br>

<hr>

▷ stretch : grid를 늘려서 grid를 채우게 한다. <br>
▷ start : item을 cell 시작에 배치한다. <br>
▷ center : item을 cell 중앙에 배치한다. <br>
▷ end : item을 cell 끝에 배치한다. <br>

<hr>

- Justify-content : start; /*(그리드가 놓이는 위치를 뜻하며 기본은 start)*/ <br>
- Align-content는 수직적으로 그리드를 움직이는 것 <br> 
- Start, end, space-evenly, space-around, space-between 사용 <br>
- 컨테이너의 height가 그리드를 담을 만큼 충분해야한다.(높이 지정) <br>
- Grid-template에서 높이를 fr로 설정하고 align-content를 stretch로 설정하면 쭉 늘어난다. <br>
- Place items와 마찬가지로 place-content를 통해 수직 수평으로 그리드 이동가능(첫번째가 수직, 두번째 옵션이 수평) <br>
- Place-items는 셀안에서 항목이 이동하는 것이며, place-content는 그리드가 이동하는 것이다. <br>

<hr>

● align-self <br>
● justify-self <br>
● place-self: (수직 ) (수평); <br>
▷ child에만 적용돠는 property이다. <br>

● grid-auto-rows: (크기); <br>
▷ 만들어놓은 row보다 더 많은 content가 있으면, 자동으로 row를 만들어라. <br>

● grid-auto-flow: (방향); [기본값: row] <br>
▷ flex-direction과 비슷하다. <br>
▷ row가 끝날 때 새로운 row를 만들지, 새로운 column을 만들지 결정한다. <br>

● grid-auto-columns: (크기); <br>
▷ grid-auto-flow: column;일때 작동한다. <br>


● max-content <br>
▷ content의 크기만큼 cell의 크기를 늘린다. <br>
● min-content <br>
▷ content의 크기를 최대한 줄여 cell의 크기를 줄인다. <br>

※ 어떻게 content가 보여야 하는지 디자인하는 것이다. <br>
※ repeat(), minmax와 결합하여 반응형 디자인을 만들 수 있다.

