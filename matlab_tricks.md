1. 续行符　...
2. 如果已知命令开头的一个或若干个字符，可以输入这些字符再按向上箭头进行查找，效率极高。
3. doc function 可直接打开相关帮助文档
4. 代码自动整理（智能缩进smart indent）Ctrl + I
5. 用　%% 构建一个cell，当光标位于某一个cell时，在菜单选“Evaluate current cell”或Ctrl+Enter即可执行该模块中的所有代码，其它模块不执行
6. matlab是解释型语言，不是编译型语言，可以这样初始化变量 x=[];
7. 可以利用lookfor命令去找自己不知道准确名字的函数，其搜索空间包括函数的注释及函数名称本身
8. 构建函数时，第一个函数之后的函数只能被第一个函数或当前文件中的其它子函数调用，这种函数我们称之为"私有函数"
9. 在一个函数中可以利用　nargin 来判断函数被调用时输入参数的个数
10. size(A,1)返回A的行数
11. syms 定义符号
12. cat(1,A,B)按列拼接，cat(1,A,B)按行拼接，cat(1,A,B)按页拼接
13. rand(n),生成nxn随机矩阵，元素服从参数为(0,1)的均匀分布。用rng设置随机数种子，e.g., rng(sd,'v4')
14. rand(m,n)*(b-a)+a对产生的随机数取整即可得到均匀分布的整数，比如floor或ceil，另外，randi也可产生均匀分布的整数
15. randn元素服从标准正态分布,要产生非标准的（mu,sigma2）正态分布，可以使用randn(m,n)*sigma+mu，mean,std,var
16. randperm(n,k)生成长度为k的随机整数排列的向量，元素在1-n之间，只是不放回抽样，若要产生有重复的，应使用randi函数，抽样之前可以先设置种子, e.g., rng(2)
17. nnz()计算非零元素的个数，nonzeros()找出矩阵中非零元素的个数，按列优先；nzmax(s)返回非零元素所占内存大小
18. expand(y)函数将符号多项式展开,参数是多项式的符号表示
19. ismember(A,S)检测集合中的元素，判断A中的元素是否在S中
20. viscircles(centers,radii): to draw a circle in matlab
