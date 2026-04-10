# lorenz_ens

Lorenz63 ensemble predictability experiment for ATOC 4815/5815.

## Usage

Without installing:

```bash
python run.py
```
Both generate `lorenz_ensemble_predictability.png`.

After packaging (lab exercise):

```bash
pip install -e .
run-lorenz
```

## Installation

```bash
pip install lorenz-project
```

Or from source:

```bash
git clone https://github.com/chra6227/lorenz-project.git
cd lorenz-project
pip install -e .
```

## Quick Start

```python
from lorenz_project import Lorenz63

model = Lorenz63(sigma=10, rho=28, beta=8/3)
trajectory = model.run([1, 1, 1], dt=0.01, n_steps=5000)
```

## Command Line

```bash
run-lorenz    # generates lorenz_ensemble.png
```

## Files

- `lorenz63.py` — Lorenz63 model class
- `integrators.py` — Forward Euler integrator
- `plotting.py` — Ensemble visualization
- `run_lorenz_ensemble.py` — Driver script

## License

MIT
