## Welcome to GitHub Pages - Blog for OI

## 可以选择查看更正常的显示（需要FastGithub）
[Link](https://github.com/NESGUIAM/oi)

## Markdown（这个表格在Github Pages不能正常显示，可以不管,是用于记Markdown的语法的）
|Markdown|————————————————|Preview|
|:--:|:--:|:--:|
|\~\~text\~\~||~~text~~|
|\*text\*||*text*|
|\*\*text\*\*||**text**|
|\*\*\*text\*\*\*||***text***|
|\`text(code)\`||`text(code)`|
|H\<sub>2\</sub>O||H<sub>2</sub>O|
|O(n\<sup>2\</sup>)||O(n<sup>2</sup>)|
|\$H_2O\$|（数学公式）|$H_2O$|
|\$O(n^2)\$|（数学公式）|$O(n^2)$|
|\-\-\-||分割线，表格不支持显示|
|\# text||一级标题（最大）|
|\#\#\#\#\#\# text||六级标题（最小）|
|\- text||无序列表|
|\+ text||- - -|
|\* text||- - -|
|箭头||[Link](https://blog.csdn.net/Ricky2007/article/details/109455046)|
|\$\neq\$|（数学公式）|$\neq$|
|\$\geq\$|（数学公式）|$\geq$|
|\$\leq\$|（数学公式）|$\leq$|
|\`\`\`cpp<br>text<br>\`\`\`||Example 1|
|\[Link\]\(https://example.com\)||[Link](https://example.com)
|\!\[Example imagine\]\(https://raw.githubusercontent.com/NESGUIAM/OI/main/test_img.png\)|(图片可能会用到Fastgithub)|![Example imagine](https://raw.githubusercontent.com/NESGUIAM/OI/main/test_img.png)|

+ **Example 1**
```cpp
#include <iostream>
using namespace std;
int main(){
    // Code
    return 0;
}
```

---

## 1. 题目：油滴扩展

[Link](https://www.luogu.com.cn/problem/P1378)

---

### 涉及算法/考点：
全排列

### 解题思路：
全排列枚举所有顺序，计算。*n* 很小，全排列复杂度并不会超时，不需要优化
### 解题关键点：
摆放油滴不同的顺序会产生不同的结果，需要列举出全部可能性再逐一比较
### 易错点/出现的错误总结：
1. 计算半径时，可能出现负数，要赋值为 *0*
2. *π*的取值要到后六位以上（r的上限为 *10<sup>6</sup>* , *πr<sup>2</sup>* 要保留整数位）
3. 摆放的第i个油滴的下标并不是[i]
### 通用技巧总结：
1. *abs* 函数可以获取绝对值
2. *sqrt* 函数可以取根号值
### 类比题目：
- 全排列

---

## 2. 题目：[CSP-J2019 江西] 次大值(考试max)

[Link](https://www.luogu.com.cn/problem/P5682)

### 涉及算法/考点：
数学简单推理与优化

### 解题思路：
对*Mod*暴力进行优化
### 解题关键点：
结果只与 *Max<sub>1</sub>*%*Max<sub>2</sub>* 和 *Max<sub>3</sub>* 有关，取最大值即为结果

### 易错点/出现的错误总结：
1. 在分析时，容易以为答案就是原数组第三大的数
### 通用技巧总结：
1. 通过暴力进行优化
### 类比题目：
- (空)

---