<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>

# PSO
较为通用的粒子群优化算法（变量维度可变）

# 使用

编写适应度函数及主函数即可，无任何依赖项

# 示例

求解\\(f(x) = sin(sqrt(x^2+y^2))/sqrt(x^2+y^2) + exp((cos(2*pi*x)+cos(2*pi*y))/2) -2.71289\\)的极大值。该函数有很多局部极大值点，而极线位置为（0，0），在（0，0）附近取得极大值。

编写适应度函数如`FitnessFunction.h`，编写主函数如`main_test.cpp`，运行过程会打印出每次迭代的结果，最终得到的结果接近（0，0），适应度值为1.00539。

示例是一个非常简单的例子，其中变量维度为2（坐标为二维），本程序可以适用于不同变量维度，更改对应参数即可。
