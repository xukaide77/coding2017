##CPU，内存，硬盘，指令以及它们之间的关系(2017.03.12)

>对这块也说不太深，大体写点吧

### CPU

CPU，就是中央处理器（Central Processing Unit），就是一大块集成电路 :)

这里面呢，有这么几个重要的东西：ALU、寄存器、时钟。

ALU：就是算数逻辑单元，我的理解，功能上就是把几个基本的逻辑计算、数学计算以电路形式实现出来。比如加法啊、与或非门啊、位移啊什么的。

寄存器：听名字，就是存储用的，保存要干的任务、给ALU提供输入、保存ALU的输出。

时钟：这个。。。，就是一个计时器。为啥需要这个计时器呢（按照上面讲的，运算已经都够完成了）？可以理解为乐队的指挥、龙舟上的鼓手，作用就是产生一个频率信号，用来指挥上面那俩按照一个节奏有序的工作。为了快速的完成任务，这个频率需要非常快，有多快呢？目前3.5GHz已经很常见了，也就是说1s运算350,000,000次。

### 内存

内存呢，也是用来存储数据的。前面说了，CPU里面已经有了寄存器这么个用来存储的东西，为啥还要个内存呢？主要原因就是寄存器又小又贵，小到不能存储所有的内容（基本上存不了什么），贵到不好任性的扩容（要满足CPU那么快的速度还是有难度的）。有人就想出了另一种方案，把不那么常用的数据呢，放在不那么快，但是更大的存储原件里面，也就是内存。平常存储点堆栈啊、缓冲什么的。这样，寄存器只要保存数据在内存中的位置，用的时候去内存取出来就好了。内存还可以分为RAM与ROM，不再细说。

### 硬盘

要硬盘，是因为内存也不够用了。。。当然，硬盘比内存还要慢，一般也会比内存大。用的时候，先从硬盘读出来放到内存就好了。

### 指令

指令，就是给CPU用的Java（当然写起来远没有Java方便），用来告诉CPU要干什么。