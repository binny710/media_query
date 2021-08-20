# media_query
css 반응형 속성
<style>...</style>
    @media(min-width:800px(조건)) {
        div {
            display:none;(반응)
            }
    }
- 웹 창의 너비가 800px보다 크면, 보이지 않게 하는 반응
- 조건에서 너비가 800px보다 크다면, 반응하는 경우의 '최소 너비가 800px'일 때라고 생각할 수 있어야 한다.

# media_query02
<style>...</style>
    @media(max-width: 800px){
        #grid {
            display: block;
        }
        #grid ol {
            border-right: none;
        }
        h1 {
            border-bottom: none;
        }
    }
- 웹 창이 800px보다 작으면, 선을 다 없애고 그리드를 없애 좌우로 된 내용을 상하로 바꾸는 반응
- 조건에서 너비가 800px보다 작다면, 반응하는 경우의 '최대 너비가 800px'일 때 = max width
- 오른쪽 내용이 보기 힘들게 잘리는 경우를 대비한 반응으로, 오른쪽 내용과 왼쪽 내용을 구분하여 줄바꿈을 하게 하는 것
- #grid의 display를 block으로 바꾸면 한 줄이 화면 전체를 쓰게 되어 자동적으로 줄바꿈이 되어 오른쪽 내용이 밑으로 내려갈 수 있다.
