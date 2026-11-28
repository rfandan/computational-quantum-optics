# Module 4: Open Quantum Systems, Dissipation & Trajectories

This module provides a rigorous, publication-grade computational exploration of **Open Quantum Systems** in quantum optics. It spans the complete progression from foundational microscopic reservoir derivations—deriving master equations from microscopic electron-phonon and field-emitter interactions—to the Gorini-Kossakowski-Sudarshan-Lindblad (GKSL) semigroup, continuous-variable cavity loss, stochastic quantum jump wavefunctions (MCWF), diffusive quantum trajectory monitoring, Itô vs. Stratonovich stochastic calculus, input-output scattering theory, non-Markovian memory kernels, and fully quantized laser and micromaser theory.

---

### Notebook Syllabus (10/10 Complete)

| # | Notebook | Core Topics |
| :-: | :--- | :--- |
| **01** | [`01_density_matrix_and_purity.ipynb`](./01_density_matrix_and_purity.ipynb) | Statistical mixtures, density operator properties ($\text{Tr}(\hat{\rho})=1, \hat{\rho}\geq 0$), purity $\gamma = \text{Tr}(\hat{\rho}^2)$, linear and von Neumann entropy $S = -\text{Tr}(\hat{\rho}\ln\hat{\rho})$, partial trace over bipartite composite spaces $\hat{\rho}_A = \text{Tr}_B(\hat{\rho}_{AB})$, 3D Bloch ball geometry of mixed qubit states, and Werner state benchmark. |
| **02** | [`02_microscopic_derivation_of_master_equations.ipynb`](./02_microscopic_derivation_of_master_equations.ipynb) | Microscopic system-bath Hamiltonian, Born approximation, Markov memoryless assumption, secular (rotating wave) coarse-graining, KMS condition $\gamma(-\omega)/\gamma(\omega) = e^{-\beta\hbar\omega}$, thermal bath detailed balance, Lamb-Stark energy shifts, and asymptotic thermal Gibbs state equilibration $\hat{\rho}_{\text{th}} = e^{-\beta\hat{H}_S}/Z$. |
| **03** | [`03_lindblad_master_equation.ipynb`](./03_lindblad_master_equation.ipynb) | Completely positive trace-preserving (CPTP) dynamical semigroups, Lindblad/GKSL superoperator dissipators $\mathcal{D}[\hat{L}]\hat{\rho}$, superoperator vectorization, Liouvillian generator matrix $\mathcal{L}$ of dimension $d^2 \times d^2$, steady-state kernel $\mathcal{L}\vec{\rho}_{\text{ss}} = 0$, dissipative spectral gap $\Delta_{\text{gap}}$, and transverse dephasing $\Gamma/2 + \gamma_\phi$. |
| **04** | [`04_cavity_decay_and_photon_loss.ipynb`](./04_cavity_decay_and_photon_loss.ipynb) | Continuous-variable Lindblad master equation for cavity decay $\kappa \mathcal{D}[\hat{a}]$, Fock state mixture cascade vs. coherent pointer state purity immunity ($\gamma(t) \equiv 1.0$), accelerated Schrödinger cat state decoherence rate $\Gamma_{\text{dec}} = 2\kappa|\alpha|^2 \gg \kappa$, thermal blackbody reservoir equilibration ($n_{\text{th}} > 0$), and phase-space Wigner quantum interference fringe erasure. |
| **05** | [`05_monte_carlo_wavefunction_method.ipynb`](./05_monte_carlo_wavefunction_method.ipynb) | The Dalibard-Castin-Mølmer (MCWF) / quantum jump method, effective non-Hermitian Hamiltonian $\hat{H}_{\text{eff}} = \hat{H} - \frac{i\hbar}{2}\sum_k \hat{L}_k^\dagger\hat{L}_k$, deterministic norm loss as Bayesian null-detection update, stochastic quantum jump selection and state collapse, $\mathcal{O}(d^2)$ computational scaling advantage, proof of GKSL equivalence, and photon waiting time distribution $w(\tau)$ displaying optical antibunching ($w(0) = 0$). |
| **06** | [`06_quantum_trajectories_and_homodyne_measurement.ipynb`](./06_quantum_trajectories_and_homodyne_measurement.ipynb) | Continuous measurement unravelings, balanced homodyne detection with intense local oscillator ($|\beta|\to\infty$), continuous differential photocurrent record $J(t)dt = 2\sqrt{\kappa}\langle\hat{x}\rangle dt + dW(t)$, Itô Stochastic Schrödinger Equation (SSE), measurement innovation and backaction, conditional quadrature squeezing $(\Delta x)^2 < 1/4$, and diffusive ensemble convergence to unconditional GKSL master equation. |
| **07** | [`07_stochastic_calculus_ito_vs_stratonovich.ipynb`](./07_stochastic_calculus_ito_vs_stratonovich.ipynb) | Wiener increments ($dW^2 = dt$), non-anticipating Itô discretization vs. midpoint Stratonovich integration, Wong-Zakai theorem and finite-bandwidth white noise limits, Itô lemma for non-linear quantum observables $df = f' dx + \frac{1}{2}f''(dx)^2$, stochastic state norm preservation, continuous homodyne photocurrent filtering, and ensemble recovery of GKSL decay. |
| **08** | [`08_input_output_theory_and_cavity_scattering.ipynb`](./08_input_output_theory_and_cavity_scattering.ipynb) | Gardiner-Collett input-output formalism, continuous bath mode quantization, boundary condition $\hat{a}_{\text{out}}(t) = \hat{a}_{\text{in}}(t) + \sqrt{\kappa}\hat{a}(t)$, Heisenberg-Langevin equations of motion in frequency domain, reflection $r(\omega)$ and transmission $t(\omega)$, undercoupled, critically coupled ($r(\omega_c) = 0, 100\%$ absorption), and overcoupled regimes, complex-plane Smith chart phase slips, strict energy conservation $R+T+A \equiv 1$, and atom-cavity vacuum Rabi splitting in transmission. |
| **09** | [`09_non_markovian_dynamics_and_spectral_densities.ipynb`](./09_non_markovian_dynamics_and_spectral_densities.ipynb) | Breakdown of Markov approximation, structured environments, Sub-Ohmic, Ohmic, and Super-Ohmic spectral densities $J(\omega) = \alpha \omega (\omega/\omega_c)^{s-1} e^{-\omega/\omega_c}$, resonant Lorentzian reservoirs, exact Volterra integro-differential equations, Time-Convolutionless (TCL) master equations, negative canonical decay rates $\gamma(t) < 0$ as information backflow, and Breuer-Laine-Piilo (BLP) trace distance measure $\mathcal{N}_{\text{BLP}}$. |
| **10** | [`10_laser_theory_and_micromaser.ipynb`](./10_laser_theory_and_micromaser.ipynb) | Semiclassical vs. fully quantized laser theory, Scully-Lamb master equation, detailed balance photon statistics $P(n)$, second-order non-equilibrium phase transition across lasing threshold $A = \kappa$, second-order coherence transition $g^{(2)}(0): 2 \to 1$, the single-atom micromaser (Meschede-Walther-Haroche), pump parameter $\theta = g\tau_{\text{int}}\sqrt{N_{\text{ex}}}$, and quantum trapping states $g\tau_{\text{int}}\sqrt{n_q + 1} = q\pi$ truncating $P(n > n_q) \equiv 0$ with macroscopic sub-Poissonian non-classical light ($Q < 0$). |

