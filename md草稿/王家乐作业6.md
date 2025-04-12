# An infinitesimal term in the Schwarz integral formula

**Problem Statement :**  
Let $ f \in H(B(0, R)) \cap C(\overline{B(0, R)}) $, where $ f = u + iv $. Prove that for any $ 0 < r \leq R $, the following holds:  
$$
f'(0) = \frac{1}{\pi r} \int_0^{2\pi} u(re^{i\theta}) e^{-i\theta} \, d\theta.
$$

**Issue in Proof:**  
I have completed the proof using another method, but encountered a problem when verifying differentiability directly via the definition.  

My computation yields:  
$$ L = f(z) - f(0) - z \cdot \frac{1}{\pi r} \int_{0}^{2\pi} u(re^{i\theta}) e^{-i\theta} \, \mathrm d\theta = \frac{z^{2}}{\pi} \int_{0}^{2\pi} \frac{u(re^{i\theta})}{re^{i\theta}(re^{i\theta} - z)} \,\mathrm d\theta, \quad \forall\ r \in (0, R].$$
Here, I used the **Schwarz integral formula**:
$$\displaystyle  f(z) = \frac{1}{2\pi} \int_{0}^{2\pi} \frac{Re^{i\theta} + z}{Re^{i\theta} - z} u\left(Re^{i\theta}\right) d\theta + iv(0).$$

**Goal:**  
Prove that 
$$\lim_{z \to 0} \frac{|L|}{|z|} = 0.$$