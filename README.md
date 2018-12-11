[![Build Status](https://travis-ci.org/lmmmmmm/JavaBase.svg?branch=master)](https://travis-ci.org/lmmmmmm/JavaBase)

>  ### 1.集合框架（collection模块） 
   * 链表       
   * 线性表.
   * map
   * 树
   * 图
   * 其他
   
>  ### 2.异常体系结构（exception模块)  
   * 定义一个异常
   * 常见异常
   * try、catch、finally

>  ### 3.Java多线程(thread模块)
   * 线程创建方式
      <table><tr><td bgcolor=#D1EEEE>
      
        + 继承Thread类  
          
        + 实现Runnable接口
        
        + 实现Callable接口，实现call方法，创建FutureTask对象，将Callable对象传递给FutureTask对象
            创建Thread对象，将FutureTask对象传给Thread对象。
            
        + 具体实现在模块下面basic包下。 
      </td></tr></table>
   * 线程的状态
   * 死锁: 当两个以上的线程，双发都在等到对方停止执行，以获得系统资源，但是没有一方提前退出时，称为死锁。
        <table><tr><td bgcolor=#D1EEEE>
         产生死锁的条件：  
         
       + 互斥条件：一个资源每次只能被一个线程使用。  
         
       + 请求与保持条件：一个线程因请求资源而阻塞时，对已获得的资源保持不释放。
       
       + 不剥夺条件：线程已获得资源，在未使用完之前，不能强行剥夺。
           
       + 循环等待条件：若干线程之间形成一种头尾相接的循环等待资源关系。
       
       + 死锁实例如deadlock包下DeadLock类所示。
           
        </td></tr></table>
        
     <table><tr><td bgcolor=#D1EEEE>
        解决死锁：打破死锁产生任意一个条件即可解决死锁问题。
 
        +  重启系统：代价较大。
        
        +  杀死线程，强迫释放资源。
        
        +  线程回退策略:让参与死锁的所有线程回退到没有发生死锁前某一点处，由此处继续执行，以求再次执行时不会发生死锁。  
     </td></tr></table>
     
   * 锁
   
   * 线程同步经典问题：生产者消费者问题、哲学家进餐问题、读写者问题。
   
>  ### 4.设计模式(design-mode模块)
   * 工厂模式： 只有一个工厂，根据传入的参数判断生成哪个对象。
   * 工厂方法： 四个关键因素
   
    1、 工厂接口：工厂方法模式核心。
    2、 工厂实现：决定如何实例化产品，需要多少产品，就有多少个工厂实现。
    3、 产品接口：定义产品规范。
    4、 产品实现：决定产品在客户端具体行为。
   * 抽象工厂模式：//TODO 
   * 建造者模式
   * 单例模式：懒汉式单例、恶汉式单例、双重if锁单例、静态内部类
   * 代理模式
    1、静态代理：代理类(ProxySubject)真实类(RealSubject)实现相同接口(Subject)，真实类实现具体方法，代理类拥有真实类实例，调用真实类方法实现代理。
    2、动态代理：//TODO
    3、Cglib代理：//TODO
   * 观察者模式：抽象观察者(Observer)，为具体观察者(ConcreteObserver)提供接口。抽象通知者(Subject)，提供增加、删除、通知观察者对象等接口，具体通知者(ConcreteObserver),实现抽象通知者接口.
>  ### 5.算法(algorithm模块)
   * 十大排序算法
   * 算法题：字符串类算法、链表类算法、栈类算法、树类算法
   
>  ### 6.第三方包(third-party-package模块)
   

>  ### 7.IO流(io-stream模块)


>  ### 8.注解(annotation模块)


>  ### 10.反射（reflect模块）
