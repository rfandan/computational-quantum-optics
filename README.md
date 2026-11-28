# Computational Quantum Optics: From Fundamentals to Frontiers

An open-source, publication-grade, hands-on computational curriculum covering quantum mechanics, quantum optics, cavity QED, open quantum systems, continuous-variable quantum information, and modern quantum optical frontiers through rigorous Python and Google Colab notebooks.

---

## Curriculum Overview

The curriculum is structured into **7 comprehensive modules**, each containing **exactly 10 publication-quality notebooks** (70 notebooks total), rigorously verified with automated unit test suites and zero external black-box quantum library dependencies (developed from first principles using NumPy, SciPy, and Matplotlib).

| Module | Title | Notebooks | Key Topics |
| :--- | :--- | :---: | :--- |
| **Module 0** | [QM Fundamentals & Matrix Mechanics](./module_0_qm_fundamentals/) | **10** | Wavefunctions, Qubits, Bloch Sphere, Commutators, QHO, Time Evolution, Coherent Wavepackets, Angular Momentum & Spin Addition, Variational & Perturbation Theory, Quantum Entanglement & Bell Inequalities |
| **Module 1** | [States of Light](./module_1_states_of_light/) | **10** | Fock, Coherent, Squeezed, Thermal, Cat States, Mandel $Q$, Second-Order Coherence $g^{(2)}(\tau)$, Phase-Squeezed & Number-Squeezed Light, Non-Classicality Depth, Multi-Mode Entangled States |
| **Module 2** | [Phase Space & Quasiprobabilities](./module_2_phase_space_quasiprobabilities/) | **10** | Wigner, Husimi $Q$, Glauber-Sudarshan $P$, Cat Interference Negativity, Quantum State Tomography, Characteristic Functions, Moyal Star Product, Gaussian State Symplectic Invariants, Sub-Planck Phase Space Structures, Cahill-Glauber $s$-Parametrized Quasiprobabilities |
| **Module 3** | [Light-Matter Interaction & Cavity QED](./module_3_light_matter_cavity_qed/) | **10** | Rabi Oscillations, Jaynes-Cummings Model, Dressed States, Vacuum Rabi Splitting, Mollow Triplet, Autler-Townes & EIT, Ultrastrong Coupling & Counter-Rotating Terms, Multi-Atom Dicke Model & Superradiance, Landau-Zener Transitions, Cavity Photon Statistics Under Atomic Drive |
| **Module 4** | [Open Quantum Systems & Dissipation](./module_4_open_systems_dissipation/) | **10** | Density Matrices & Purity, Microscopic Born-Markov Master Equation, Lindblad Form, Cavity Decay & Photon Loss, Monte Carlo Wavefunction (MCWF) Jumps, Quantum Trajectories & Homodyne Detection, Stochastic Calculus (Itô vs Stratonovich), Input-Output Theory & Scattering, Non-Markovian Memory Dynamics & Spectral Densities, Laser Theory & Micromaser Phase Transitions |
| **Module 5** | [Multi-Mode & Quantum Information](./module_5_multimode_quantum_information/) | **10** | Quantum Beam Splitter, Hong-Ou-Mandel Interference, Mach-Zehnder & Multiport Unitary Meshes (Reck/Clements), Two-Mode Squeezing & EPR Entanglement, Continuous-Variable Quantum Teleportation, Gaussian States & Symplectic Operations, CV-QKD (GG02 Protocol & Holevo Bound), Measurement-Based Quantum Computing on CV Clusters, Quantum State Engineering & Photon Subtraction, Linear Optical Quantum Computing & Boson Sampling |
| **Module 6** | [Advanced Frontiers in Quantum Optics](./module_6_advanced_frontiers/) | **10** | Cavity Optomechanics & Radiation Pressure, Quantum Metrology & Heisenberg Scaling, Non-Hermitian Optics & Exceptional Points, Circuit QED & Transmon Qubits, Photon Blockade & Non-Linear Optics, Chiral & Waveguide QED, Topological Quantum Photonics (SSH Model), Bosonic QEC (GKP & Cat Codes), Quantum Reservoir Engineering & Cat Qubits, Optimal Quantum Control & GRAPE Algorithm |
| **Total** | **All 7 Modules** | **70** | **70 Comprehensive Notebooks • 350 Automated Unit Tests • Full First-Principles Implementations** |

---

## Detailed Module Syllabi

