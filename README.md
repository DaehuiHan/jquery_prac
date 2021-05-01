# jQuary prac

- 미리 작성된 자바스크립트 코드
    document.getElementById("element").style.display = "none";
    이런 코드를
    $('#element').hide();이렇게 간단하게 쓸 수 있음

- FIXME: import를 꼭 해야 쓸 수 있다.
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    이걸 import하면 된다.

- html태그에 id를 주고 지정을 해줘서 사용한다.
    id로 지정한 것에 대해 가지고 올때는
    $('#[id이름]').함수; 
    이렇게 가지고 온다.

        - input 박스 value 가지고 오기
            $('#[id]).val();
        -input 박스 value 바꾸기
            $('#[id]).val('내용'); 이렇게 하면 해당 내용으로 바뀐다.

        - div 숨기고 나타내기
            $('#[id]').show();
            $('#[id]').hide();
            이걸 버튼을 만들어서 숨기고 나타내고 할 수도 있다.

        - css 속성 가지고 오기
            $('#[id]').css('[css 항목]');
        - css 속성을 바꿀수도 있다.
            예시, $('#[id]').css('width', '700px');
            이렇게 하면 width가 700px로 바뀐다.

        - text 가지고 오기
            $('#[id]').text();
            * val과 마찬가지로 변경도 가능하다.

        - 백틱을 사용하여 html 변수를 만들어 준뒤 붙여줄 수 있다.
            let temp_html = `<button>나는 버튼이다. </button>`
            $('#cards-box').append(temp_html);

- 백틱 문법으로
    let title = '나는 제목이다.'
    이렇게 하고
    let temp_html = `
    <div>
        <h1>${title}</h1>
    </div>
    `
    이렇게 해서 원하는 곳에 붙일 수 있다.

- 본문에 FIXME로 표시한 곳에 jQuary이용한 함수 사용
