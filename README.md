# Asia Cup 2025: A Structured T20 Match-Level Dataset and Exploratory Analysis
<p align="center"> <a href="https://kousarraza.github.io/AsiaCup2025"><img src="https://img.shields.io/badge/🌐-Project%20Page-blue" alt="Project Page"></a> <a href="https://arxiv.org/abs/2512.XXXX"><img src="https://img.shields.io/badge/📄-arXiv%3A2512.XXXX-b31b1b" alt="arXiv"></a> <a href="https://doi.org/10.5281/zenodo.17228056"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.17228056.svg" alt="DOI"></a> <a href="https://github.com/kousarraza/AsiaCup2025/blob/main/LICENSE"><img src="https://img.shields.io/badge/📜-License%3A%20CC%20BY%204.0%2FMIT-green" alt="License"></a> <a href="https://github.com/kousarraza/AsiaCup2025/stargazers"><img src="https://img.shields.io/github/stars/kousarraza/AsiaCup2025?style=social&logo=github" alt="GitHub Stars"></a> <a href="https://github.com/kousarraza/AsiaCup2025/network/members"><img src="https://img.shields.io/github/forks/kousarraza/AsiaCup2025?style=social&logo=github" alt="GitHub Forks"></a> <a href="https://github.com/kousarraza/AsiaCup2025/issues"><img src="https://img.shields.io/github/issues/kousarraza/AsiaCup2025" alt="GitHub Issues"></a> </p><p align="center"> <strong>A Complete Dataset and Analysis of the Asia Cup 2025 T20 Cricket Tournament</strong><br> <em>19 Matches • 61 Variables • 22 Visualizations • Open Source</em> </p><p align="center"> <a href="https://github.com/kousarraza">Kousar Raza</a><sup>1*</sup> · <a href="https://github.com/faizanali">Faizan Ali</a><sup>2*</sup> </p><p align="center"> <sup>1</sup>University of Isfahan, Iran · <sup>2</sup>University of Sindh, Jamshoro, Pakistan </p><p align="center"> <a href="https://kousarraza.github.io/AsiaCup2025">🌐 Live Interactive Report</a> · <a href="https://github.com/kousarraza/AsiaCup2025/archive/refs/heads/main.zip">📦 Download Dataset</a> · <a href="#citation">📝 Cite This Work</a> · <a href="#contact">📧 Contact</a> </p>

<p align="center">
  <strong>Directional Textual Inversion for Personalized Text-to-Image Generation</strong>
</p>


<p align="center">
  <sup>1</sup>KAIST · <sup>2</sup>Sookmyung Women's University
</p>

---

## Overview

Textual Inversion (TI) is efficient but often suffers from **embedding norm inflation**—learned tokens drift to out-of-distribution magnitudes, degrading prompt fidelity in pre-norm Transformers.

**Directional Textual Inversion (DTI)** addresses this by:
- **Decoupling magnitude and direction**: Fixing embedding magnitude to an in-distribution scale
- **Spherical optimization**: Optimizing only the direction on the unit hypersphere via Riemannian SGD
- **vMF prior**: Using a von Mises-Fisher prior for semantic coherence

DTI achieves superior text fidelity and subject preservation on **SDXL** and **SANA**.

<p align="center">
  <img src="docs/assets/teaser.png" alt="DTI Results" width="100%">
</p>

## Installation

**Requirements:** Python 3.9+ · PyTorch 2.0+ · CUDA GPU

```bash
git clone https://github.com/kunheek/dti
cd dti
pip install -e .
```

<details>
<summary>Using uv (recommended for faster setup)</summary>

```bash
uv venv python=3.12
source .venv/bin/activate
pip install -e .
```
</details>

## Quick Start

### Train DTI on SDXL

```bash
python exps/ours_sdxl.py -g 0
```

This runs DTI on all DreamBooth subjects. To train on a specific subject:

```bash
python exps/ours_sdxl.py -g 0 --instances dog
```

<details>
<summary>Full training command</summary>

```bash
accelerate launch --mixed_precision=bf16 --num_processes=1 \
  scripts/train_sdxl.py \
  --pretrained_model_name_or_path "stabilityai/stable-diffusion-xl-base-1.0" \
  --train_data_dir data/dreambooth/dog \
  --output_dir output/dti-sdxl/dog \
  --placeholder_token "<dog>" \
  --initializer_token dog \
  --resolution 768 \
  --train_batch_size 4 \
  --max_train_steps 400 \
  --learning_rate 0.01 \
  --token_scale mean \
  --kappa 1e-4 \
  --decompose_scale true
```
</details>

### Train on SANA

```bash
python exps/ours_sana.py -g 0 -m sana1.5_1.6b
```

### Evaluate

```bash
python scripts/evaluate.py -e output/dti-sdxl
```

## Training Options

| Parameter | Description | Default |
|-----------|-------------|---------|
| `-g` | GPU ID | `0` |
| `--instances` | Subject names | all |
| `--max_train_steps` | Training iterations | `400` |
| `--kappa` | vMF prior strength | `1e-4` |
| `--learning_rate` | Learning rate | `0.01` |
| `--token_scale` | Magnitude scale (`mean`, `max`, or float) | `mean` |

### Baselines

```bash
# Standard Textual Inversion
python exps/ti_sdxl.py -g 0

# DCO + DTI
python exps/ours_dco_sdxl.py -g 0
```

## Data Format

```
data/
├── dreambooth.json
└── dreambooth/
    └── subject_name/
        ├── 00.jpg
        ├── 01.jpg
        └── ...
```

JSON format:
```json
{
  "subject_name": {
    "path": "data/dreambooth/subject_name",
    "class": "dog",
    "initialization": "dog"
  }
}
```

Download DreamBooth dataset:
```bash
python scripts/download_datasets.py
```

## Project Structure

```
dti/
├── src/dti/       # Core implementation
├── scripts/       # Training & evaluation scripts
├── exps/          # Experiment launchers
└── data/          # Datasets and configs
```

## Citation

```bibtex
@article{kim2025directional,
  title={Directional Textual Inversion for Personalized Text-to-Image Generation},
  author={Kim, Kunhee and Park, NaHyeon and Hong, Kibeom and Shim, Hyunjung},
  journal={arXiv preprint arXiv:2512.13672},
  year={2025}
}
```

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
