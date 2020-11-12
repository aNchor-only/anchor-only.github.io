# Go Packages and Imports


## 영상

{{<youtube 1xe2UIZ3gx0>}}



## 패키지

main.go 에서 Hello World 를 출력할 때 ```fmt.Println``` 으로 출력했었다. fmt 는 format 을 위한 패키지다. 그런데 왜 Println 은 첫글자가 대문자일까?

## Import

파이썬, 자바, 자바스크립트 등에서는 무언가를 import 할때 맨 위에 

```import 000 from 000``` 형식으로 import 해온다. 또 node.js 나 자바스크립트 같은것에서는 모듈을 export 해야한다. 

<br>

Go 에서는, function을 export 해주고 싶다면, function 을 대문자로 시작하면 된다. 

또 import 받는 쪽에서도 첫글자가 대문자로 인식된다.



그러니까 첫글자가 대문자인 function 들은 다른곳에서 import 된거라고 보면 된다.
