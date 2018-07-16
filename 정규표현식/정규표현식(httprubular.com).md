### 정규표현식(http://rubular.com/)

<https://medium.com/@originerd/%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D-%EC%A2%80-%EB%8D%94-%EA%B9%8A%EC%9D%B4-%EC%95%8C%EC%95%84%EB%B3%B4%EA%B8%B0-5bd16027e1e0>



## 정규표현식

1. 단순패턴 사용하기

   ```ruby
   /app/
   # This app is made by apple!
   ```

   This **app** is made by **app**le!

2. 문자열 사용하기

   3. `^` : 문장 가장 앞을 뜻함.

      `/^apple/` 

      - pineapple => X
      - apple => `apple`

   4. `$` : 문장 가장 끝을 뜻함.
      `/apple$/` 

      * pineapple => pine`apple`
      * apple => `apple`

   5. `[abc]`: a or b or c

      `[^abc]`: !(a|b|c)
      `[a-z]` : a~z
      `[a-zA-Z]`: a~z A~Z 

   6. `?` : 0번 혹은 1번, `{0,1}`
      `/bo?/`: `b`am`bo`o 

      `*` : 0번 이상, `{0,}` 같음
      `/bo*/`: `b`am`bo`o
      `+` : 1번 이상, `{1,}` 같다.
      `/bo+/` : `b` am `bo`o
      `a{3,}` : a가 3번이상
      `a{1,4}`: a가 1~4번
      `a{2}` : a가 2번

   7. `.` : 개행문자를 제외한 모든 문자
      `a.e`: `ate`, apple
      `a.+e`: `ate`, `apple`

   8. `\s` : white space
      `\S` : !white space
      `\d` : number
      `\D` : !number
      `\w` : [a-zA-Z0-9_]
      `\W` : [ ^a-zA-Z0-9_]

   9. `|` or case

## 정규표현식 심화

1. Group `()`

   Q. html 코드 중에서 문법에 맞는 것 찾기.

   ```html
   <h1>hihi</h1>
   <h2>title</h2>
   <h3>hihi</h4>
   <h9>hihi</h9>
   ```

   `<h[1-6]>[a-z]+<\/h[1-6]>`

   => 이 경우에는 `<h3>hihi</h4>` 도 찾음.

   `<(h[1-6])>[a-z]+<\/\1>` 이렇게하면, 앞의 그룹을 참조하여 정확히 열고 닫았을 때만 찾게 됨.

2. Greedy 
   `internationalization` 
   `i\w+n` => `internationalization`
   `i\w+?n` => `intern` at`ion`al`ization`

3. 전방탐색/후방탐색
   `(?=__)`: __에 조건식을 넣으면, 전방탐색
   `(?<=__)`: __에 조건식을 넣으면, 후방탐색

   ```
   
   ```

   `\d+(?=원)` => `1000` `2000`

4. 부정형 전방탐색/후방탐색
   `(?!__)` : 조건이 일치하지 않는 전방탐색

   `(?<!__)` : 조건이 일치하지 않는 후방탐색