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
