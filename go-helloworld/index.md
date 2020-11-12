# Go Hello World


## 영상

{{<youtube p4cVTw_f3-k>}}



main.go 를 만들었다. 

{{< admonition type=tip title="중요" open=true >}}

go 프로젝트를 컴파일 하고 싶다면 파일 이름을 main.go 로 해야한다. example.go 같은 경우에는 컴파일이 되지 않는다. 

{{</admonition>}}



main.go 의 맨 윗줄에 ```package main``` 이라고 작성한다. Go 에서는 어떤 패키지를 사용하는지 알려주어야 한다. 또 Node.js 나 Python 과 달리 특정한 function 을 찾는다. 



```go
package main

func main() {

}
```



## Hello World

Hello World 를 프린트해보자.

function 안에 ```fmt.Println('Hello World!')```를 쓴 뒤 package 뒤에 

import "fmt" 를 쓴다. fmt 가 뭔지는 다음에.

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello World!")
}
```

```go run main.go``` 로 작동시켜보면

```powershell
PS C:\Go\PJCT> go run main.go
Hello World!
```

잘 작동한다!
