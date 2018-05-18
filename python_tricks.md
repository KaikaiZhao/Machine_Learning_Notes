1. IPython,一种加强的交互式Python解释器
2. %run命令，IPython会在同一个进程中执行指定文件的代码，执行完之后，就可以通过交互的方式研究其结果了　e.g. `%run hellp_world.py`
3. 几乎所有的python对象都有一些附属函数（方法），他们可以访问该对象内部数据。函数可以接受位置参数，也可以接受关键字参数。
4. isinstance()检查一个对象是否是某个特定类型的实例 e.g., isinstance(a, int)
5. a=b, a和b是指向同一个对象的引用，改变任何一个的值，另一个引用就会跟着变。list函数始终会创建新列表
6. is和==不是一回事，前者用来判断是不是一个对象，后者仅仅判断内容是否一样。前者也用来判断是否为None，因为None实例只有一个
7. // 除后圆整运算符
8. 字符串是immutable
9. 字符串最左边引号前面加上r，表示所有字符应该按照原本的样子进行解释
10. None不是一个保留关键字，它只是NoneTpye的一个实例而已
11. pass是‘空操作’，将pass用作代码中的占位符
12. range函数用于产生一组间隔平均的整数，range(10),也可以指定起始值、结束值及步长，range(0,20,2),不包括末端值
13. 元组一旦创建完毕就不能被修改，但可以这样，`tup[1].append(3)`，元组可以通过+连接产生更长的元组，也可以乘以一个整数，相当于连接多个副本
14. 元组和列表一个非常有用的方法，count计算指定值的出现次数`a.count(2)`
15. append将元素添加到列表末尾，insert可以将元素插入到列表的指定位置`b.insert(1,'red')`，逆运算是pop，用于移除并返回指定索引出的元素，`remove`用于按值删除元素
16. 合并列表`extend`要比`+`快得多
17. `sort`可以实现就地排序，无需创建新对象
18. `bisect.bisect`可以找出新元素应该被插入到哪个位置才能保持原列表的有序性，`bisect.insort`则确实将新元素插入到那个位置
19. `seq[::2]`每隔一位取出一个元素，`seq[::-1]`实现反序
20. `enumerate`逐个返回序列的`(i,value)`元组，`mapping=dict((v,i) for i,v in enumerate(some_list))`
21. `sorted`函数将任何序列返回为新的有序列表，常将`sorted`和`set`结合使用得到一个又序列中的唯一元素组成的有序列表，e.g.,`sorted(set('this is just some string'))`
22. `zip`将多个序列的元素配对，产生一个新的元组列表，可以结合`enumerate`使用，`for i,(a,b) in enumerate(zip(seq1,seq2)):print('%d: %s, %s' % (i,a,b))`
23. `zip`也有对序列解压的功能，`zip(*pitchers)`
24. `reversed`用于按逆序迭代序列中的元素`list(reversed(range(10)))`
25. `empty_dict={}`字典，`'b' in d1`判断字典中是否存在某个键，使用`del`关键字或`pop`方法（删除指定键后将其值返回）可以删除值
26. `python3`,`dict.keys()`,`dict.values()`返回迭代器而不是列表
27. `update`方法，一个字典可以被合并到另一个字典
28. 将两个序列中的元素配对组成字典`mapping=dict(zip(range(s),reversed(range(5))))`
29. 集合运算，`a.difference(b)` a中不属于b的元素，`a.symmetric_difference(b)` a或b中不同时属于a和b的元素，`a.issubset(b),a.issuperset(b),a.disjoint(b)`子集、超集、是否存在连接
30. `map`函数用于在一组数据上应用一个函数
31. 生成器表达式（generator expression）有一个类似于列表、字典、集合推导式的东西，其创建方式为，把列表推导式两端的方括号改为圆括号`gen=(x**2 for x in xrange(100))`
32. `sum.__doc__`获取`sum`函数的文档字符串，`help(sum)`也可以
33. 复制一个列表的副本，`n=names[:]`
34. `*`收集其余的位置参数，返回元组；`**`收集关键字参数，返回字典
35. 
