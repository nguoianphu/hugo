# Hugo Static Site Generator

## Build

    go get github.com/golang/crypto
    go get github.com/golang/net
    go get github.com/golang/text

    mkdir -p $GOPATH/src/golang.org/x
    mv $GOPATH/github.com/golang/crypto $GOPATH/src/golang.org/x/
    mv $GOPATH/github.com/golang/net $GOPATH/src/golang.org/x/
    mv $GOPATH/github.com/golang/text $GOPATH/src/golang.org/x/
    
    go get -v github.com/nguoianphu/hugo
    hugo version
    
## Create new site    
    
    cd /my/pages/source
    hugo new site bookshelf
    cd bookshelf
    hugo new post/good-to-great.md
    cd ..
    cd themes
    git clone https://github.com/digitalcraftsman/hugo-icarus-theme.git
    cd ..
    hugo server --theme=hugo-icarus-theme --buildDrafts
    hugo undraft content/post/good-to-great.md