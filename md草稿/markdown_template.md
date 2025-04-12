小船的运动由以下微分方程组描述：

$$
\begin{cases} 
\frac{dx}{dt} = v_1 - v_2 \cos \alpha, \\ 
\frac{dy}{dt} = v_2 \sin \alpha, 
\end{cases}
$$

其中角度 $\alpha$ 满足：

$$
\sin \alpha = \frac{-y}{\sqrt{x^2 + y^2}}, \quad \cos \alpha = \frac{x}{\sqrt{x^2 + y^2}}.
$$

## 2. 极坐标变换
将笛卡尔坐标 $(x, y)$ 转换为极坐标 $(r, \theta)$：

$$
\begin{cases} 
x = r \cos \theta, \\ 
y = r \sin \theta. 
\end{cases}
$$

## 3. 极坐标下的微分方程
原方程转化为：

$$
\begin{cases} 
\displaystyle \frac{dr}{dt} = v_1 \cos \theta - v_2, \\ 
\displaystyle \frac{d\theta}{dt} = -\frac{v_1 \sin \theta}{r}. 
\end{cases}
$$

## 4. 消去时间变量 $t$
通过链式法则消去 $t$，并代入初值条件 $r(-\frac{\pi}{2}) = d$：

$$
\begin{cases} 
\frac{dr}{d\theta} = -r \frac{v_1 \cos \theta - v_2}{v_1 \sin \theta}, \\ 
r\left(-\frac{\pi}{2}\right) = d. 
\end{cases}
$$

## 5. 解析解
最终得到小船航线的极坐标解析解：

$$
r(\theta) = d \left| \frac{\csc \theta - \cot \theta}{|\sin \theta|} \right|^{\frac{1}{k}}.
$$

其中 $k = \frac{v_2}{v_1}$ 为速度比参数。