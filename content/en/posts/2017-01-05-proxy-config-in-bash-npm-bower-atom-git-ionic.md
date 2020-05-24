+++
title = "Proxy config in Bash, NPM, Bower, Atom, Git & Ionic"
description = ""
tags = [
    "linux",
]
date = "2017-01-05"
categories = [
    "Linux",
]
menu = "main"
+++

Sometimes when you are building stuff behind huge networks like universities and
corporates, you often face proxy configuration issues with many applications
like NPM, Bower, Ionic, Git, Atom and Linux Bash itself. This article focuses on
resolving these issues.

### Linux Bash

##### With Authentication

```

export http_proxy='http://username:password@[Your Proxy]:[Proxy Port]/'    
export https_proxy='http://username:password@[Your Proxy]:[Proxy Port]/'
export ftp_proxy='http://username:password@[Your Proxy]:[Proxy Port]/'

```

##### Without Authentication

```

export http_proxy='http://[Your Proxy]:[Proxy Port]'    
export https_proxy='http://[Your Proxy]:[Proxy Port]'
export ftp_proxy='http://[Your Proxy]:[Proxy Port]'

```

##### View Proxy

```

env | grep -i proxy

```

##### Remove proxy

```

unset http_proxy
unset https_proxy
unset ftp_proxy
//these commands disable the proxy, temporarily for that particular bash session.

```


### NPM

##### With Authentication

```

npm config set proxy "http://username:password@[Your Proxy]:[Proxy Port]/"
npm config set https-proxy "http://username:password@[Your Proxy]:[Proxy Port]/"

```



##### Without Authentication

```

npm config set https-proxy http://[Your Proxy]:[Proxy Port]
npm config set proxy http://[Your Proxy]:[Proxy Port]

```


##### View Proxy

```

npm config get https-proxy
npm config get proxy

```


##### Remove proxy

```

npm config delete https-proxy
npm config delete proxy

//or

npm config set https-proxy null
npm config set proxy null

```


### Bower

##### With Authentication

```

//add the lines to `.bowerrc`
"proxy":"http://username:password@[Your Proxy]:[Proxy Port]/"
"https-proxy":"http://username:password@[Your Proxy]:[Proxy Port]/"

```


##### Without Authentication

```

// add the lines to `.bowerrc`
"proxy":"http://[Your Proxy]:[Proxy Port]"
"https-proxy":"http://[Your Proxy]:[Proxy Port]"

```


##### View Proxy

```

cat .bowerrc

```


##### Remove proxy

```

// edit and remove the lines from `.bowerrc` added earlier

```


### Atom

##### With Authentication

```

apm config set proxy "http://username:password@[Your Proxy]:[Proxy Port]/"
apm config set https-proxy "http://username:password@[Your Proxy]:[Proxy Port]/"

```



##### Without Authentication

```

apm config set https-proxy http://[Your Proxy]:[Proxy Port]
apm config set proxy http://[Your Proxy]:[Proxy Port]

```


##### View Proxy

```

apm config get https-proxy
apm config get proxy

```


##### Remove proxy

```

apm config delete https-proxy
apm config delete proxy

//or

apm config set https-proxy null
apm config set proxy null

```


### Git

##### With Authentication

```

git config --add http.proxy "http://username:password@[YourProxy]:[ProxyPort]/"
git config --add https.proxy "http://username:password@[YourProxy]:[ProxyPort]/"

```


##### Without Authentication

```

git config --add http.proxy http://[YourProxy]:[ProxyPort]
git config --add https.proxy http://[YourProxy]:[ProxyPort]

```


##### View Proxy

```

git config --get http.proxy
git config --get https.proxy

```


##### Remove proxy

```

git config --unset http.proxy
git config --unset https.proxy

```


### Ionic

##### With Authentication

```

//You can add proxy along with the a particular serve
PROXY="http://username:password@[YourProxy]:[ProxyPort]/" ionic start [your app]

```


##### Without Authentication

```

//You can add proxy along with the a particular serve
PROXY=http://[Your Proxy]:[Proxy Port] ionic start [your app]

```

*This post will be updated regularly with changes in configurations and new frameworks.*

*Comment below for any suggestions and framework/language requests.*

[Here](https://medium.com/@magician03/proxy-config-in-bash-npm-bower-atom-git-ionic-56b545b76a6d) is the Medium article for this post.