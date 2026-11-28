# Module 1: Single-Mode and Multi-Mode Quantum States of Light

This module explores canonical field quantization, the quantum vacuum, the complete taxonomy of single-mode radiation states, ladder operators, phase operators, photon counting statistics, and higher-order quantum coherence.

---

### Notebook Syllabus

| # | Notebook | Core Topics |
| :-: | :--- | :--- |
| **01** | [`01_canonical_field_quantization_and_vacuum.ipynb`](./01_canonical_field_quantization_and_vacuum.ipynb) | Maxwell equation quantization, Coulomb gauge $\mathbf{A}(\mathbf{r})$, field operators $\hat{\mathbf{E}}$ and $\hat{\mathbf{B}}$, vacuum zero-point energy $\frac{1}{2}\hbar\omega$, Euler-Maclaurin regularization, Casimir attraction $P \propto d^{-4}$ |
| **02** | [`02_fock_states_and_ladder_operators.ipynb`](./02_fock_states_and_ladder_operators.ipynb) | Discrete Fock space, ladder operators $\hat{a}, \hat{a}^\dagger$, commutator boundary artifact $-(N-1)$, quadrature noise $\frac{2n+1}{4}$, cutoff convergence $N \ge \bar{n} + 4\sqrt{\bar{n}} + 10$ |
| **03** | [`03_coherent_states_and_displacement.ipynb`](./03_coherent_states_and_displacement.ipynb) | Displacement operator $\hat{D}(\alpha)$, coherent states $|\alpha\rangle$, Poissonian statistics, minimum uncertainty $\Delta X_1 \Delta X_2 = 1/4$, phase space circles, overcomplete basis |
| **04** | [`04_squeezed_states_and_quadrature_noise.ipynb`](./04_squeezed_states_and_quadrature_noise.ipynb) | Squeeze operator $\hat{S}(\xi)$, quadrature noise ellipses, Bogoliubov transformation, even-Fock number distributions, noise reduction below shot noise (dB scaling) |
| **05** | [`05_displaced_squeezed_states.ipynb`](./05_displaced_squeezed_states.ipynb) | Displaced squeezed states $\hat{D}(\alpha)\hat{S}(\xi)|0\rangle$ vs $\hat{S}(\xi)\hat{D}(\alpha)|0\rangle$, operator commutation $\gamma = \alpha\cosh r - \alpha^* e^{i\theta}\sinh r$, amplitude vs phase squeezing, Schleich-Wheeler interference in phase space |
| **06** | [`06_thermal_and_mixed_states.ipynb`](./06_thermal_and_mixed_states.ipynb) | Thermal states $\hat{\rho}_{\text{th}}$, Bose-Einstein distribution, Einstein 1909 fluctuation decomposition $\bar{n} + \bar{n}^2$, purity $\mathcal{P} = 1/(2\bar{n}+1)$, von Neumann entropy, phase-diffused laser comparison |
| **07** | [`07_quantum_phase_operators_and_pegg_barnett.ipynb`](./07_quantum_phase_operators_and_pegg_barnett.ipynb) | Dirac phase operator paradox, Susskind-Glogower non-unitary operators, Pegg-Barnett discrete $(s+1)$-dimensional phase basis, continuous $P(\theta)$, number-phase uncertainty $\Delta N \Delta\Phi \ge 1/2$ |
| **08** | [`08_mandel_q_parameter.ipynb`](./08_mandel_q_parameter.ipynb) | Mandel $Q$-parameter, Fano factor, Glauber-Sudarshan non-classicality proof ($Q < 0$), sufficient vs necessary criteria, squeezing optimization landscape |
| **09** | [`09_second_order_coherence_g2.ipynb`](./09_second_order_coherence_g2.ipynb) | Zero-delay coherence $g^{(2)}(0)$, Cauchy-Schwarz inequality, HBT interferometer, photon anti-bunching ($g^{(2)} < 1$), bunching ($g^{(2)} = 2$), detector jitter and $g^{(2)}(0) < 0.5$ criterion |
| **10** | [`10_higher_order_coherence_and_hbt.ipynb`](./10_higher_order_coherence_and_hbt.ipynb) | Glauber $n$-th order coherence $g^{(n)}(0)$, thermal factorial super-bunching $n!$, multi-detector HBT delay landscape $g^{(3)}(\tau_1, \tau_2)$, single-photon multi-coincidence vanishing |
