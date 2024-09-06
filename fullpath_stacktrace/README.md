## Full path

```
> go build
```

```
> ./main

Oh god.
The stacktrace....
Its coming!!!
panic: I'm here

goroutine 1 [running]:
main.main()
	/home/jesse/code/golang_reproductions/fullpath_stacktrace/trace.go:12 +0xdf
```


## Relative path
```
> go build -trimpath
```

```
> ./main 
Oh god.
The stacktrace....
Its coming!!!
panic: I'm here

goroutine 1 [running]:
main.main()
	main/trace.go:12 +0xdf
```
