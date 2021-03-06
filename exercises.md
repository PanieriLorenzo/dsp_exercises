# Chapter 2 (Week 1)

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

## Exercise 2.11 - Sum of Sinusoids of Same Frequency

![image-20210614124310589](image-20210614124310589.png)

Rewrite into exponential form and factor out $e^{j\omega t}$ frequency component to get the three phase and amplitude phasors without any variables.

$x(t)=\Re\{(e^{-j\pi}+e^{j\pi/3}+2e^{-j\pi/3})e^{j\omega t}\}$

Now I write each of the three phasors in cartesian form:

* $e^{j\pi}\to \cos(\pi)+j\sin(\pi)=-1+j0$
* $e^{j\pi/3}\to\cos(\pi/3)+j\sin(\pi/3)=\frac{1}{2}+j\frac{\sqrt{3}}{2}$
* $2e^{-j\pi/3}\to2\cos(-\pi/3)+j2\sin(-\pi/3)=1-j\sqrt{3}$

Now we add everything together and simplify:

$x(t)=\Re\{(\frac{1}{2}-j\frac{\sqrt{3}}{2})e^{j\omega t}\}$

Now we need to get it back into standard sinusoid form, so we need to rewrite the phasor in polar form, and multiply the frequency component back on:

$\varphi = \angle X = \operatorname{atan}\left(\dfrac{-\sqrt 3/2}{1/2}\right)=-\pi/3$

$A=|X|=\sqrt{\left(-\sqrt 3/2\right)^2+\left(1/2\right)^2}=1$

$x(t)=\Re\{e^{-j\pi/3}e^{j\omega t}\}$

Now we can finally get the standard sinusoid form:

$x(t)=\cos(\omega t - \pi/3)$

**Note:** if you are feeling adventurous you can bypass the exponential form entirely, by doing some steps in your head.

## Exercise 2.17 - TODO

![image-20210609140253759](image-20210609140253759.png)

## Exercise 2.20 - TODO

![image-20210609140314932](image-20210609140314932.png)

## Exercise 2.24 - TODO

![image-20210609140330006](image-20210609140330006.png)



# Chapter 3 (Week 2)

## Exercise 3.1 - Reading Spectrum Representation

![image-20210610150322777](image-20210610150322777.png)

![image-20210610150339320](image-20210610150339320.png)

**a)**

$x(t) = 11 + 14\cos(100\pi-\pi/3)+8\cos(350\pi-\pi/2)$

**b)**

Yes. Its fundamental frequency is the greatest common divisor between the frequencies of the two cosines. Then you take the reciprocal.

```matlab
clear
gcd(50, 175)
% 25
```

**c)**

Because otherwise the signal would be complex, and that doesn't make sense for real signals.

## Exercise 3.3 - Standard Form to Spectrum Form

![image-20210610150411913](image-20210610150411913.png)

**a)**

$z(t) = 2 + \cos(t) + 2\cos(2 t) + \Re\{2 e^{j\pi/3} e^{j3t}\}$

$z(t)=2+\cos(t)+2\cos(2t)+2\cos(3t+\pi/3)$

**b)**

Bruh I don't feel like it.

## Exercise 3.4 - TODO

![image-20210610150428345](image-20210610150428345.png)



## Exercise 3.9 - TODO

![image-20210610150452607](image-20210610150452607.png)

## Exercise 3.13 - TODO

![image-20210610150514717](image-20210610150514717.png)

## Exercise 3.16 - TODO

![image-20210610150539693](image-20210610150539693.png)

## Exercise 3.24 - TODO

![image-20210610150610065](image-20210610150610065.png)

# Chapter 4 (Week 3)

## Exercise 4.1 -

![image-20210611120329336](image-20210611120329336.png)

## Exercise 4.8 -

## Exercise 4.12 -

## Exercise 4.15 -

## Exercise 4.17 -

# Chapter 5 (Week 4) - 

## Exercise 5.1 -

## Exercise 5.4 -

## Exercise 5.6 - (Skipped)

![image-20210614180618970](image-20210614180618970.png)

Not relevant for exam

## Exercise 5.7 -

## Exercise 5.13 -

## Exercise 5.18 -

# Chapter 6 (Week 5) -

## Exercise 6.2 -

## Exercise 6.6 - z-Transform, Frequency Response, Convolution

![image-20210614162046320](image-20210614162046320.png)

**a)**

First finding the z-transform of the filter:

$h[n]=\delta[n]-\delta[n-4]$

$H(z)=1-z^{-4}$

Finding the frequency response by setting $z=e^{j\hat\omega}$

$H(\hat\omega)=1-(e^{j\hat\omega})^{-4}=1-e^{-4j\hat\omega}$

I couldn't get it to that form.



**b)**

$x[n]=4+\cos(0.25\pi n-\pi/4)$ is given

