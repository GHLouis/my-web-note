---
{"dg-publish":true,"permalink":"/shared note/web note test/","tags":["gardenEntry"]}
---


# 20230708
## 小变形、线弹性假设
如何理解？
计算简图不会发生改变，原来是什么方向，变形后依然可以认为是什么方向
悬臂梁的例子

## 习题2-19
==求位移，注意方向。==

型钢的参数，参见Page 362，注意是两片角钢共同工作
刚性杆：不会发生变形的杆件

## 习题2-20
$$
\delta=\int \frac{F(x)dx}{EA(x)}
$$
如果是等截面二力杆，上式变为：
$$
\delta=\frac{FL}{EA}
$$
# 20230705
## 细节解释
柔软：制动带与圆盘之间是`滑动`，所以用滑动摩擦力公式$f=\mu F_N$
角度关系：$d\theta \rightarrow \dfrac{d\theta}{2}$，初中几何
## 公式推导
平衡方程

$$\sum F_{r}=0,\mathrm{d}F_{r}-(F+\mathrm{d}F)\sin\frac{\mathrm{d}\theta}{2}-F\sin\frac{\mathrm{d}\theta}{2}=0 \quad(1)$$
$$\sum F_{\theta}=0,(F+\mathrm{d}F)\cos\frac{\mathrm{d}\theta}{2}-F\cos\frac{\mathrm{d}\theta}{2}-f\mathrm{d}F_{r}=0 \quad(2)$$

由(1)得到$$\mathrm{d}F_{r}=(2F+\mathrm{d}F)\sin\frac{\mathrm{d}\theta}{2}\approx(2F+\mathrm{d}F)\frac{\mathrm{d}\theta}{2}\approx F\mathrm{d}\theta  \quad(3)$$
由(2)得到
$$\mathrm{d}F\cos\frac{\mathrm{d}\theta}{2}=f\mathrm{d}F_{r} \rightarrow \mathrm{d}F=f\mathrm{d}F_{r}  \quad(4)$$
把（3）代入（4）中，得到
$$dF=fFd\theta$$
分量变量，把有F的放到一边，有$\theta$的放到另一边：
$$\frac{dF}{F}=fd\theta$$
左右两边同时积分：
$$\int\frac{dF}{F}=\int fd\theta$$
得到：
$$\ln F=f\theta + C_0$$
两边同时取对数：
$$F=e^{f\theta + C_0}=e^{f\theta}e^{C_0}=Ae^{f\theta}$$
最后看书，根据边界条件得到$F$的表达式
