[README.md](https://github.com/user-attachments/files/34579456/README.md)
# AIRS reference implementation

Vectorised digital-twin simulator (`dtenv.py`), AIRS and baselines (`agents.py`, `neural.py`), experiment drivers and aggregation.

Requirements: Python 3.10+, numpy, scipy, torch (CPU), matplotlib.

Run everything: `bash run_all.sh` (resumable; results go to `results/`), then `python aggregate.py` (writes `results/stats.json`) and `python figs2.py`.
Individual stages: `run_main.py` (10 seeds), `run_neural.py` (5 seeds), `run_other.py` (ablation, detector, scalability), `timing.py`, `run_iqlteam.py` (IQL-DQN with team reward).
Simulator parameters are listed in Appendix A of the manuscript.
