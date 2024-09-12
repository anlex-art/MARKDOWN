#  <font face="仿宋" font color=orange>Laplace Derivation</font>
## 数学推导

#### 1. 定义目标函数

考虑一个函数 \( f(x) \)，当参数 \( n \) 很大时，我们想要近似计算以下积分：

\[
\int_{-\infty}^{\infty} e^{n f(x)} \, dx
\]

#### 2. 泰勒展开

在 \( x = x_0 \) 处 \( f(x) \) 取得极大值点。对函数 \( f(x) \) 在 \( x_0 \) 附近进行二阶泰勒展开：

\[
f(x) \approx f(x_0) + \frac{1}{2} f''(x_0) (x - x_0)^2
\]

#### 3. 指数函数近似

将泰勒展开代入积分中，得到：

\[
e^{n f(x)} \approx e^{n f(x_0)} e^{\frac{n}{2} f''(x_0) (x - x_0)^2}
\]

#### 4. 高斯积分

对上式中的指数项进行积分。使用高斯积分结果：

\[
\int_{-\infty}^{\infty} e^{\frac{n}{2} f''(x_0) (x - x_0)^2} \, dx = \sqrt{\frac{2 \pi}{- f''(x_0)}}
\]

#### 5. 合并结果

将结果代入之前的公式，得到拉普拉斯近似：

\[
\int_{-\infty}^{\infty} e^{n f(x)} \, dx \approx e^{n f(x_0)} \sqrt{\frac{2 \pi}{- f''(x_0)}}
\]

