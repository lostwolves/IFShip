# IFShip
IFShip is a vision-language model for remote sensing fine-grained ship classification (RS-FGSC). It uses domain-aware CoT prompts and the TITANIC-FGS dataset to enable step-by-step visual reasoning, achieving both high accuracy and interpretability beyond models like LLaVA and MiniGPT-4.

## TITANIC-FGS Dataset Overview

TITANIC-FGS is the first domain knowledge-enhanced, instruction-following dataset specifically designed for the Remote Sensing Fine-Grained Ship Classification (RS-FGSC) task. It simulates human-like step-by-step decision-making to train vision-language models (VLMs) for interpretable and accurate ship classification.

### 🛳️ Category Coverage
The dataset covers 17 categories, including:
- 8 military ships:  
  C1 – Aircraft carrier  
  C2 – Amphibious assault ship  
  C3 – Cruiser  
  C4 – Depot ship  
  C5 – Destroyer  
  C6 – Frigate  
  C7 – Landing ship  
  C8 – Littoral combat ship  

- 8 civilian ships:  
  C10 – Container ship  
  C11 – Cruise ship  
  C12 – Fishing boat  
  C13 – Icebreaker  
  C14 – Oil tanker  
  C15 – Scientific research ship  
  C16 – Tugboat  
  C17 – Yacht  

- 1 background class:  
  C9 – Non ship

### 🖼️ Data Statistics
- Total images: 18,929  
  - Training: 16,876 images with multi-round CoT-style instructions (4–6 turns for ship images, 1 for non-ship)  
  - Testing: 2,053 images with fine-grained labels only  
- Image resolution: ranges from 200×100 to 4000×2000 pixels  
- Source: Public search engines (e.g., Google, Baidu)

### 🧠 Instruction Design
Each training sample includes natural language instructions that guide the model through human-like reasoning, encouraging alignment between model predictions and domain knowledge. This structure enables effective learning of interpretable classification patterns.

📥 **Download Link**: [Click to download TITANIC-FGS](https://drive.google.com/file/d/1dyvK3AJ9pnlg6u8ruHZS16TeM6hdl_SR/view?usp=drive_link)

## Citation

If you find our work useful in your research, please cite our paper:

```
@article{GUO2025111672,
  title     = {IFShip: Interpretable fine-grained ship classification with domain knowledge-enhanced vision-language models},
  journal   = {Pattern Recognition},
  volume    = {166},
  pages     = {111672},
  year      = {2025},
  issn      = {0031-3203},
  doi       = {https://doi.org/10.1016/j.patcog.2025.111672},
  url       = {https://www.sciencedirect.com/science/article/pii/S0031320325003322},
  author    = {Mingning Guo and Mengwei Wu and Yuxiang Shen and Haifeng Li and Chao Tao}
}
```