---

### Key Formulas & Physical Principles

* **GKSL Lindblad Master Equation:**
  $$\frac{d\hat{\rho}}{dt} = -\frac{i}{\hbar}[\hat{H}, \hat{\rho}] + \sum_k \left( \hat{L}_k \hat{\rho} \hat{L}_k^\dagger - \frac{1}{2}\{\hat{L}_k^\dagger \hat{L}_k, \hat{\rho}\} \right)$$

* **Vectorized Liouvillian Superoperator:**
  $$\mathcal{L} = -i\left(\hat{H} \otimes \hat{I} - \hat{I} \otimes \hat{H}^T\right) + \sum_k \left[ \hat{L}_k^* \otimes \hat{L}_k - \frac{1}{2}\hat{I}\otimes (\hat{L}_k^\dagger \hat{L}_k)^T - \frac{1}{2}(\hat{L}_k^\dagger \hat{L}_k)^* \otimes \hat{I} \right]$$

* **KMS Detailed Balance Condition:**
  $$\frac{\gamma(-\omega)}{\gamma(\omega)} = e^{-\beta \hbar \omega} \implies \hat{\rho}_{\text{ss}} = \frac{e^{-\beta \hat{H}_S}}{\mathcal{Z}}$$

* **Accelerated Cat State Decoherence Rate:**
  $$\Gamma_{\text{dec}} = 2\kappa |\alpha|^2 \gg \kappa, \quad W(0,0; t) \approx - \frac{2}{\pi} e^{-2\kappa|\alpha|^2 t}$$

