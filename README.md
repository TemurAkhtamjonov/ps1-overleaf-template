# Commitment Bonds and Calibrated Trust

COMSCI/ECON 206 PS1 research proposal by Temur Akhtamjonov.

This repository contains the submitted Overleaf source, the editable teaser figure, a reproducible Python/Colab benchmark, and the source of the interactive teaching demo.

## Question

When does an AI receiver's public promise become credible? The primary one-shot model compares cheap talk with the same promise backed by a transparent commitment bond. It holds the hidden honest/exploitative bot-type prior fixed at 50/50, elicits a forecast before investment, and uses exact half-point returns.

The repository also includes an eight-round learning visualization: five cheap-talk rounds followed by three bond rounds with one hidden programmed type held fixed. This mode is educational, not a causal estimate; a future study would randomize or counterbalance order.

## Run the artifacts

- [Open the Google Colab notebook](https://colab.research.google.com/drive/1EwIGvrd73aRVu7Y1Rci-PaBxlrlTwzzC) or open `companion/notebooks/Temur_PS1_Commitment_Bond_Revised.ipynb` in Colab and run all cells.
- [Play the Hugging Face demo](https://huggingface.co/spaces/dku-comsci-econ206-2026/commitment-bond-trust-game).
- To run the demo locally, open `companion/hf_space/index.html` with `model.js` in the same folder. No backend, API key, account, or data collection is used.

Outputs are programmed synthetic benchmarks, not evidence about human participants or deployed LLMs.

## Reproducibility

At investment `s = 10`, expected promise compliance is 0.5 under cheap talk and 1.0 under the bond. Expected welfare is 30 in both conditions; the bond changes compliance and the payoff distribution from `(7.5, 22.5)` to `(15, 15)`.

The notebook uses standard Python libraries. Returns are represented exactly in half-points; no values are rounded down.

## Files

- `main.tex`, `sections/`, `appendices/`, and `references.bib`: submitted proposal source.
- `commitment_bond_teaser.drawio`: editable teaser master; `.svg` and `.pdf` are vector exports.
- `companion/notebooks/Temur_PS1_Commitment_Bond_Revised.ipynb`: computational benchmark.
- `companion/hf_space/`: static interactive demo source.

The project supports SDG 4 (Quality Education) by giving students a hands-on way to compare cheap talk with an incentive-backed promise and inspect forecast calibration.
