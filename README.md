# JavaUnsafeTree
Java中的Unsafe技术研究


<pre>
Unsafe位于sun.misc包内，看其命名就知道与注重安全性的jdk无缘。
Unsafe的特点是可以直接操作堆外内存，可以随意查看及修改JVM中运行的数据结构。
      可以用来在任意地址位置处读写数据，支持一些CAS原子操作。
Unsafe可以查看和修改对象的成员，Unsafe的操作粒度不是类，而是数据和地址。

Java最初被设计为一种安全的受控环境。尽管如此，HotSpot还是包含了一个后门sun,misc.Unsafe，
提供了一些可以直接操控内存和线程的底层操作。

Unsafe被JDK广泛引用与java.nio和并发包等实现中，这个不安全的类提供了一个观察HotSpot Jvm
内部结构并且对其进行修改。
</pre>