### [Module 0: Quantum Mechanics Fundamentals & Matrix Mechanics](./module_0_qm_fundamentals/)
* `01_wavefunctions_and_schrodinger_equation.ipynb`: Position/momentum wavepackets, finite-difference kinetic energy operator, spatial dispersion $\sigma_x(t) = \sigma_0\sqrt{1 + (t/\tau)^2}$.
* `02_qubits_and_bloch_sphere.ipynb`: Pure states, mixed state density matrices, Pauli algebra, Bloch sphere geodesic trajectories.
* `03_operators_and_commutators.ipynb`: Non-commuting observable algebras, Robertson-Schrödinger uncertainty relation $\Delta A \Delta B \ge \frac{1}{2}|\langle[A, B]\rangle|$.
* `04_quantum_harmonic_oscillator.ipynb`: Ladder operator calculus $[\hat{a}, \hat{a}^\dagger] = 1$, Hermite-Gauss stationary eigenfunctions, Fock basis representation.
* `05_time_evolution_and_unitary_operators.ipynb`: Unitary evolution operators $\hat{U}(t) = \exp(-i\hat{H}t/\hbar)$, split-operator Trotter propagation, norm preservation.
* `06_coherent_wavepackets_and_ Ehrenfest_theorem.ipynb`: Minimum uncertainty wavepacket dynamics, harmonic restoration, Ehrenfest expectation value matching.
* `07_angular_momentum_and_spin_addition.ipynb`: $SU(2)$ angular momentum algebra, Clebsch-Gordan coefficients, singlet and triplet spin coupling.
* `08_variational_method_and_perturbation_theory.ipynb`: Rayleigh-Ritz variational optimization, Rayleigh-Schrödinger non-degenerate and degenerate perturbation theory.
* `09_quantum_entanglement_and_bell_inequalities.ipynb`: Density matrix partial trace, Schmidt decomposition, von Neumann entropy, CHSH inequality violation ($S = 2\sqrt{2} > 2$).
* `10_numerical_matrix_diagonalization_and_sparse_methods.ipynb`: Dense and sparse Hamiltonian matrix diagonalization (SciPy `eigsh`), Krylov subspace methods, convergence benchmarking.

### [Module 1: Single-Mode and Multi-Mode Quantum States of Light](./module_1_states_of_light/)
* `01_fock_states_and_photon_number.ipynb`: Exact discrete photon number states $|n\rangle$, orthogonal projection, sub-Poissonian variance $\Delta n^2 = 0$.
* `02_coherent_states_and_poissonian_statistics.ipynb`: Displaced vacuum $|\alpha\rangle = \hat{D}(\alpha)|0\rangle$, Poissonian statistics $P(n) = e^{-|\alpha|^2}|\alpha|^{2n}/n!$, shot-noise limit.
* `03_squeezed_states_and_quadrature_noise.ipynb`: Single-mode squeeze operator $\hat{S}(\xi) = \exp[\frac{1}{2}(\xi^* \hat{a}^2 - \xi \hat{a}^{\dagger 2})]$, sub-shot-noise quadrature variance $\Delta X_1^2 = \frac{1}{4}e^{-2r}$.
* `04_thermal_states_and_bose_einstein_distribution.ipynb`: Maximum-entropy Gibbs thermal states $\hat{\rho}_{\text{th}}$, geometric photon distribution, super-Poissonian noise $g^{(2)}(0) = 2$.
* `05_schrodinger_cat_states.ipynb`: Even, odd, and Yurke-Stoler macroscopic superpositions $|\mathcal{C}_\alpha^\pm\rangle \propto |\alpha\rangle \pm |-\alpha\rangle$, parity operator $\langle\hat{\Pi}\rangle = \pm 1$.
* `06_mandel_q_parameter_and_photon_statistics.ipynb`: Mandel $Q = (\Delta n^2 - \langle n \rangle)/\langle n \rangle$ diagnostic for sub-Poissonian ($Q < 0$), Poissonian ($Q = 0$), and super-Poissonian ($Q > 0$) light.
* `07_second_order_coherence_g2.ipynb`: Hanbury Brown-Twiss intensity correlation $g^{(2)}(\tau)$, photon antibunching ($g^{(2)}(0) < 1$), bunching, and chaotic fluctuations.
* `08_phase_squeezed_vs_number_squeezed_light.ipynb`: Amplitude vs. phase quadrature trade-offs, crescent-shaped phase-space distributions, Pegg-Barnett phase formalism.
* `09_nonclassicality_depth_and_operational_criteria.ipynb`: Lee's non-classicality depth $\tau_m$, operational criteria (Hillery, Agarwal-Tara), convolution filtering of singular distributions.
* `10_multimode_entangled_states.ipynb`: Multi-mode Gaussian and non-Gaussian states, covariance matrices, Peres-Horodecki partial transposition (PPT criterion).

