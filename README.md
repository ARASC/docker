# docker


## deepctr docker镜像使用方法
1. 在工作目录下, 执行如下命令，初始化docker环境
```shell
$ docker run -it -d -v --name deepctr $PWD:/workspace/ docker.io/zqmath1994/deepctr_tf_1_14_0_with_py3:latest /bin/bash
```
2. 进入docker环境
```shell
$ docker exec -it deepctr /bin/bash
```
3. 在docker环境内,运行训练脚本
```shell
$ cd /workspace 
$ sh xxx.sh or python xxx.py
```

eg:
- 停止deepctr环境的运行: docker stop deepctr
- 启动deepctr环境的运行: docker start deepctr
- 删除deepctr环境的运行: docker rm deepctr
