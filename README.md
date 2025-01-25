# chatserver
工作在nginx tcp负载均衡环境中的集群聊天服务器和客户端源码 基于moduo实现 

编译方式
cd build
rm -rf *
cmake ..
make

需要nginx/redis等
下载指令：
（1）nginx
sudo apt-get install libpcre3 libpcre3-dev
sudo apt-get install zlib1g zlib1g-dev
sudo sudo apt-get install openssl
sudo apt-get install libssl-dev
sudo wget https://nginx.org/download/nginx-1.24.0.tar.gz
cd XXX
./configure --with-stream
make && make install
编译之后还需进入usr/local/nginx/conf,在root权限下修改nginx.conf配置文件

（2）redis
sudo apt-get install redis-server
