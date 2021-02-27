## Beginner Usages for Go:
### Creating commands:
* Create main.go with a `func main() {}` to be run on call
* After calling `go build` your executable will have the same name as the parent folder.
* To put the executable output onto `$GOPATH` use `go install`, after which you will be able to call the executable from the commandline
### Creating packages:
* Create a Go file with the same name as your project folder
* Although not strictly necessary, your go file may contain functions; naming a function with a **Capital** will allow Go to export the function. Otherwise, your function will not be usable by anything.
* **Creating Tests** is very important for having a well documented and readable Go package. Common practice includes functionality for examples that serve as test code for your package.
### Combining Packages and Commands:
* Create a subdirectory `cmd`
* Create another subdirectory with your package name (to be called as a command this time)
* `go install ./cmd/gotut` To install your new command

* Go can be used for creating utilities that greatly increase your ability to create and code. In the example provided by rob, the project is a utility for

## Steps to Reproduce This Project on Windows:
1. Install [Go](https://golang.org/doc/install)
2. Initialize github project
`git clone git@github.com/patrick-yeadon/gotut`
3. Initialize mod.go with the url for the github project
`go mod init github.com/patrick-yeadon/gotut`

---
# Go Design Principles

* I'm going to need a [Redirect]()
* Allows multiple concurrent package development efforts without needing to pull from public repos. Useful when privately developing multiple packages at once.
* In a Go project, there is no concept of a `src` directory. In fact, there are no standardized specifications for how to make a Go package, other than having `go.mod` in your main directory.

---
