
##Lab4 Deadlock Analysis

* 1.试跑了两次，一次停在了228，一次停在了78
![first](https://github.com/ChenWenchen/ES2016_14353033/blob/master/image/deadlock_1.png)
![first](https://github.com/ChenWenchen/ES2016_14353033/blob/master/image/deadlock_2.bmp)

* 2.死锁产生的四个条件：
  * 资源互斥：一个资源在同一时间只能被一个进程使用。
  * 占有且等待：一个进程在请求资源时，自己同时占有自己的资源不释放。
  * 非抢占：不存在抢占的机制使得资源被抢夺。
  * 循环等待：进程之间存在着头尾相连的资源等待关系。


* 3.在上述的java程序中，A类中的方法methodA使用了一个b的资源（要请求使用b这个资源）同时b这个资源中的方法又请求使用同一个a的资源，这就造成了互相请求的循环等待队列，而且满足死锁产生的条件，如果此时刚好卡在a这个进程不在running中而b进行请求的动作，就可能发生死锁。
