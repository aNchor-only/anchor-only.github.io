# Go Installation






## 영상

{{<youtube ic89gBxdHgs>}}



## Go 다운받기



[https://golang.org/](https://golang.org/)

로 접속한다.

<br>

리눅스라면 

```
sudo apt install go
sudo dnf install go
yay -S go
sudo pacman -S go
```

{{< admonition type=tip title="aur 주소" open=false >}}
https://www.archlinux.org/packages/community/x86_64/go/
{{< /admonition >}}



맥이나 윈도우는

 ![download](C:\hugo\content\posts\img\downloads.png))



여기서 클릭해서 다운

<br>

맥은

```
brew install golang
```

하면 될거고

<br>

윈도우는

```
choco install go
```

하면 될듯



## 환경변수 추가

맥

```
mkdir -p $HOME/go/{bin,src,pkg}
export GOPATH=$HOME/go
export GOROOT="$(brew --prefix golang)/libexec"
export PATH="$PATH:${GOPATH}/bin:${GOROOT}/bin"
```

https://medium.com/@jimkang/install-go-on-mac-with-homebrew-5fa421fc55f5



<br>

윈도우

![environmentvariable](C:\hugo\content\posts\img\windowsenvironmentsvariable.png)

![variables](C:\hugo\content\posts\img\variables.png)

![gopath](C:\hugo\content\posts\img\gopath.png)

Path 에 Go 를 설치한 폴더가 들어있으면 된다.



{{<admonition>}}

Go 는 Go 의 Path 가 설치된 곳에서만 작동한다. 원하는 곳에 폴더를 만들어서 작업할 수 없다는 소리다. 자동적으로 생성되는 Go Path 디렉토리는 C:\Go 지만 환경변수를 수정해 D 드라이브로 바꿨다. 그래서 C:\Go 안의 특정 폴더 안에서 작업을 해야 한다.

{{</admonition>}}



Go 는 Node.js 나 Python 같이 모듈이나 패키지를 다운받을 수 있는곳이 제한적이다. npm 이나 pypi 등등. Go 는 그런거 없다. 그렇기 때문에 코드를 다운받을, 업로드 할 도메인으로 깔끔하게 정리한다.

<br>



src 안에 자신의 깃허브 주소로 디렉터리를 만들고 프로젝트 이름으로 디렉터리를 만든다. 그리고 그 안에 main.go 를 생성하고 vscode 로 열면 install 같은게 많이 나올텐데 모두 하면 된다. 
