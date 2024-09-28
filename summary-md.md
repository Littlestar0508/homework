# MD파일 본격 정리!

## 제목(h1~h6)

1.  HTML에서 사용되는 h태그는 md 파일에선 #의 개수로 구분
2.  ex) # [contents] or #### [contents]
3.  최대 6개(h6)까지 지원<br>

출력 예제

> # h1
>
> ## h2
>
> ### h3
>
> #### h4
>
> ##### h5
>
> ###### h6

---

## 인용

1.  문장을 가져오고 싶을때 사용
2.  ex) > Quote
3.  인용 안에 또 다른 인용이 가능합니다<br>

출력 예제

> Quote1
>
> > Quote2
> >
> > > Quote3

---

## 순서O 리스트

1. 문장들에 순서를 부여하고 싶을때 사용
2. ex) 1. con1 \n 2. con2 \n 3. con3
3. 숫자를 아무거나 쓰고 다음 줄로 넘겨도 출력은 여전히 이어서 됩니다<br/>
   ex)1 2 3 -> 1 2 3 / 1 1 1 -> 1 2 3

출력 예제

> 1. con1
> 2. con2
> 3. con3

---

## 순서X 리스트

1. \* , + , - 기호를 사용하여 나타내기
2. ex) \* con1 / + con2<br>

출력 예제

> - con1(\*사용)
>
> * con2(+사용)
>
> - con3(-사용)

## 글씨체

1. 글씨체를 italic,bold 등과 같은 꼴로 변경
2. ex) \*Italic\*
3. 문장 중간에 특정 부분만 사용 가능

출력 예제

> _Italic_(\*content\*)<br>
>
> _Italic_(\_content\_)<br>
>
> **Bold**(\*\*content\*\*)<br>
>
> **Bold**(\_\_content\_\_)<br>
>
> **Bold & _Italic_**(\*\*\_content\_\*\*)<br>
>
> <u>underline</u>(\<u>content\</u>)<br>
>
> ~~LineThrough~~(\~~content\~~)<br> > <br>

<hr>

## 링크

1. 외부 사이트의 링크로 연결 시키기
2. ex) [GOOGLE](https://google.com)
3. [] 안에는 나타낼 글자 () 안에는 해당 주소를 입력
   <br/>

출력 예제

> 1. [GOOGLE](https://www.google.com)
> 2. [NAVER](https://www.naver.com)
> 3. [GITHUB](https://github.com/Littlestar0508) > <br/>

<hr>

## 요약

1. 글이 너무 길거나 해당 내용을 초기에 숨기고 싶을때
2. summary와 details 태그를 사용

출력 예제

> <details>
>  <summary>생략됐습니다</summary>
>  이게 진짜 본문의 내용입니다.<br>
> 조금 더 길게 써보고 싶지만 내용이 생각나지 않아서<br>
> 3줄로만 글을 작성하겠습니다.
> </details>

<hr>

## 체크리스트

1. 할 일이나 했던 일을 표시하고 싶을 때
2. ex) - [ ] contents

출력 예제

> - [ ] 할 일(\- \[ \] 할 일)
> - [x] 한 일(\- \[X\] 한 일)

<hr>

## 이미지

1. 원하는 이미지를 md 문서에 삽입
2. ex) \!\[제목](경로)
3. 해당 파일이 디렉토리 경로에 존재 해야 한다(크기 조절 불가능)
4. img 태그를 사용해서도 나타낼 수 있다(크기 조절 가능)

출력 예제

> ![photoJ1](./assets/md/jphoto1.jpg) <br>
>
> <img src="./assets/md/jphoto4.jpg" width="400px" alt="photoJ2"/>

<hr>

## 코드 생성

1. 원하는 코드를 넣고 싶을때 사용
2. ex) \`\`\` code \`\`\`

출력 예제

> `import java.util.* `<br> > `public class Main { `<br> > `&ensp;public class void main(String[] args) { `<br> > `&ensp;&ensp;System.out.println("Hello World!!"); `<br> > `&ensp;&ensp;} `<br> > `&ensp;} `<br>
