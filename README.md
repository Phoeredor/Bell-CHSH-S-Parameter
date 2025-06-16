# Bell-CHSH-S-Parameter

A reproducible comparison of CHSH Bell‑inequality measurements on the Bell state |Φ⁺⟩, implemented in three environments using Qiskit  
- Ideal Qiskit Aer (no noise)  
- Noise‑model simulation (FakeWashington)  
- IBM real hardware  

[![MIT License]()](LICENSE)

## 📋 Table of Contents

1. [Overview](#overview)  
2. [Repository Structure](#repository-structure)  
3. [Installation](#installation)  
4. [Usage](#usage)  
5. [Examples of Output](#examples-of-output)  
6. [Acknowledgments](#acknowledgments)  
7. [Contributing](#contributing)  
8. [License](#license)  
9. [Citation](#citation)


## 🔍 Overview

We prepare the Bell state  
\[
  |\Phi^+\rangle = \tfrac{1}{\sqrt2}(|00\rangle + |11\rangle)
\]
apply a rotation \(R_y(\theta)\) on qubit 0, and measure the CHSH witness observables  
\[
  W_1 = Z\otimes Z - Z\otimes X + X\otimes Z + X\otimes X,\quad
  W_2 = Z\otimes Z + Z\otimes X - X\otimes Z + X\otimes X
\]
for \(\theta\in[0,2\pi]\). We extract the maximal \(S\)-parameter for each backend:

| Backend | \(S_{\max}\)     | Mean ± σ      |
|:-------:|:----------------:|:-------------:|
| Ideal   | 2.8274           | 2.528 ± 0.269 |
| Noisy   | 2.4647           | 2.204 ± 0.234 |
| Real    | 2.8645           | 2.525 ± 0.266 |

## 📂 Repository Structure

## ⚙️ Installation

1. **Clone the repository**  
    ```bash
    git clone https://github.com/your-user/bell-chsh-benchmark.git
    cd bell-chsh-benchmark

2. **Set up a virtual enviroment
    ```bash
    python3 -m venv .venv
    source .venv/bin/activate
3. Install dependencies
    ```bash
    pip install -r requirements.txt

---

## 7. Examples of Output  

Show your key plots inline with relative paths:

```markdown
## 📈 Examples of Output

![Ideal Simulator CHSH](figures/AERSIMULATOR_chsh_witness.svg)  
![Noise Simulator CHSH](figures/Noise_chsh_witness.svg)  
![Hardware CHSH](figures/IBM_chsh_witness.svg)







