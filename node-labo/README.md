# node-labo
## install(mac)
* install nodebrew 
```
$brew install nodebrew
```

* setup nodebrew
```
$nodebrew setup
Fetching nodebrew...
Installed nodebrew in $HOME/.nodebrew

========================================
Export a path to nodebrew:

export PATH=$HOME/.nodebrew/current/bin:$PATH
========================================
```

* pathing
```
$echo "export PATH=$HOME/.nodebrew/current/bin:$PATH" >> ~/.bash_profile
$source ~/.bash_profile 
```

* show lineup
```
$nodebrew ls-remote
...
v9.6.1    v9.7.0    v9.7.1    v9.8.0    v9.9.0    v9.10.0   v9.10.1   v9.11.0
v9.11.1   

v10.0.0   v10.1.0   v10.2.0   v10.2.1   

io@v1.0.0 io@v1.0.1 io@v1.0.2 io@v1.0.3 io@v1.0.4 io@v1.1.0 io@v1.2.0 io@v1.3.0
io@v1.4.1 io@v1.4.2 io@v1.4.3 io@v1.5.0 io@v1.5.1 io@v1.6.0 io@v1.6.1 io@v1.6.2
io@v1.6.3 io@v1.6.4 io@v1.7.1 io@v1.8.1 io@v1.8.2 io@v1.8.3 io@v1.8.4 

io@v2.0.0 io@v2.0.1 io@v2.0.2 io@v2.1.0 io@v2.2.0 io@v2.2.1 io@v2.3.0 io@v2.3.1
io@v2.3.2 io@v2.3.3 io@v2.3.4 io@v2.4.0 io@v2.5.0 

io@v3.0.0 io@v3.1.0 io@v3.2.0 io@v3.3.0 io@v3.3.1 
```
* install latest
```
$nodebrew install-binary latest
Fetching: https://nodejs.org/dist/v10.4.1/node-v10.4.1-darwin-x64.tar.gz
######################################################################## 100.0%
Installed successfully
```

* confrim active node.js
```
$nodebrew ls
v10.2.1
v10.4.1

current: none
```
* active node.js
```
$nodebrew use v10.4.1
```
* confirm version of node.js
```
$node -v
v10.4.1
```

## hello world
```
(move workspace)
$echo "console.log('Hello World')" > helloworld.js
$node helloworld.js 
Hello World
```

## if you face following errors...
* do "nodebrew setup"
```
Fetching: https://nodejs.org/dist/v10.2.1/node-v10.2.1-darwin-x64.tar.gz
Warning: Failed to create the file 
Warning: /Users/aaaa/.nodebrew/src/v10.2.1/node-v10.2.1-darwin-x64.tar
Warning: .gz: No such file or directory
                                                                           0.0%
curl: (23) Failed writing body (0 != 1056)
download failed: https://nodejs.org/dist/v10.2.1/node-v10.2.1-darwin-x64.tar.gz
```

* do "pathing after nodebrew setup"
```
$node -v
-bash: node: command not found
```
