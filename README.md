# BrainModeling_project
Investigation of Stochastic Resonance in a Leaky Integrate-and-Fire neuron under subthreshold sinusoidal input. Analysis of noise-induced spike-signal synchronization using Vector Strength and population-level robustness.

# Stochastic-Resonance-LIF
Brain Modeling project investigating **Stochastic Resonance** in a **Leaky Integrate-and-Fire (LIF) neuron**, analyzing how noise influences spike–signal synchronization at both single-neuron and population levels.


## Stochastic Resonance in a LIF Neuron
- **Language:** Python  
- **Libraries:**  
  - **Scientific Computing:** numpy, scipy  
  - **Visualization:** matplotlib  
  - **Utilities:** tqdm  


## Overview  
This project studies how **Gaussian white noise** can enhance the detection of a weak subthreshold sinusoidal input in a nonlinear threshold system.  

Using a **Leaky Integrate-and-Fire (LIF) model**, we investigate whether an intermediate noise intensity maximizes spike–signal synchronization, a phenomenon known as **Stochastic Resonance (SR)**.

The analysis is performed at:
1. **Single-neuron level**, using phase-locking metrics.  
2. **Population level**, pooling independent neurons to assess robustness of temporal encoding.


## Model and Methodology  
- **Neuron Model:** Leaky Integrate-and-Fire with fixed threshold and reset.  
- **Input Current:** Subthreshold sinusoidal signal with adjustable amplitude and DC bias.  
- **Noise:** Gaussian white noise added to the input current.  
- **Numerical Integration:** Euler–Maruyama scheme.  
- **Synchronization Metric:** Vector Strength computed from spike phases.  

Parameter sweeps were performed to test:
- Optimal noise intensity (σ_opt)  
- Dependence on signal amplitude  
- Dependence on bias current  
- High-noise degradation effects  
- Population-level robustness (N = 50 neurons)


## Results and Insights  
- Spike–signal synchronization exhibits a **non-monotonic dependence on noise intensity**, confirming the existence of an optimal σ.  
- Increasing signal amplitude or bias current shifts the optimal noise level toward lower values.  
- Excessive noise increases firing rate but **degrades temporal precision**.  
- Population pooling stabilizes temporal signal representation despite single-neuron variability.  

The results highlight a dissociation between **firing rate** and **temporal coding precision**.


## View the Full Notebook  
You can explore the complete notebook directly in this repository:  
`BrainModeling_project.ipynb`  

For a static preview:  
[Open in nbviewer](https://nbviewer.org/github/BeatriceCamera/stochastic-resonance-lif/blob/main/BrainModeling_project.ipynb)


## Authors  
Beatrice Camera  
Irene Marrali  
Sabina Gallo  

B.Sc. Artificial Intelligence @ University of Pavia, University of Milan, University of Milano-Bicocca  
