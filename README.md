<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:6e40c9&height=200&section=header&text=Aidan%20Joneleit&fontSize=50&fontColor=ffffff&fontAlignY=38&desc=AI%20Software%20Engineer&descAlignY=58&descSize=18" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=900&color=A371F7&center=true&vCenter=true&width=780&lines=AI+software+engineer+who+builds+end+to+end;Fine-tuning+RNA+language+models+%40+TriasBio;Agent+evals+and+RL+environments+%40+OpenAI;On-device+LLM+serving+%40+Qualcomm)](https://github.com/joneleit)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aidanjoneleit)
[![Email](https://img.shields.io/badge/joneleit@berkeley.edu-161b22?style=for-the-badge&logo=gmail&logoColor=EA4335)](mailto:joneleit@berkeley.edu)
[![UC Berkeley](https://img.shields.io/badge/UC%20Berkeley-M.E.T.%20Program-161b22?style=for-the-badge&logo=googlescholar&logoColor=FDB515)](https://met.berkeley.edu/)

</div>

---

## 👋 About me

I'm an AI software engineer who likes building things end to end, from the product down to the systems that run it. I'm at UC Berkeley studying for a B.S. Electrical Engineering and Computer Sciences and a B.S. Business Administration through the M.E.T. dual-degree program.

- 🧬 Summer 2026: ML engineer at TriasBio, fine-tuning RNA language models to help design personalized medicines
- 🤖 Recently: built reinforcement-learning training environments and agent evaluations at OpenAI, and got large language models running directly on Snapdragon phone chips at Qualcomm
- 🃏 Founder of PokePulse, a Python e-commerce platform with automatic pricing (~500 products, about $21K per month in profit) that I ran for seven years
- 🏔️ Eagle Scout who led a 176-mile backcountry expedition. I disappear into the mountains when my training runs are stable

<div align="center">

## 🛠️ Tools I build with

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🚀 Featured projects

### 🦅 [kestrel](https://github.com/joneleit/kestrel) ~ an LLM inference engine built from scratch

> The system that serves a large language model and streams tokens back to the user, the same role tools like vLLM and TGI play. I wrote every layer myself, from the HTTP server down to the GPU kernels, so I understand exactly how inference works.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Triton](https://img.shields.io/badge/-Triton%20kernel-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Tests](https://img.shields.io/badge/tests-41%20passing-2ea043?style=flat-square)

- ⚡ Real serving techniques (paged KV cache, continuous batching, speculative decoding) that keep latency low under load
- ✅ Correctness proven by tests: the optimized path produces identical output to a simple reference implementation, even under memory pressure
- ☁️ Production-ready: an OpenAI-compatible API, one-command AWS deployment, and live dashboards for throughput and cost

### 🧵 [loom](https://github.com/joneleit/loom) ~ training a language model from zero

> A full pipeline that builds a small language model from scratch: pretraining, then supervised fine-tuning, then reinforcement learning, with evaluations at each stage that show the model measurably improve.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![GRPO](https://img.shields.io/badge/-GRPO%20RL-8957e5?style=flat-square)
![Tests](https://img.shields.io/badge/tests-28%20passing-2ea043?style=flat-square)

- 📈 Held-out accuracy climbed 3% to 20% to 26% across the three training stages, and every number is reproducible from the repo
- 🧮 The reinforcement-learning algorithm (GRPO) is implemented from the math up, with no pre-made library
- 💾 Survives cloud interruptions: training resumes exactly where it left off, which keeps costs low on cheap spot servers

### 🎨 [sketchroom](https://github.com/joneleit/sketchroom) ~ a real-time collaborative whiteboard

> A shared canvas anyone can join from a link: strokes and live cursors appear on every screen as they happen. It's the same synchronization problem behind Figma and Google Docs, solved with nothing but AWS serverless parts, so a room costs nothing while it sits idle.

![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![AWS](https://img.shields.io/badge/-AWS%20serverless-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Tests](https://img.shields.io/badge/tests-12%20passing-2ea043?style=flat-square)

- ⚡ Feels instant: pointer input is batched every 60 ms and fanned out through API Gateway WebSockets by Lambda, so a stroke shows up on everyone's screen while it's still being drawn
- 🧹 Nothing to babysit: one DynamoDB table holds rooms, peers, and strokes; TTLs erase abandoned rooms on their own, and late joiners still get the full canvas
- 💰 The whole stack is Terraform and deploys with one command; a ten-person, hour-long session costs under a cent

<div align="center">

All three repos include a design write-up explaining every decision and a roadmap of what I'm building next.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6e40c9,100:0d1117&height=120&section=footer" width="100%"/>

</div>
