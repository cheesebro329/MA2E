# MA<sup>2</sup>E : Addressing Partial Observability in Multi-Agent Reinforcement Learning with Masked Auto-Encoder
<a href="[https://arxiv.org/abs/2405.19806](https://openreview.net/forum?id=klpdEThT8q&referrer=%5BAuthor%20Console%5D(%2Fgroup%3Fid%3DICLR.cc%2F2025%2FConference%2FAuthors%23your-submissions))"><img src="https://img.shields.io/badge/Paper-OpenReview-Green"></a>
<a href="#citation
"><img src="https://img.shields.io/badge/Paper-BibTex-yellow"></a>

<div style="display: flex; justify-content: center; gap: 20px;">
  <img src="./assets/figure2.jpg" alt="" width="48%">
  <img src="./assets/figure3.jpg" alt="" width="48%">
</div>

## 🎯 Description 
This is the official code repository for the paper ["MA<sup>2</sup>E : Addressing Partial Observability in Multi-Agent Reinforcement Learning with Masked Auto-Encoder"](https://openreview.net/forum?id=klpdEThT8q&referrer=%5BAuthor%20Console%5D(%2Fgroup%3Fid%3DICLR.cc%2F2025%2FConference%2FAuthors%23your-submissions)) accepted by ICLR 2025.
MA<sup>2</sup> is a novel approach to addressing partial observability in multi-agent reinforcement learning (MARL). MA<sup>2</sup>E enables agents to infer global information solely from local observations by leveraging masked auto-encoders (MAE), eliminating the need for explicit communication.


## ⚙️ Installation
The code is based on pymarl2. 
For detailed information, refere to the installation instructions of [pymarl2](https://github.com/hijkzzz/pymarl2) and [SMAC](https://github.com/oxwhirl/smac).

1️⃣ Cloning MA<sup>2</sup>E 

`git clone https://github.com/cheesebro329/MA2E.git`

2️⃣ Donwload and setup StarCraftII 

`bash install_sc2.sh`

3️⃣ Install required packages 

`pip install -r requirements.txt`


## 🎮 Running Script

🏃Run an experiment 

`bash run.sh config_name env_config_name map_name_list (arg_list threads_num gpu_list experinments_num)`

✔️ Example 

`bash run.sh qmix sc2 3s_vs_5z use_MT=True 3 0 3`

* Run QMIX+MA2E in SMAC 3s_vs_5z scenario
  
* `use_MT` means executing the model plugs in MA2E into the baseline algorithm. 

<a name="citation"></a>
## 📌 Citation
```bibtext
@inproceedings{
kang2025mae,
title={{MA}\${\textasciicircum}2\$E: Addressing Partial Observability in Multi-Agent Reinforcement Learning with Masked Auto-Encoder},
author={Sehyeok Kang and Yongsik Lee and Gahee Kim and Song Chong and Se-Young Yun},
booktitle={The Thirteenth International Conference on Learning Representations},
year={2025},
url={https://openreview.net/forum?id=klpdEThT8q}
}
```