### [Module 2: Phase Space & Quasiprobability Distributions](./module_2_phase_space_quasiprobabilities/)
* `01_wigner_function_fundamentals.ipynb`: Symmetrically ordered Weyl-Wigner transform, real-valued phase space representation, marginal integration properties.
* `02_husimi_q_distribution.ipynb`: Anti-normally ordered projection $Q(\alpha) = \frac{1}{\pi}\langle\alpha|\hat{\rho}|\alpha\rangle$, strictly non-negative phase-space representation.
* `03_glauber_sudarshan_p_representation.ipynb`: Normally ordered expansion $\hat{\rho} = \int P(\alpha)|\alpha\rangle\langle\alpha| d^2\alpha$, tempered distribution singularities for quantum states.
* `04_wigner_negativity_and_nonclassicality.ipynb`: Kenfack-Życzkowski negativity volume $\delta(\hat{\rho}) = \int (|W| - W) dx dp$, Hudson's theorem (Gaussian positivity).
* `05_quantum_state_tomography.ipynb`: Radon transform inversion, maximum likelihood estimation (MLE) reconstruction from homodyne quadrature marginals.
* `06_characteristic_functions_in_phase_space.ipynb`: Symmetric, normal, and anti-normal characteristic functions $\chi(\eta)$, 2D symplectic Fourier transforms.
* `07_moyal_bracket_and_phase_space_dynamics.ipynb`: Moyal star product $A \star B$, phase-space time evolution equation $\partial_t W = -\{\{H, W\}\}_{\text{Moyal}}$, quantum corrections to Liouville dynamics.
* `08_symplectic_geometry_and_gaussian_phase_space.ipynb`: $2N \times 2N$ real symplectic matrices $S \in Sp(2N, \mathbb{R})$, Williamson's theorem, symplectic spectrum $\nu_k \ge 1/2$.
* `09_sub_planck_structures_in_phase_space.ipynb`: Zurek phase-space compass states, interference oscillations at scale $a_{\text{sub}} \sim \hbar^2 / \Delta x \Delta p \ll \hbar$, hyper-sensitivity to phase perturbations.
* `10_cahill_glauber_s_parametrized_quasiprobabilities.ipynb`: Continuous parameter $s \in [-1, 1]$ bridging $P$ ($s=1$), $W$ ($s=0$), and $Q$ ($s=-1$), smoothing kernels and singularities.

### [Module 3: Light-Matter Interaction & Cavity QED](./module_3_light_matter_cavity_qed/)
* `01_semiclassical_rabi_oscillations.ipynb`: Two-level atomic dipoles in classical monochromatic electromagnetic fields, generalized Rabi frequency $\Omega_{\text{eff}} = \sqrt{\Omega^2 + \Delta^2}$.
* `02_jaynes_cummings_model.ipynb`: Fully quantized atom-cavity Hamiltonian $\hat{H}_{\text{JC}} = \hbar\omega_c \hat{a}^\dagger\hat{a} + \frac{1}{2}\hbar\omega_a \hat{\sigma}_z + \hbar g(\hat{a}\hat{\sigma}_+ + \hat{a}^\dagger\hat{\sigma}_-)$, exact block diagonalization.
* `03_dressed_states_and_eigenvalues.ipynb`: Jaynes-Cummings ladder eigenstates $|n, \pm\rangle$, photon-number-dependent splitting $\Delta E_n = 2\hbar g\sqrt{n}$, non-linear energy spectrum.
* `04_vacuum_rabi_splitting.ipynb`: Resonant strong coupling $g > (\kappa, \gamma)$, transmission doublet $\omega_c \pm g$, coherent atom-cavity excitation exchange.
* `05_mollow_triplet_and_resonance_fluorescence.ipynb`: Power-broadened strongly driven two-level fluorescence spectrum, central Rayleigh peak flanked by sidebands at $\omega_L \pm \Omega$.
* `06_autler_townes_splitting_and_eit.ipynb`: Three-level $\Lambda$-systems, coherent population trapping (CPT), Electromagnetically Induced Transparency (EIT), ultra-slow light group velocity.
* `07_ultrastrong_coupling_and_counter_rotating_terms.ipynb`: Rabi Hamiltonian without RWA ($g/\omega_c \gtrsim 0.1$), virtual photon dressing of the vacuum ground state, parity symmetry breaking.
* `08_dicke_model_and_superradiance.ipynb`: Ensemble of $N$ identical emitters coupled to a single cavity mode, cooperative decay rate $\Gamma_{\text{super}} \sim N\gamma_0$, Dicke superradiant quantum phase transition.
* `09_landau_zener_transitions_in_cavity_qed.ipynb`: Non-adiabatic passage through avoided level crossings, Landau-Zener transition probability $P_{\text{LZ}} = \exp(-2\pi g^2 / v)$, sweep rate scaling.
* `10_cavity_photon_statistics_under_atomic_drive.ipynb`: Driven dissipative atom-cavity systems, non-linear photon transmission, single-atom optical bistability and hysteresis.

