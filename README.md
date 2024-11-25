### Go.sublime-build

Windows
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
