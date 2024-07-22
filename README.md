使用c++实现一个线程池，能够自定义限制线程数量，自动根据任务数量调整线程数。
改为map存放线程id与线程实例，vector存放已结束的线程id。在工作线程结束后，根据vector查找map，将已结束的线程实例销毁。

编译与运行方法： 

mkdir build

cd mkdir

cmake ..

make

./thread_pool