### [Module 4: Open Quantum Systems, Dissipation & Measurement](./module_4_open_systems_dissipation/)
* `01_density_matrix_and_purity.ipynb`: Statistical mixtures, purity $\gamma = \mathrm{Tr}(\rho^2) \le 1$, von Neumann entropy $\mathcal{S}(\rho) = -\mathrm{Tr}(\rho \ln \rho)$, Bloch sphere representation.
* `02_microscopic_derivation_of_master_equations.ipynb`: System-bath coupling, Born-Markov approximation, secular rotating wave approximation, transition rate tensor.
* `03_lindblad_master_equation.ipynb`: Complete positivity preserving generators $\dot{\rho} = -i[H, \rho] + \sum_k \gamma_k \mathcal{D}[L_k]\rho$, Liouvillian superoperator spectrum, relaxation rates.
* `04_cavity_decay_and_photon_loss.ipynb`: Lindblad jump operator $\hat{a}$ with rate $\kappa$, exponential photon decay $\langle n(t) \rangle = n_0 e^{-\kappa t}$, decoherence of Schrödinger cat superpositions.
* `05_monte_carlo_wavefunction_method.ipynb`: Stochastic quantum jump method, non-Hermitian effective Hamiltonian $\hat{H}_{\text{eff}} = \hat{H} - \frac{i\hbar}{2}\sum_k L_k^\dagger L_k$, random quantum jumps.
* `06_quantum_trajectories_and_homodyne_measurement.ipynb`: Continuous measurement backaction, stochastic Schrödinger equation (SSE), homodyne photocurrent $I(t) = \langle\hat{x}\rangle + \frac{dW}{\sqrt{8\kappa}dt}$.
* `07_stochastic_calculus_ito_vs_stratonovich.ipynb`: Wiener processes ($dW^2 = dt$), Itô's lemma, Stratonovich drift correction, numerical Euler-Maruyama and Milstein integrators.
* `08_input_output_theory_and_cavity_scattering.ipynb`: Gardiner-Collett boundary condition $\hat{a}_{\text{out}}(t) = \hat{a}_{\text{in}}(t) + \sqrt{\kappa}\hat{a}(t)$, cavity reflection/transmission spectra, phase response.
* `09_non_markovian_dynamics_and_spectral_densities.ipynb`: Structured baths, Lorentzian and Ohm spectral densities, Volterra integro-differential memory equations, canonical negative decay rates $\gamma(t) < 0$, BLP non-Markovianity measure.
* `10_laser_theory_and_micromaser.ipynb`: Scully-Lamb master equation, threshold inversion pump parameter, Poisson-to-sub-Poissonian statistics, trapping states in micromaser cavity.