$x[n-4]=4+\cos(0.25\pi (n-4) - \pi/4)$ is the time shifted input

$=4+\cos(0.25\pi n - \pi -\pi/4)$

$= 4+\cos(n \pi/4-\pi 5/4)$

So the output will be:

$y[n]=\cos(n \pi/4-\pi/4)-\cos(n\pi/4 - \pi 5/4)$

In cartesian phasor form, factoring out the frequency phasor:

$y[n]=\Re\{(\cos(-\pi/4)+j\sin(-\pi/4)-\cos(-\pi 5/4)-j\sin(-\pi5/4))e^{n \pi/4}\}$

$y[n]=\Re\{(1/\sqrt 2-j 1/\sqrt 2+1/\sqrt2-j1/\sqrt{2})e^{n\pi/4}\}$

$y[n]=\Re\{(\sqrt{2}-j\sqrt{2})e^{n\pi/4}\}$

Now I re-write in polar form, using Wolfram Alpha

$A=2, \varphi=-\pi/4$

Finally the output in standard form is:

$y[n]=2\cos(n \pi/4 -\pi/4)$



**c)**

For positive values of $n$ the two functions never cross because one has a maximum amplitude of 2, and the other one is shifted with a DC offset of 4 and has an amplitude of 1. So they are only the same for negative values of $n$, so when:

$2\cos(n\pi/4 -\pi/4) = 0$

... dunno



## Exercise 6.7 -

## Exercise 6.13 -

## Exercise 6.19 -

## Exercise 6.23 -

# Chapter 7 (Week 6) -

## Exercise 7.1 -

## Exercise 7.2 -

## Exercise 7.8 -

## Exercise 7.11 -

# Chapter 8 (Week 7) - DFT & FFT

## Exercise 8.1 - Frequency Sampling

![image-20210614152924717](image-20210614152924717.png)

![image-20210614152933851](image-20210614152933851.png)

**a)**

$x = [1, 0, 0, 0, 0, 0, 0, 0, 0, 0] =\delta[n]\quad n\in[0, 9]$

$DTFT\{x\}=X(\hat\omega)=1$

$DFT\{x\}=X(2\pi k/10)=[1,1,1,1,1,1,1,1,1,1]$

Checking in Matlab:

```matlab
clear
a = [1 0 0 0 0 0 0 0 0 0]
A = fft(a)
% 1 1 1 1 1 1 1 1 1 1
stem(A) % plots FFT spectrum
```

**b)**

Skipped rest of them

## Exercise 8.2 -

## Exercise 8.8 -

# Chapter 9 (Week 8) -

## Exercise 9.1 -

## Exercise 9.3 -

## Exercise 9.4 -

## Exercise 9.6 -

## Exercise 9.14 -

# Chapter 10 (Week 9, 10) -

## Exercise 10.1 -

## Exercise 10.2 - IIR Filter Impulse Response

![image-20210614202338404](image-20210614202338404.png)

![image-20210614202349742](image-20210614202349742.png)

The smallest delay in the difference equation is 1 sample, so at $n=0$ and before, the output will be 0.

The first step to finding the impulse response is taking the $z$ transform, this is done by putting all y terms in the denominator and all the x terms in the numerator, then the delay amount becomes the exponent of the $z$ variable:

$H(z)=\dfrac{z^{-1}}{1-0.9z^{-1}+0.9z^{-2}}$

Now I use Matlab to find the partial fraction decomposition, so we can find the closed-form impulse response:

```matlab
clear
[r, p, k] = residue([1 0],[0.9 -0.9 1])
[theta rho] = cart2pol(real(r), imag(r))
% theta = 2??1    
%   -0.4942
%    0.4942
%
% rho = 2??1    
%    0.6311
%    0.6311

[theta rho] = cart2pol(real(p), imag(p))
% theta = 2??1    
%    1.0766
%   -1.0766
%
% rho = 2??1    
%    1.0541
%    1.0541
```

$H(z)=\dfrac{0.\overline5-j0.2993}{z^{-1}-0.5-j0.928}+\dfrac{0.\overline5+j0.2993}{z^{-1}-0.5+j0.928}$

$H(z)=\dfrac{0.6311e^{-j0.4942}}{z^{-1}-1.0541e^{j1.0766}}+\dfrac{0.6311e^{j0.4942}}{z^{-1}-1.0541e^{-j1.0766}}$

Now the inverse $z$ transform can get us the impulse response:

...dunno

## Exercise 10.3 -

## Exercise 10.5 -

## Exercise 10.6 -

## Exercise 10.7 -

## Exercise 10.8 -

## Exercise 10.9 -

## Exercise 10.11.3 -

## Exercise 10.11.4 -

## Exercise 10.11.5 -

## Exercise 10.12 -

