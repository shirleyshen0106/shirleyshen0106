### Shirley Shen

Final-year PhD researcher at **Imperial College London**, working on machine learning for
nonlinear time-series prediction from sparse, noisy experimental data.

Most of what I do sits after the model fits. A good score is easy to produce and easy to
believe; the work is establishing whether it means anything. The repositories here are
small, self-contained demonstrations of that, each built around a result I can defend
rather than a technique I can name.

---

**[leakage-safe-eval](https://github.com/shirleyshen0106/leakage-safe-eval)** &nbsp;·&nbsp; splitting and calibration for data whose rows are not independent

Same data, same model: a random split reports R² = 0.945, an honest one reports 0.667.
Conformal coverage under the leaking split looks healthy at 92% against a nominal 90,
which is the point. Calibration and leakage are independent failure modes, and fixing
one tells you nothing about the other.

**[pinn-objective-ablation](https://github.com/shirleyshen0106/pinn-objective-ablation)** &nbsp;·&nbsp; a multi-term objective taken apart term by term

The physics residual cuts extrapolation error by a factor of 80. The initial-condition
term on its own makes it *worse*, and only earns its place in combination with the
residual. Terms interact, so ablating one at a time is necessary but not sufficient.

**[timeseries-method-landscape](https://github.com/shirleyshen0106/timeseries-method-landscape)** &nbsp;·&nbsp; when does each method family earn its keep

Seventeen families of sequence and dynamical-systems methods, each with its enabling
condition and the concrete case where it fails. Benchmarks age; preconditions do not.

**[polymarket-calibration](https://github.com/shirleyshen0106/polymarket-calibration)** &nbsp;·&nbsp; are market prices calibrated probabilities?

16,759 resolved markets, 36,814 quote–outcome pairs across two tiled weeks. Away from even
odds, prices are too extreme: 5–35% resolve Yes more often than quoted, 65–95% less often.
Withdrawn twice and rebuilt, both times after I found truncation in my own harvester; the
corrections are dated in the README rather than quietly patched.

---

**Publications**

- *Learning rocking dynamics from sparse shake-table data with interpretable
  physics-informed neural networks.* **Earthquake Engineering & Structural Dynamics**,
  2026. [10.1002/eqe.70239](https://doi.org/10.1002/eqe.70239)
- *Physics-informed artificial intelligence models for the seismic response prediction
  of rocking structures.* **Data-Centric Engineering**, 5, 2024.

*Code and the supporting datasets for both papers will be released here after
thesis submission.*

**Tools** &nbsp; Python · PyTorch · TensorFlow · scikit-learn · NumPy · SciPy · pandas · MATLAB
