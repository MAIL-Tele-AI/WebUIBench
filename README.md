<h1 align="center"> WebUIBench </h1>
<h3 align="center"> A Comprehensive Benchmark for Evaluating Multimodal Large Language Models in WebUI-to-Code </h3>

<p align="center">
  <a href="https://arxiv.org/abs/xx" target="_blank">📄arXiv</a> •
  <a href="https://huggingface.co/papers/xx" target="_blank">🤗HFPaper</a> •
  <a href="https://zjunlp.github.io/project/WorFBench/" target="_blank">🌐Web</a> •
  <a href="https://huggingface.co/collections/zjunlp/worfbench-66fc28b8ac1c8e2672192ea1" target="_blank">📊Dataset</a> •
</p>

[![Awesome](https://awesome.re/badge.svg)](https://github.com/zjunlp/WorFBench) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
![](https://img.shields.io/github/last-commit/zjunlp/WorFBench?color=green) 

## 💡 News

- `2024/05/20`: We release the Leaderboard of WebUIBench. Download dataset [here](https://huggingface.co/datasets/xx)



## 🌟Overview

With the rapid advancement of Generative AI technology, Multimodal Large Language Models(MLLMs) have the potential to act as AI software engineers capable of executing complex web application development. Considering that the model requires a confluence of multidimensional sub-capabilities to address the challenges of various development phases, constructing a multi-view evaluation framework is crucial for accurately guiding the enhancement of  development efficiency. However, existing benchmarks usually fail to provide an assessment of sub-capabilities and focus solely on webpage generation outcomes. In this work, we draw inspiration from the principles of software engineering and further propose WebUIBench, a benchmark systematically designed to evaluate MLLMs in four key areas: \textit{*WebUI Perception*}, \textit{*HTML Programming*}, \textit{*WebUI-HTML Understanding*}, and \textit{*WebUI-to-Code*}. WebUIBench comprises 21K high-quality question-answer pairs derived from over 0.7K real-world websites. The extensive evaluation of 29 mainstream MLLMs uncovers the skill characteristics and various weakness that models encountered during the development process. You can download our dataset from [huggingface](https://huggingface.co/xx)!

![overview](assets/overview.PNG)

## 💡Evaluation Results

The research team conducted a comprehensive evaluation of 29 mainstream multimodal large language models, including 7 closed-source models (such as GPT-4o, Gemini-1.5 Pro, and Claude-3.5-Sonnet) and 22 open-source models (such as the InternVL2.5 series and the Qwen2-VL series, with parameter sizes ranging from 2B to 78B).

![eval_results](assets/eval_results.png)


## 🔧Installation

```bash
git clone https://github.com/MAIL-Tele-AI/WebUIBench
cd WebUIBench
pip install -r requirements.txt
```

## 🤔Evaluation

```bash
tasks=(ec ocr ap vg cec cfe whm whr w2c)
model_name=your_model_name
for task in ${tasks[@]}; do
    python model_eval.py \
        --task xx \
        --model_name ${model_name} \
        --gold_path xx
        --pred_path xx
        --eval_model gpt4o \
        --eval_output xx
        --eval_type node \
        --task_type ${task} \
```

## 🚩Citation

If you find this work is helpful, please kindly cite as follows. Thanks !

```bibtex
@article{xx,
  title={WebUIBench: A Comprehensive Benchmark for Evaluating Multimodal Large Language Models in WebUI-to-Code},
  author={xx},
  journal={arXiv preprint arXiv:xx},
  year={2025}
}
```

## 💐 Acknowledgement

We expressed sincerely gratitude for the projects listed following:

- [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) provides useful out-of-box tools and implements many adavanced LVLMs. Thanks for their selfless dedication.

  

We will offer long-term maintenance to fix bugs and solve issues. So if you have any problems, please put issues to us. 





