# Interactive Digital Circuit Intelligence Notebook
### From CMOS Inverter to Time-Based Logic Systems

**IEEE SSCS Code-a-Chip Competition — VLSI 2026**

---

## Team

| Field | Details |
|---|---|
| Team Name | Matrix Neo |
| Team Lead | Venkatesh K |
| Email | Venkateshk@ieee.org |
| Competition | IEEE SSCS Code-a-Chip — VLSI 2026 |

---

## Description

> This work emphasizes intuition-first circuit understanding through interactive visualization, rather than static simulation outputs.


A simulation-grade, interactive Jupyter notebook modeling the CMOS inverter using a
**nonlinear sigmoid-based Voltage Transfer Characteristic (VTC)**. The notebook extends
from single-device physics to multi-stage logic chains and a full time-based sequential
logic system with D flip-flop behavior, metastability detection, and inverter-delayed
feedback — all with real-time `ipywidgets` parameter control.

---

## Features

- **Nonlinear Inverter Model** — Sigmoid VTC with parametric gain steepness and threshold
- **VTC Visualization** — Transfer curve, unity-gain points, noise margins ($NM_H$, $NM_L$)
- **Instantaneous Gain Plot** — $dV_{out}/dV_{in}$ with peak gain annotation
- **Interactive Sliders** — $V_{DD}$, $V_M$, $k$ (steepness) via `ipywidgets`
- **Signal Propagation Simulation** — Trapezoidal waveform through inverter at configurable frequency
- **Multi-Stage Inverter Chain** — Noise restoration demonstrated across up to 8 stages
- **Time-Based Sequential Logic** — D flip-flop simulation with clock/data at incommensurate frequencies
- **Metastability Detection** — Setup/hold violations highlighted on all waveform panels
- **Inverter-Delayed Feedback** — Sigmoid-modeled propagation delay on Q output
- **Fully Interactive** — All simulations respond to real-time slider input

---

## Repository Structure

```
VLSI26/
└── submitted_notebooks/
    └── CMOS_Inverter_Visualization/
        ├── inverter.ipynb   # Main notebook
        ├── README.md
        └── LICENSE
```

---

## Running the Notebook

**Google Colab (recommended):**

1. Upload `inverter.ipynb` to [colab.research.google.com](https://colab.research.google.com)
2. Runtime → Run all
3. `ipywidgets` installs automatically on first cell execution

**Local:**

```bash
pip install numpy matplotlib ipywidgets notebook
jupyter notebook inverter.ipynb
```

---

## Tools Used

| Tool | Version |
|---|---|
| Python | 3.10+ |
| NumPy | 1.24+ |
| Matplotlib | 3.7+ |
| ipywidgets | 8.x |
| Google Colab | — |

---

## References

- OpenFASOC: https://github.com/idea-fasoc/OpenFASOC
- Google Silicon / OpenLane: https://developers.google.com/silicon/guides/digital-inverter-openlane
- ChipsAlliance Notebooks: https://github.com/chipsalliance/silicon-notebooks

---

## License

Apache License 2.0 — see [LICENSE](./LICENSE)

Copyright 2025 Matrix Neo / Venkatesh K
