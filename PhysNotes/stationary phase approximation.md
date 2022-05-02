from [[@colemanQUANTUMFIELDTHEORY2018#17 4 Obtaining the decay law by stationary phase approximation zotero open-pdf 0_4E7XKTS3 408|QFT by S.C.]].

If we have an integral
$$
I=\int d t e^{i \theta(t)} g(t)
$$
with a real function $\theta(t)$ that varies rapidly compared to the rate at which $g(t)$ varies, then in general the value of this integral will be zilch-nothing. Because $\theta(t)$ is oscillating rapidly, the exponential averages out to zero. The main contribution to the integral comes at points of stationary phase, where the derivative of $\theta(t)$ is zero. At such points $\theta(t)$ is not rapidly varying; it doesn't vary at all. Therefore the integral is dominated by stationary phase points. I will assume there is only one such point, $t_{0}$;
$$
\frac{d \theta}{d t}=0 \text { for } t=t_{0}
$$
If there are several such points, you get a sum. People normally like to phrase this principle by putting a parameter $\lambda$ in front of $\theta(t)$ and say "we're studying large $\lambda$." That's neither here nor there. There may or may not be an adjustable parameter in the theory. It's just that if $\theta(t)$ is varying very rapidly, and $g(t)$ is not, this is a good approximation. We therefore approximate the integral by its value near the stationary phase point. By the stationary phase approximation
$$
I=e^{i \theta\left(t_{0}\right)} g\left(t_{0}\right) \int d t e^{\frac{i}{2} \theta^{\prime \prime}\left(t_{0}\right)\left(t-t_{0}\right)^{2}}
$$
The integral is trivial: it is a complex version of a Gaussian, and it gives us
$$
I=e^{i \theta\left(t_{0}\right)} g\left(t_{0}\right) \sqrt{\frac{2 \pi}{\left|\theta^{\prime \prime}\left(t_{0}\right)\right|}} e^{i(\pi / 4) \operatorname{sgn}\left(\theta^{\prime \prime}\left(t_{0}\right)\right)}
$$
If $\theta^{\prime \prime}\left(t_{0}\right)=0$, we have to think again. We have to expand out to the quartic term, or cubic, whichever is the first non-vanishing one. We will apply this method to our amplitude, (17.33).