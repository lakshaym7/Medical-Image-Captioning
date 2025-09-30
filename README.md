# 🩺 QMuTrf: Quantum-Infused Multimodal Transformer for Radiology Captioning  

## 📌 Overview  
*QMuTrf* is a Quantum-Infused Multimodal Transformer that integrates:  
- Vision Transformers (*ViT, DEiT, BEiT*)  
- *Quantum Transfer Learning (QTL)*  
- *GPT-2 decoder*  

for *automated radiology caption generation* from chest X-rays.  

This hybrid *quantum-classical framework* pushes the boundaries of medical AI by capturing subtle diagnostic patterns and producing *clinically meaningful radiology reports*.  

📄 *Full paper: *Quantum-Infused Multimodal Transformer Leveraging Cross-Domain Transfer Learning for Enhanced Radiology Caption Generation  

---

## 🚀 Features  
- *Quantum Transfer Learning (QTL)* using Variational Quantum Circuits (VQCs)  
- *Cross-Domain Transfer Learning (CDTL)* from *ImageNet → Chest X-rays*  
- *Transformer backbone*: ViT, DEiT, BEiT (with QTL integration)  
- *Decoder*: GPT-2 with cross-attention to generate captions  
- *Evaluation Metrics*:  
  - BLEU-1 to BLEU-4  
  - ROUGE-L  
  - Skip-Thought  
  - Greedy Matching  
  - Vector Extrema  
- *Datasets*:  
  - Chest X-ray Pneumonia Dataset ([HuggingFace](https://huggingface.co/datasets/hf-vision/chest-xray-pneumonia))  
  - IU Chest X-ray Dataset ([NIH OpenI](https://openi.nlm.nih.gov/gridquery?q=indiana%20university%20chest%20xray&m=1&n))  

---

## 📊 Results  

| *Model*            | *BLEU-1* | *BLEU-4* | *ROUGE-L* | *SkipThought CS* |
|-----------------------|------------|------------|-------------|---------------------|
| ViT-GPT2             | 0.581      | 0.114      | 0.387       | 0.981              |
| *ViT-GPT2 + QTL*   | *0.608*  | *0.137*  | *0.423*   | *0.987*          |
| DEiT-GPT2            | 0.575      | 0.109      | 0.420       | 0.983              |
| *DEiT-GPT2 + QTL*  | *0.614*  | *0.142*  | *0.437*   | *0.996*          |
| BEiT-GPT2            | 0.549      | 0.091      | 0.391       | 0.979              |
| *BEiT-GPT2 + QTL*  | *0.608*  | *0.137*  | *0.457*   | *0.991*          |

📌 *Best performance with 30 qubits & circuit depth 6*:  
- *BLEU-1* = 0.733  
- *BLEU-4* = 0.289  
- *ROUGE-L* = 0.614  

---

## 🧑‍⚕ Applications  
- Automated *radiology reporting* for chest X-rays  
- *Clinical decision support* to reduce reporting delays  
- *Medical AI research* at the intersection of quantum computing & healthcare  

---

## 📖 Citation  
If you use this work, please cite:  
```bibtex
@article{madan2025qmultrf,
  title={Quantum-Infused Multimodal Transformer Leveraging Cross-Domain Transfer Learning for Enhanced Radiology Caption Generation},
  author={Lakshay Madan Gopal, Hrishikesh G Kulkarni, Sridevi S, Gorkem Kar},
  journal={arXiv preprint arXiv:xxxx.xxxxx},
  year={2025}
}
