# 1.语法相关
* [各种COUNT()的区别](https://zhuanlan.zhihu.com/p/89299468)
  * COUNT(主键)最快
  * 没有主键: `COUNT(1) > COUNT(*)`
  * 有主键, 多个列: `COUNT(*) > COUNT(1)`
  * 只有一列: `COUNT(*) > COUNT(1)`
* 各种`join`的区别
  * `left`
  * `right`
  * `inner`
  * `outer`其结果集中不仅包含符合连接条件的行，而且还会包括左表、右表或两个表中的所有数据行，这三种情况依次称之为左外连接，右外连接，和全外连接。
# 2.偏底层相关

* MySQL执行顺序????
* [数据倾斜: 为什么hive select count distinct 查询的reduce一直卡在99%,这可能是什么原因导致的，你有什么解决方法"。](https://blog.csdn.net/Dreamy_zsy/article/details/112676320)
  * MapReduce计算框架:
  * 数据倾斜: MapReduce计算框架中经常发生。大量相同的key被分配到了同一个任务上，一个人累死、其他人闲死，这违背了分布式计算的初衷，使得整体的执行效率十分低下。

