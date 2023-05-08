# 使用snap安装coq
https://snapcraft.io/coq-prover
# 编译
## step1
创建_CoqProject文件
```shell
touch _CoqProject && echo "-Q . LF" > _CoqProject
```
## step2
生成makefile
```shell
coq_makefile -f _CoqProject *.v -o Makefile
```
## step3
make编译所有文件
```shell
make
```
