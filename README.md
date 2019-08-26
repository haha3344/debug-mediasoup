
### 环境
- ubuntu 18.04
- CLion
- mediasoup 3.2.5
- mediasoup-demo (v3 commit 74aea5f)


### 方法
- 需要手动编译安装`mediasoup/worker/deps/`下的`usrsctp`,`libsrtp`,`openssl`,`libuv`
- 将`CMakeLists.txt`放入`mediasoup/worker/`下，用`Clion`新建工程并编译
- 将生成的可执行文件`mediasoup-worker`覆盖`mediasoup-demo/server/node_modules/mediasoup/worker/out/Release/`中的原文件
- 在`CLion`中使用`Run->Attach to Process...`, 选择`mediasoup-worker`进程