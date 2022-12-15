# [vlookup函数](https://www.bilibili.com/video/BV1EN411Z7UX/?spm_id_from=333.337.search-card.all.click)
* `VLOOKUP(lookup_value，table_array，col_index_num，[range_lookup])`
* `IFERROR(判断是否error,替换值)`
* 通配符`?`匹配一个字符`*`匹配任意长度
* 混合查找，`*1`自动变成数值型, `&""`自动变成文本型
* 替换`SUBSTITUTE(" ","")`空格替换成空
* 去除不可见字符`CLEAN()`
* 多列查找`COLUMN(), MATCH()`
* 一对多查找, 用`COUNTIF()`带辅助列123
  * `= C85&COUNTIF($C$85:C85,C85)`
* 多行合并查找,递归的思想`=C98&IFERROR("、"&VLOOKUP(B98,B99:D106,3,0),"")`
* `INDIRECT()`将地址激活
* `IF({1,0},列，列)`交换两列的顺序，原理就是又真又假，所以真假都输出