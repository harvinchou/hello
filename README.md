# Hello Go

Create a package directory for Hello program.

```bash
$ mkdir $GOPATH/src/github.com/<username>/hello
```

Create a file in the *hello* directory named `hello.go` and add the following code to it:

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, world.")
}
```

Build and install Hello program:

```bash
$ cd $GOPATH/src/github.com/<username>/hello
$ go install
```

Run Hello program:

```bash
$ $GOPATH/bin/hello
Hello, world.
```

Create an empty repository, add the files, commit changes, and then push to a remote repository.

```bash
$ git init
$ git add hello.go
$ git commit -m "initial commit"
$ git status
$ git remote add origin https://github.com/<username>/hello.git
$ git pull --rebase origin master
$ git push -u origin master
```  
