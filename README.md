# Js 이용해 html에서의 input 값 console에 출력하기

## html 에서 js 파일 linking 하는 방법?
> ```<script>``` 태그 사용   
```
<script type="text/javascript" src="./Resource/js/login.js"></script>
```

## 'onclick' Event 사용
> id가 "output" 으로 지정된 버튼 클릭 시, js의 out() 함수를 실행시키기 위해    
```
dconst output = document.getElementById("output");
output.onclick = function out() {
```

## onclick과 addEventListener 차이?
> ```onclick``` 이벤트 핸들러를 두 번 이상 사용한다면, 기존 이벤트 핸들러를 덮어쓰기 때문에 가장 아래에 추가한 핸들러만 제대로 작동함 <br> 
반면, ```addEventListener```는 기존 이벤트 핸들러를 덮어 쓰지 않고 얼마든지 계속해서 핸들러를 추가해도 모든 핸들러가 정상적으로 작동함 <br>
**addEventListener는 IE8 이하에서는 작동을 하지 않는다.** <br>
**그래서 구형 브라우저 지원이 필요하면 onclick을 사용하는 것임**  


## document.getElementById("id").value?
> 주어진 문자열과 일치하는 id 속성을 가진 요소를 찾고, 이를 나타내는 Element 객체의 value 값을 반환함   

## console.log()?
> Web Console 창에 메시지를 출력함 <br>
() 안에 console 창에 출력하고 싶은 내용을 적음 <br>   
윈도우 기준, ```ctrl + shift + j``` 또는 ```F12``` 으로 확인 가능     

#### 출력 결과
```
id : 다미 login.js:6
pw : 123 login.js:7
```

---
# Problem 과 Solution   

## Console 창에 결과가 잘 나오지 않을 때?
> ```.addEventListener("click", myScript)``` 으로도 시도해 보시길!

---

### git add 취소?
``` 
git reset HEAD <file>
```

### git commit 취소?
```
git reset --soft HEAD
```

### git commit message 변경?
```
git commit --amend
```

### git push 취소?
```
git reset HEAD
// 가장 최근의 commit을 취소
```


