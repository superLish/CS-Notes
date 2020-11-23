### 异步
异步的核心思想，可以这么去理解。异步可以抽象为一个一个子任务，等待调度器去调度执行，或者是一段供将来调度的代码。执行这个子任务有两种结果，一种是就绪，直接执行，返回结果。还有一种是未就绪，这时候如果是同步调用的话，一般的处理是等待，直到就绪再执行，而异步的话，如果是未就绪，就挂起这个子任务，等待就绪后再唤醒这个子任务去调度执行。所以，这里的一个关键就是怎么去唤醒这个子任务。

[The Future Trait](https://rust-lang.github.io/async-book/02_execution/02_future.html)
