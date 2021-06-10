# Chapter 2

## Exercise 2.1 - Plotting in Matlab

![image-20210609134127706](image-20210609134127706.png)

```matlab
clear
syms t
x = 3 * cos(0.2 * pi * t - 0.25 * pi)
fplot(x, [-10, 20])
```

## Exercise 2.4 - (Skipped)

## Exercise 2.5 - Phasor Form

![image-20210609131722582](image-20210609131722582.png)

**a) Calculations In Phasor Form**

$$\cos(\theta_1 +\theta_2)$$ 

$$= \Re\{\cos(\theta_1 + \theta_2) + j\sin(\theta_1 + \theta_2)\}$$ 

$$= \Re\{e^{j(\theta_1 + \theta_2)}\}$$

$$=\Re\{e^{j\theta_1 + j\theta_2}\}$$

$$=\Re\{e^{j\theta_1}e^{j\theta_2}\}$$

$$=\Re\{(\cos(\theta_1)+j\sin(\theta_1))(\cos(\theta_2)+j\sin(\theta_2))\}$$

$$=\Re\{\cos(\theta_1)\cos(\theta_2)+j^2\sin(\theta_1)\sin(\theta_2)+j\cos(\theta_1)\sin(\theta_2)+j\sin(\theta_1)\cos(\theta_2)\}$$

$$=\Re\{\cos(\theta_1)\cos(\theta_2)-\sin(\theta_1)\sin(\theta_2)+j\cos(\theta_1)\sin(\theta_2)+j\sin(\theta_1)\cos(\theta_2)\}$$

$$=\cos(\theta_1)\cos(\theta_2)-\sin(\theta_1)\sin(\theta_2)$$

QED

**b) (Skipped)**

## Exercise 2.7 - Complex Number Arithmetic

![image-20210609135441891](image-20210609135441891.png)

**a)**

```matlab
clear
a = 3*exp(j * pi / 3) + 4 * exp(-j * pi / 6)
[theta, r] = cart2pol(real(a), imag(a))
% a = 4.9641 + 0.5981i
% theta = 0.1199
% r = 5.0000
```

Cartesian form:

$4.9641 + j0.5981$

Polar form:

$5e^{j0.1199}$

**b)**

```matlab
clear
b = (sqrt(3) - j*3)^10
[theta, r] = cart2pol(real(b), imag(b))
% b = -1.2442e+05 + 2.1549e+05i
% theta = 2.0944
% r = 248832
```

Skipped the rest cause it's the same.

## Exercise 2.11 - TODO

![image-20210609140233898](image-20210609140233898.png)

## Exercise 2.17 - TODO

![image-20210609140253759](image-20210609140253759.png)

## Exercise 2.20 - TODO

![image-20210609140314932](image-20210609140314932.png)

## Exercise 2.24 - TODO

![image-20210609140330006](image-20210609140330006.png)



