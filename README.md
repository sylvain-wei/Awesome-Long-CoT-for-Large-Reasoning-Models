# Awesome-Long-CoT-for-Large-Reasoning-Models
Collection of insights for Long-CoT for Large Reasoning Models

# Long CoT in Post-training
## Training Paradigm
1. [(25.02 arxiv, UCB) LLMs Can Easily Learn to Reason from Demonstrations Structure, not content, is what matters!](https://arxiv.org/pdf/2502.07374):
   - A Large Language model (LLM) can effectively learn Long CoT reasoning through data-efficient supervised fine-tuning (SFT) and parameter-efficient low-rank adaptation (LoRA);
   - **The structure of Long CoT is critical to the learning process, whereas the content of individual reasoning steps has minimal impact.**


# Why Long CoT + RL Works?
1. [(25.02 arxiv, CMU) Demystifying Long CoT Reasoning in LLMs](https://arxiv.org/pdf/2502.03373):
 - While SFT is not strictly necessary, it simplifies training and improves efficiency;
 - Reasoning capabilities tend to emerge with increased training compute, but their development is not guaranteed, making reward shaping crucial for stabilizing CoT length growth;
 - Scaling verifiable reward sig-nals is critical for RL. We find that leveraging noisy, web-extracted solutions with filtering mechanisms shows strong potential, particularly for out-of-distribution (OOD) tasks such as STEM reasoning;
 - Core abilities like error correction are inherently present in base models, but incentivizing these skills effectively for complex tasks via RL demands significant compute, and measuring their emergence requires a nuanced approach. 
