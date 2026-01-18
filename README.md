# CHSH Bell S-Parameter Test

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/python-3.8%2B-green.svg)]()  

A reproducible implementation of the CHSH Bell‑inequality test on the maximally entangled state |Φ⁺⟩, comparing three environments:

- **Ideal Aer simulator** (noiseless)  
- **Noise‑model (FakeWashington)**  
- **IBM quantum hardware**

## :cd: Quick Start

1. **Clone & enter**  
```bash
   git clone https://github.com/your-user/bell-chsh-benchmark.git
   cd bell-chsh-benchmark
```
2. **Setup**
  ```bash
python3 -m venv .venv

# macOS / Linux
source .venv/bin/activate

# Windows PowerShell
# .\.venv\Scripts\Activate.ps1
  ```
3. **Requirements**
In order to run the notebooks, ensure to have Python ≥ 3.8 and install the requirements
```bash
pip install -r requirements.txt
```
4. **Run**
- Notebook
  ```bash
  jupyter lab notebooks/Real_Hardware_Simulation_CHSH.ipynb
  ```
- Script
  ```bash
  python src/chsh_benchmark.py --backend ideal --shots 100000
  ```
## :chart_with_upwards_trend: Results
| Backend | S<sub>max</sub>  | Mean ± &sigma;|
|:-------:|:----------------:|:-------------:|
| Ideal   | 2.8274           | 2.528 ± 0.269 |
| Noisy   | 2.4647           | 2.204 ± 0.234 |
| Real    | 2.8645           | 2.525 ± 0.266 |

See [Results/](Results/) for plots and circuits gained.
## :handshake: Acknowledgments
   - Base circuits and measurement scheme adapted from the [IBM Quantum Experience documentation](https://learning.quantum.ibm.com/tutorial/chsh-inequality)
   - Portions of code generated with assistence from [ChatGPT](https://openai.com/index/chatgpt/)
## :page_with_curl: License
This project is distributed under the MIT License.  
See [LICENSE](LICENSE) for details.

