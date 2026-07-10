<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:6e40c9&height=200&section=header&text=Aidan%20Joneleit&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI%20Software%20Engineer&descAlignY=58&descSize=18" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=900&color=A371F7&center=true&vCenter=true&width=780&lines=AI+software+engineer+who+builds+end+to+end;Fine-tuning+RNA+language+models+%40+TriasBio;Agent+evals+and+RL+environments+%40+OpenAI;On-device+LLM+serving+%40+Qualcomm)](https://github.com/joneleit)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aidanjoneleit)
[![Email](https://img.shields.io/badge/Email-161b22?style=for-the-badge&logo=gmail&logoColor=EA4335)](mailto:joneleit@berkeley.edu)
[![UC Berkeley](https://img.shields.io/badge/UC%20Berkeley-M.E.T.%20Program-161b22?style=for-the-badge&logo=googlescholar&logoColor=FDB515)](https://met.berkeley.edu/)

</div>

---

## 👋 About me

I'm an AI software engineer who likes building things end to end, from the product down to the systems that run it. I'm at UC Berkeley earning a B.S. Electrical Engineering and Computer Sciences and a B.S. Business Administration through the M.E.T. dual-degree program.

- 🧬 Summer 2026: ML engineer at TriasBio, fine-tuning RNA language models to help design personalized medicines
- 🤖 Recently: built reinforcement-learning training environments and agent evaluations at OpenAI, and got large language models running directly on Snapdragon phone chips at Qualcomm
- 🃏 Founder of PokePulse, a Python e-commerce platform with automatic pricing (~500 products, about $21K per month in profit) that I ran for seven years
- 🏔️ Eagle Scout who led a 176-mile backcountry expedition. I disappear into the mountains when my training runs are stable

<div align="center">

## 🛠️ Tools I build with

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🚀 Featured projects

### 🦅 [kestrel](https://github.com/joneleit/kestrel) — an LLM inference engine built from scratch

> **In plain English:** the software that actually runs a large language model and streams back answers, the same job tools like vLLM do. I built every layer myself, from the web server down to the GPU code, so I understand how it works underneath.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Triton](https://img.shields.io/badge/-Triton%20kernel-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Tests](https://img.shields.io/badge/tests-41%20passing-2ea043?style=flat-square)

- ⚡ Real serving techniques (paged memory, request batching, speculative decoding) that make a language model respond fast
- ✅ Proven correct by tests: the fast version gives exactly the same output as the simple reference version, even under memory pressure
- ☁️ Full production setup: an OpenAI-compatible API, one-command AWS deployment, and live dashboards for speed and cost

### 🧵 [loom](https://github.com/joneleit/loom) — training a language model from zero

> **In plain English:** I built the full pipeline to create a small language model from nothing. Teach it to read, then teach it to answer, then improve it with reinforcement learning, and I measured that it got smarter at each step.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![GRPO](https://img.shields.io/badge/-GRPO%20RL-8957e5?style=flat-square)
![Tests](https://img.shields.io/badge/tests-28%20passing-2ea043?style=flat-square)

- 📈 Accuracy climbed 3% to 20% to 26% across the three training stages on a held-out test, and every number is real and saved in the repo
- 🧮 The reinforcement-learning algorithm (GRPO) is written from the math up, with no pre-made library
- 💾 Survives cloud interruptions: training resumes exactly where it left off, which keeps costs low on cheap spot servers

<div align="center">

Both repos include a design write-up explaining every decision and a roadmap of what I'm building next.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6e40c9,100:0d1117&height=120&section=footer" width="100%"/>

</div>
