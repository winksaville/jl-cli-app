# Create a julia script that executes from command line

This is trivial create a legal executable and add
the shebang header:

```
wink@3900x:~/prgs/julia/projects/cli-app
$ cat cli-app 
#!/usr/bin/env julia
println(PROGRAM_FILE)
for x in ARGS
	println(x)
end
```

Change the mode to executable something like
`chmod a+x cli-app` and then execute it:
```
wink@3900x:~/prgs/julia/projects/cli-app
$ ./cli-app first-param second-param
./cli-app
first-param
second-param
```