* **MCWF Effective Non-Hermitian Hamiltonian & Jump Probability:**
  $$\hat{H}_{\text{eff}} = \hat{H} - \frac{i\hbar}{2}\sum_k \hat{L}_k^\dagger \hat{L}_k, \quad \delta p = \delta t \sum_k \langle\psi|\hat{L}_k^\dagger \hat{L}_k|\psi\rangle$$

* **Diffusive Stochastic Schrödinger Equation (Homodyne Detection):**
  $$d|\psi\rangle = \left[ -i\hat{H}dt - \frac{\kappa}{2}\left(\hat{a}^\dagger\hat{a} - 2\langle\hat{x}\rangle\hat{a} + \langle\hat{x}\rangle^2\right)dt + \sqrt{\kappa}\left(\hat{a} - \langle\hat{x}\rangle\right)dW \right]|\psi\rangle$$

* **Itô Lemma for Quantum Expectation Values:**
  $$d\langle \hat{A} \rangle = \left\langle d\hat{A} \right\rangle + \frac{1}{2}\text{Tr}\left(\mathcal{H}_{\hat{A}} (dX)(dX)^T\right)$$

* **Gardiner-Collett Boundary Condition & Critical Coupling:**
  $$\hat{a}_{\text{out}}(\omega) = \hat{a}_{\text{in}}(\omega) + \sqrt{\kappa_c}\hat{a}(\omega), \quad r(\omega) = \frac{i(\omega - \omega_c) + \frac{\kappa_c - \kappa_i}{2}}{i(\omega - \omega_c) + \frac{\kappa_c + \kappa_i}{2}} \implies r(\omega_c) = 0 \text{ when } \kappa_c = \kappa_i$$

* **Non-Markovian Memory Kernel & Volterra Equation:**
  $$\dot{c}_e(t) = -\int_0^t f(t-t') c_e(t') dt', \quad f(\tau) = \int_0^\infty J(\omega) e^{-i(\omega-\omega_0)\tau} d\omega$$

* **Breuer-Laine-Piilo (BLP) Non-Markovianity Measure:**
  $$\sigma(t) = \frac{d}{dt} D(\rho_1(t), \rho_2(t)), \quad \mathcal{N}_{\text{BLP}} = \int_{\sigma > 0} \sigma(t) \, dt > 0 \iff \lambda < 2\gamma_0$$

* **Scully-Lamb Laser Detailed Balance & Micromaser Trapping Condition:**
  $$P(n) = P(n-1)\frac{A / \kappa}{1 + (B/A)n}, \quad g \tau_{\text{int}}\sqrt{n_q + 1} = q \pi \implies P(n > n_q) \equiv 0$$
