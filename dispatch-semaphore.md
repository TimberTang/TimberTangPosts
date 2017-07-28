---

title: Dispatch Semaphore
date: 2017-05-10 11:05:48
tags:

---

### 使用Dispatch Semaphore

dispatch_semaphore_t 类似信号量,可以用来控制访问某一资源访问数量。
使用过程：

1.先创建一个Dispatch Semaphore对象，用整数值表示资源的可用数量

2.在每个任务中，调用dispatch_semaphore_wait来等待
获得资源就可以进行操作
3.操作完后调用dispatch_semaphore_signal来释放资源

