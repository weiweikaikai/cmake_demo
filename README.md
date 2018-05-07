
#简单的cmake构建工程demo

cd build

cmake -DCMAKE_INSTALL_PREFIX= (要安装的目录绝对路径)  ..  
#如果直接cmake ..   不指定CMAKE_INSTALL_PREFIX系统默认安装到 /usr/local/bin  /usr/local/lib  /usr/local/share/doc

make 

make install


#目录中的 shared_lib   static_lib 是单独作为动态库构建和静态库构建的例子  这两个目录的CMakelist.txt 并没有加到主CMakelist.txt中   lib目录下可以同时生成 静态和动态库来替代