### [Module 5: Multi-Mode Quantum Optics & Quantum Information](./module_5_multimode_quantum_information/)
* `01_quantum_beam_splitter.ipynb`: $SU(2)$ unitary transformation $\hat{U}_{\text{BS}} = \exp[\frac{\theta}{2}(\hat{a}^\dagger\hat{b} - \hat{a}\hat{b}^\dagger)]$, Casimir invariants, input-output mode transformations.
* `02_hong_ou_mandel_interference.ipynb`: Two-photon quantum interference, destructive path amplitude cancellation, HOM dip with $100\%$ visibility for indistinguishable photons.
* `03_mach_zehnder_and_multiport_interferometers.ipynb`: MZI phase estimation, Standard Quantum Limit vs. Heisenberg scaling, NOON state super-resolution $\cos(N\phi)$, universal multiport unitary mesh decomposition (Reck/Clements Givens nulling).
* `04_two_mode_squeezing_and_epr_states.ipynb`: Two-mode squeeze operator $\hat{S}_2(\xi) = \exp(\xi^*\hat{a}\hat{b} - \xi\hat{a}^\dagger\hat{b}^\dagger)$, continuous-variable Einstein-Podolsky-Rosen (EPR) entanglement, Duan inseparability criterion.
* `05_continuous_variable_quantum_teleportation.ipynb`: Braunstein-Kimble protocol, dual homodyne Bell-state measurement, feedforward displacement $\hat{D}(g\beta)$, teleportation fidelity surpassing classical limit $F > 1/2$.
* `06_gaussian_states_and_symplectic_operations.ipynb`: $2N \times 2N$ covariance matrices, symplectic transformations $S \in Sp(2N, \mathbb{R})$, Williamson normal forms, logarithmic negativity entanglement.
* `07_cv_quantum_key_distribution_gg02.ipynb`: Grosshans-Grangier 2002 (GG02) Gaussian-modulated coherent state QKD, shot-noise homodyne detection, collective eavesdropping Holevo bound $\chi_{BE}$, reverse reconciliation exceeding 3 dB loss limit.
* `08_measurement_based_quantum_computing_cv_clusters.ipynb`: Continuous-variable graph and cluster states, adjacency matrices $A$, nullifier squeezing $\Delta\hat{\delta}_a^2 \to 0$, $C_Z$ symplectic gates, 1D cluster state gate teleportation.
* `09_quantum_state_engineering_and_photon_subtraction.ipynb`: Non-Gaussian state engineering via photon subtraction $\hat{a}|\text{TMSV}\rangle$, Wigner negativity generation, entanglement distillation, Schrödinger kitten state synthesis.
* `10_linear_optical_quantum_computing_and_boson_sampling.ipynb`: KLM scheme, permanent of submatrices $\mathrm{Perm}(U_{s,t})$, Aaronson-Arkhipov Boson Sampling, Gurvits algorithm, computational quantum advantage.

### [Module 6: Advanced Frontiers in Quantum Optics](./module_6_advanced_frontiers/)
* `01_cavity_optomechanics_and_radiation_pressure.ipynb`: Radiation pressure Hamiltonian $\hat{H}_{\text{int}} = -\hbar g_0 \hat{a}^\dagger\hat{a}(\hat{b} + \hat{b}^\dagger)$, dynamical backaction, red sideband resolved ground-state cooling, Optomechanically Induced Transparency (OMIT).
* `02_quantum_sensing_and_heisenberg_limit.ipynb`: Quantum Fisher Information (QFI) $\mathcal{F}_Q$, quantum Cramér-Rao bound $\Delta\theta \ge 1/\sqrt{\nu \mathcal{F}_Q}$, NOON state Heisenberg scaling $\Delta\theta = 1/N$, squeezed vacuum dark-port injection (LIGO architecture).
* `03_non_hermitian_optics_and_exceptional_points.ipynb`: $\mathcal{PT}$-symmetric dimers, unbroken vs. broken phases, Exceptional Points (EPs) with simultaneous eigenvalue and eigenvector coalescence, square-root Puiseux perturbation sensitivity $\Delta\lambda \propto \sqrt{\epsilon}$, Petermann noise factor divergence.
* `04_circuit_qed_and_transmon_qubits.ipynb`: Cooper Pair Box Hamiltonian, transmon flat-band engineering ($E_J/E_C = 50$), exponential charge noise suppression, negative Duffing anharmonicity, dispersive readout and photon-number resolving spectroscopy.
* `05_photon_blockade_and_quantum_nonlinear_optics.ipynb`: Kerr non-linearity $\hat{H}_{\text{Kerr}} = \hbar \chi (\hat{a}^\dagger)^2 \hat{a}^2$, conventional vs. unconventional photon blockade, steady-state Liouvillian solver, strong antibunching $g^{(2)}(0) < 0.05$ at $U = 5\kappa$.
* `06_chiral_and_waveguide_quantum_electrodynamics.ipynb`: Spin-momentum locking, directional decay rates $\gamma_R, \gamma_L$, vanishing reflection $r \equiv 0$, non-reciprocal $\pi$ phase shift, Gardiner-Carmichael cascaded master equation with strictly unidirectional energy transfer.
* `07_topological_quantum_photonics.ipynb`: 1D Su-Schrieffer-Heeger (SSH) photonic lattice, intra/inter-cell hopping dimerisation, chiral sublattice symmetry, bulk winding number $\mathcal{W}$, zero-energy topological boundary edge modes, robust disorder localization.
* `08_bosonic_quantum_error_correction_gkp_and_cat_codes.ipynb`: Hardware-efficient cvQEC in a single bosonic mode, Knill-Laflamme conditions, 2-legged and 4-legged Schrödinger cat codes, parity jump syndrome extraction ($\hat{\Pi} \to -\hat{\Pi}$), finite-energy GKP grid states.
* `09_quantum_reservoir_engineering_and_dissipative_stabilization.ipynb`: Autonomous state preparation via non-linear baths, two-photon driven dissipator $\kappa_2 \mathcal{D}[\hat{a}^2 - \alpha^2]$, cat qubit dark manifold, exponential bit-flip error suppression $\Gamma_X \propto e^{-2|\alpha|^2}$ ($> 900\times$), Wigner interference negativity.
* `10_optimal_control_and_grape_algorithm.ipynb`: Quantum optimal control on Lie group $SU(d)$, Gradient Ascent Pulse Engineering (GRAPE), exact analytical forward-backward gradients without finite differences, high-fidelity gate synthesis ($\mathcal{F} > 99.99\%$), Quantum Speed Limit (QSL).

