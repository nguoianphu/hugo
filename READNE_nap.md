

    go get github.com/golang/crypto
    go get github.com/golang/net
    go get github.com/golang/text

    mkdir -p $GOPATH/src/golang.org/x
    mv $GOPATH/github.com/golang/crypto $GOPATH/src/golang.org/x/
    mv $GOPATH/github.com/golang/net $GOPATH/src/golang.org/x/
    mv $GOPATH/github.com/golang/text $GOPATH/src/golang.org/x/
    
    go get -v github.com/nguoianphu/hugo
    hugo version
    