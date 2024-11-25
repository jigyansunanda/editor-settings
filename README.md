### Go.sublime-build

Windows

    - Check `go version` first. If Go is installed, output should be something like `go version go1.23.3 windows/386`.
    
    - Check `GOPATH` by running `echo $env:GOPATH`. Output should be something like `C:\Users\nanda\go`.
    
    - Check `env:PATH` by running `echo $env:PATH`. Output should contain `C:\Program Files (x86)\Go\bin` or `C:\Users\nanda\go\bin`. This means your PATH environment variable includes the Go binary directory and Go should be accessible from the command line. 

```
{
    "shell_cmd": "go run \"${file}\" < input.txt > output.txt 2>&1",
    "selector": "source.go"
}
```

Mac
```
{
    "shell_cmd": "PATH=$PATH:/usr/local/go/bin go run ${file} < input.txt > output.txt 2>&1",
    "selector": "source.go"
}
```