---

## Architectural & Pedagogical Standards

Every notebook adheres to a strict **10-cell structural architecture**:

```
Cell 1: [Markdown] Rigorous theoretical exposition, formal operator definitions, and physics context
Cell 2: [Code]     Headless, reproducible imports (NumPy, SciPy, Matplotlib) & numerical configuration
Cell 3: [Markdown] Mathematical derivation of the target problem, analytical bounds, and equations
Cell 4: [Code]     Object-oriented computational engine implementing first-principles physics algorithms
Cell 5: [Code]     Publication-grade 4-panel Matplotlib visualization (300 DPI, academic styling)
Cell 6: [Markdown] In-depth physical interpretation connecting computational features to physical theory
Cell 7: [Code]     Interactive parameter diagnostics suite and sensitivity analysis
Cell 8: [Markdown] Quantitative acceptance criteria and rigorous numerical validation thresholds
Cell 9: [Code]     Automated 5-test unit test suite verifying physical invariants, norms, and bounds
Cell 10: [Code]    Clean ASCII execution and verification summary table
```

### Key Technical Guarantees
1. **Zero External Black-Box Dependencies:** No proprietary quantum frameworks are required. All quantum mechanical simulations (diagonalizations, matrix exponentials, master equations, Wigner integrals, symplectic transformations) are constructed directly from scratch in standard NumPy and SciPy.
2. **Automated Unit Testing:** Every single notebook contains an automated 5-test unit test suite (350 automated unit tests across the entire curriculum), asserting exact quantum mechanical invariants (unitary norm preservation, Hermiticity, trace preservation, positive semidefiniteness, parity invariance, uncertainty relations).
3. **Publication-Ready Figures:** Every notebook automatically generates high-resolution 4-panel figures at 300 DPI saved directly to disk.

---

## Getting Started

### Local Setup
Clone this repository and install dependencies:
```bash
git clone https://github.com/<your-username>/computational-quantum-optics.git
cd computational-quantum-optics
pip install -r requirements.txt
```

### Dependencies (`requirements.txt`)
- `numpy >= 1.24.0` (fully compatible with NumPy 2.x)
- `scipy >= 1.10.0`
- `matplotlib >= 3.7.0`
- `jupyter >= 1.0.0`
- `nbformat >= 5.9.0`

### Running Notebooks
Launch Jupyter Notebook or JupyterLab:
```bash
jupyter lab
```
Navigate to any module (`module_0_qm_fundamentals` through `module_6_advanced_frontiers`) and open any `.ipynb` file. All notebooks run out-of-the-box in sequential execution mode.

---

## License
This project is licensed under the MIT License — see the [LICENSE](./LICENSE) file for details.
