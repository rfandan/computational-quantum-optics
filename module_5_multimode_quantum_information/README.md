# Module 5: Multi-Mode Quantum Optics & Quantum Information

This module covers the core principles, state representations, and physical protocols of **Multi-Mode Quantum Optics** and optical **Quantum Information Processing**. It bridges linear optical interference—from single-mode and dual-mode beam splitters to multiport unitary network decompositions—with continuous-variable (CV) entanglement, symplectic Gaussian transformations, discrete-variable and continuous-variable quantum teleportation, CV quantum key distribution (GG02), measurement-based cluster state quantum computing (MBQC), non-Gaussian state engineering via photon subtraction, and #P-hard computational advantage via Boson Sampling.

---

### Notebook Syllabus (10/10 Complete)

| # | Notebook | Core Topics |
| :-: | :--- | :--- |
| **01** | [`01_quantum_beam_splitter.ipynb`](./01_quantum_beam_splitter.ipynb) | Canonical quantization of two-mode spatial mixing, $SU(2)$ Lie algebra representations (Schwinger boson mapping $\hat{J}_x, \hat{J}_y, \hat{J}_z$), unitary scattering operator $\hat{U}_{\text{BS}}(\theta, \phi) = \exp[-i\theta(\hat{a}_1^\dagger\hat{a}_2 e^{i\phi} + \hat{a}_1\hat{a}_2^\dagger e^{-i\phi})]$, single-photon routing, coherent state splitting $|\alpha\rangle|0\rangle \to |t\alpha\rangle|r\alpha\rangle$, and two-mode quadrature transformation. |
| **02** | [`02_hong_ou_mandel_interference.ipynb`](./02_hong_ou_mandel_interference.ipynb) | Two-photon quantum interference, destructive quantum interference of probability amplitudes $(rt + tr = 0)$, suppression of coincidence counts $P(1,1) = 0$, generation of NOON states $(|2,0\rangle + |0,2\rangle)/\sqrt{2}$, temporal wavepacket overlap, visibility $V = (R_{\text{max}} - R_{\text{min}})/R_{\text{max}}$, distinguishability via polarization, frequency detuning, and spatial mismatch. |
| **03** | [`03_mach_zehnder_and_multiport_interferometers.ipynb`](./03_mach_zehnder_and_multiport_interferometers.ipynb) | Mach-Zehnder Interferometry (MZI), quantum metrology, Standard Quantum Limit (SQL: $\Delta\phi \sim 1/\sqrt{N}$) vs. Heisenberg Limit (HL: $\Delta\phi \sim 1/N$), Quantum Fisher Information $\mathcal{F}_Q$, NOON state super-resolving fringes $\propto \cos^2(N\phi/2)$, and Reck/Clements multiport unitary mesh decomposition synthesizing arbitrary $U \in U(N)$ with $N(N-1)/2$ beam splitters. |
| **04** | [`04_two_mode_squeezing_and_epr_states.ipynb`](./04_two_mode_squeezing_and_epr_states.ipynb) | Non-degenerate parametric down-conversion (SPDC Type-II), Hamiltonian $\hat{H}_{\text{int}} = i\hbar \kappa (\hat{a}_1^\dagger\hat{a}_2^\dagger - \hat{a}_1\hat{a}_2)$, Two-Mode Squeezed Vacuum (TMSV) state $|\text{TMSV}\rangle = \sqrt{1-\tanh^2 r}\sum_n \tanh^n r |n, n\rangle$, inter-mode photon number correlations, Einstein-Podolsky-Rosen (EPR) paradox, Duan-Giedke-Cirac-Zoller (DGCZ) inseparability criterion $\Delta(\hat{x}_1 - \hat{x}_2)^2 + \Delta(\hat{p}_1 + \hat{p}_2)^2 = 2e^{-2r} < 2$, and thermal reduced state entropy. |
| **05** | [`05_continuous_variable_quantum_teleportation.ipynb`](./05_continuous_variable_quantum_teleportation.ipynb) | Continuous-variable Braunstein-Kimble protocol, dual-homodyne Bell-state measurement, classical feedforward displacement $\hat{D}(\beta)$, teleportation of non-orthogonal coherent states, finite-squeezing fidelity $F(r) = 1/(1 + e^{-2r})$, classical teleportation boundary $F_{\text{class}} = 1/2$, and quantum entanglement benchmark $F > 2/3$. |
| **06** | [`06_gaussian_states_and_symplectic_operations.ipynb`](./06_gaussian_states_and_symplectic_operations.ipynb) | Phase-space continuous variables, displacement vector $\mathbf{d}$ and $2N \times 2N$ symmetric covariance matrix $\mathbf{\sigma}$, symplectic group $Sp(2N, \mathbb{R})$, Williamson's theorem and symplectic diagonalization $\mathbf{\sigma} = S \mathbf{\nu} S^T$, Heisenberg-Robertson uncertainty relation $\mathbf{\sigma} + \frac{i}{2}\Omega \ge 0$, partial transpose criterion (PPT / Simon's criterion), logarithmic negativity $E_N = \max(0, -\ln(2\tilde{\nu}_-))$, and multi-mode Gaussian states. |
| **07** | [`07_cv_quantum_key_distribution_gg02.ipynb`](./07_cv_quantum_key_distribution_gg02.ipynb) | Grosshans-Grangier 2002 (GG02) Gaussian-modulated coherent state QKD, shot-noise-limited balanced homodyne detection, fiber loss and excess noise modeling, collective Gaussian eavesdropping attacks, reverse reconciliation overcoming the $3\text{ dB}$ loss limit, Holevo information bound $\chi_{BE}$, and asymptotic secret key rate $K = \max(0, \beta I_{AB} - \chi_{BE})$ past $50\text{ km}$. |
| **08** | [`08_measurement_based_quantum_computing_cv_clusters.ipynb`](./08_measurement_based_quantum_computing_cv_clusters.ipynb) | Continuous-variable cluster states and graph states, graph adjacency matrix $A$, entanglement nullifiers $\hat{\delta}_j = \hat{p}_j - \sum_k A_{jk}\hat{x}_k \to 0$, exponential nullifier variance suppression $\Delta\hat{\delta}^2 = \frac{1}{2}e^{-2r}$, Controlled-Phase entangling symplectic transformations, 1D cluster state gate teleportation, finite-squeezing Gaussian noise accumulation, and GKP fault-tolerance threshold. |
| **09** | [`09_quantum_state_engineering_and_photon_subtraction.ipynb`](./09_quantum_state_engineering_and_photon_subtraction.ipynb) | Non-Gaussian state generation, conditional measurement / heraldings, photon subtraction $\hat{a}|\psi\rangle$, creation of high-fidelity Schrödinger kitten states from squeezed vacuum, Wigner function negativity at the origin $W(0,0) < 0$, photon addition $\hat{a}^\dagger|\psi\rangle$, non-Gaussianity measures (relative entropy of non-Gaussianity), and quantum error-correction resource preparation. |
| **10** | [`10_linear_optical_quantum_computing_and_boson_sampling.ipynb`](./10_linear_optical_quantum_computing_and_boson_sampling.ipynb) | The Knill-Laflamme-Milburn (KLM) theorem, non-linear sign (NS) shift gate using ancilla photons, Aaronson-Arkhipov Boson Sampling, permanent of submatrices $\text{Perm}(U_{S,T})$, computational complexity hierarchy (#P-hard permanent vs $\mathcal{O}(N^3)$ classical determinant), Ryser and Glynn algorithms, validation tests against mean-field distinguishable bosons, and quantum computational supremacy. |

---

### Key Formulas & Physical Principles

* **Beam Splitter $SU(2)$ Schwinger Representation:**
  $$\hat{J}_x = \frac{\hat{a}_1^\dagger\hat{a}_2 + \hat{a}_2^\dagger\hat{a}_1}{2}, \quad \hat{J}_y = \frac{\hat{a}_1^\dagger\hat{a}_2 - \hat{a}_2^\dagger\hat{a}_1}{2i}, \quad \hat{J}_z = \frac{\hat{a}_1^\dagger\hat{a}_1 - \hat{a}_2^\dagger\hat{a}_2}{2}, \quad \hat{U}_{\text{BS}} = \exp\left[-2i\theta\left(\hat{J}_x \cos\phi - \hat{J}_y \sin\phi\right)\right]$$

* **Hong-Ou-Mandel Dip Visibility:**
  $$P(1,1; \delta\tau) = \frac{1}{2}\left(1 - V_{\text{HOM}} e^{-(\delta\tau / \tau_{\text{coh}})^2}\right), \quad V_{\text{HOM}} = \frac{R_{\text{max}} - R_{\text{min}}}{R_{\text{max}}} = 1.0 \text{ (Identical photons)}$$

* **Quantum Fisher Information & Heisenberg Limit:**
  $$\mathcal{F}_Q(\text{NOON}) = N^2 \implies \Delta\phi_{\text{HL}} = \frac{1}{N}, \qquad \mathcal{F}_Q(\text{Coherent}) = N \implies \Delta\phi_{\text{SQL}} = \frac{1}{\sqrt{N}}$$

* **Reck/Clements Universal Multiport Unitary Decomposition:**
  $$U \in U(N) \implies U = \left( \prod_{k=1}^{N(N-1)/2} T_{p_k, q_k}^\dagger \right) \text{diag}(e^{i\varphi_1}, \dots, e^{i\varphi_N})$$

* **Duan Inseparability Criterion (EPR / TMSV):**
  $$\Delta(\hat{x}_1 - \hat{x}_2)^2 + \Delta(\hat{p}_1 + \hat{p}_2)^2 = 2 e^{-2r} < 2 \implies \text{Inseparable (Entangled)}$$

* **Braunstein-Kimble CV Teleportation Fidelity:**
  $$F(r) = \frac{1}{1 + e^{-2r}}, \quad F(0) = \frac{1}{2} \text{ (Classical)}, \quad F(r) > \frac{2}{3} \implies \text{Quantum Benchmarking}$$

* **Williamson's Theorem & Simon's PPT Entanglement Criterion:**
  $$\mathbf{\sigma} = S \text{diag}(\nu_1, \nu_1, \dots, \nu_N, \nu_N) S^T, \quad \tilde{\nu}_- < \frac{1}{2} \iff \text{Bipartite Entangled}$$

* **GG02 CV-QKD Secret Key Rate (Reverse Reconciliation):**
  $$K_{\text{rev}} = \max\left(0, \beta I_{AB} - \chi_{BE}\right), \quad \chi_{BE} = S(\rho_{AB}) - S(\rho_{A|x_B})$$

* **Continuous-Variable Cluster State Nullifiers:**
  $$\hat{\delta}_j = \hat{p}_j - \sum_{k \in \mathcal{N}(j)} A_{jk}\hat{x}_k, \quad \langle \hat{\delta}_j^2 \rangle = \frac{1}{2}e^{-2r} \xrightarrow{r \to \infty} 0$$

* **Aaronson-Arkhipov Boson Sampling Transition Amplitude:**
  $$\langle s_1, \dots, s_M | \hat{U} | t_1, \dots, t_M \rangle = \frac{\text{Perm}(U_{s,t})}{\sqrt{s_1!\dots s_M! t_1!\dots t_M!}}$$
