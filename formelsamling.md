# Sinusoids

$$x(t) = A\cdot\cos(\omega_0 t + \varphi) = A\cos(2\pi f_0 t + \varphi)$$

where:

* $$A$$ is amplitude
* $\varphi$ is phase shift, is in radians, not seconds, i.e. time shift relative to the frequency.
* $\omega_0$ is the radian frequency (radians per second)
* $f_0 = \omega_0/(2 \pi)$ is the cyclic frequency (normal nice intuitive frequency)

## Period vs. Frequency

$$T_0=\dfrac{1}{f_0}=\dfrac{2\pi}{\omega_0}$$

Where $T_0$ is the *period* of the oscillation, i.e. how long it takes for a single cycle of oscillation, start to finish, whereas $f_0$ is how many oscillations per second.

## Time-Shift vs. Phase-Shift

Phase shift is relative to frequency and is in radians, time shift is absolute and is in seconds.

$$x(t - t_0) = A\cdot\cos(\omega_0 (t - t_0) + \varphi)$$

Where:

* $t_0$: time shift
* $\varphi$: phase shift
* Everything else explained above

## Complex Exponential Form

Complex exponentials are basically vectors that spin around the origin. The x and y coordinates are a sine and cosine function, so sinusoids can be re-written as complex exponentials.

$$A e^{j(\omega_0 t+\varphi)} = A\cos(\omega_0 t + \varphi) + jA\sin(\omega_0 t + \varphi)$$

### Regneregler

$$\cos\theta = \dfrac{e^{j\theta} + e^{-j\theta}}{2}$$

$$\sin\theta =\dfrac{e^{j\theta}-e^{-j\theta}}{2j}$$

Sum of sinusoids with the same frequency, but different phases or amplitudes, is a new sinusoid with the same frequency but different amplitude and phase.

$$\cos(...) + \cos(...) + ...$$ (where they have the same frequency but not the same amplitude or phase)

$$\sum A_ke^{j\phi_k} = Ae^{j\phi}$$

$$\Re\{Ae^{j\phi}e^{j\omega_0 t}\}=\cos(...)$$

If you need to sum a bunch of sinusoids that have the same frequency, just transform them to polar form, add them together, multiply the result by $e^{j\omega_0 t}$ and take the real part and that's the sum.



