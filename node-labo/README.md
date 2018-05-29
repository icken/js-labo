# node-labo
## install(mac)
* install nodebrew 
```
brew install nodebrew
```
* show lineup
```
nodebrew ls-remote
```
```
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
nodebrew install-binary latest
```
* but following error occurs!
```
Fetching: https://nodejs.org/dist/v10.2.1/node-v10.2.1-darwin-x64.tar.gz
Warning: Failed to create the file 
Warning: /Users/aaaa/.nodebrew/src/v10.2.1/node-v10.2.1-darwin-x64.tar
Warning: .gz: No such file or directory
                                                                           0.0%
curl: (23) Failed writing body (0 != 1056)
download failed: https://nodejs.org/dist/v10.2.1/node-v10.2.1-darwin-x64.tar.gz
```
* so mkdir
```
mkdir -p .nodebrew/src
```
* install latest again
```
nodebrew install-binary latest
```
* confrim active node.js
```
nodebrew ls
```
```
v10.2.1

current: none
```
* active node.js
```
nodebrew use v10.2.1
```
* confirm version of node.js
```
node -v
```
```
-bash: node: command not found
```
* wander for node command
```
ll .nodebrew/node/v10.2.1/bin/
```
* no idea to set path for it or get any wrong way(now).
