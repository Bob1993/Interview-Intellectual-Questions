# Interview-Intellectual-Questions

程序员面试那些有趣的智力题

#### 给你一个3升的桶和一个5升的桶,如何称出4升水来?

> 由于不知道两个桶底面积是否相同,也不能估计倒一半,精确版解答如下：
> 
> 1. 满3升水倒入空5升桶中,再满3升水倒入5升桶中至倒满,这样3升桶中刚好剩1升水.
> 2. 将5升桶的水全倒出,再将3升桶中的1升水倒入5升空桶,这样5升空桶有1升水.
> 3. 最后把3升桶装满,再倒入5升桶,5升桶就有4升水了.

#### 有25匹马，速度都不同，但每匹马的速度都是定值。现在只有5条赛道，无法计时，即每赛一场最多只能知道5匹马的相对快慢。问最少赛几场可以找出25匹马中速度最快的前3名？

> 每匹马都至少要有一次参赛的机会，所以25匹马分成5组，一开始的这5场比赛是免不了的。接下来要找冠军也很容易，每一组的冠军在一起赛一场就行了（第6场）。最后就是要找第2和第3名。我们按照第6场比赛中得到的名次依次把它们在前5场比赛中所在的组命名为A、B、C、D、E。即：A组的冠军是第6场的第1名，B组的冠军是第6场的第2名……每一组的5匹马按照他们已经赛出的成绩从快到慢编号：

> * A组：1，2，3，4，5
* B组：1，2，3，4，5
* C组：1，2，3，4，5
* D组：1，2，3，4，5
* E组：1，2，3，4，5

> 从现在所得到的信息，我们可以知道哪些马已经被排除在3名以外。只要已经能确定有3匹或3匹以上的马比这匹马快，那么它就已经被淘汰了。可以看到，只有上表中粗体蓝色的那5匹马才有可能为2、3名的。即：A组的2、3名；B组的1、2名，C组的第1名。取这5匹马进行第7场比赛，第7场比赛的前两名就是25匹马中的2、3名。故一共最少要赛7场。