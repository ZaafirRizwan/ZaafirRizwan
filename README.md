<div align="center">

<img src="assets/banner.svg" alt="Zaafir Rizwan — AI Engineer building production LLM, RAG and voice systems" width="100%" />

<br/>

<a href="https://github.com/ZaafirRizwan">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=17&duration=2600&pause=900&color=22D3EE&center=true&vCenter=true&multiline=false&repeat=true&width=720&height=40&lines=LLM+agents+with+tool+calling%2C+MCP+and+provider+failover;RAG+pipelines%3A+ingestion+%E2%86%92+embeddings+%E2%86%92+Qdrant+%E2%86%92+answers;Real-time+voice+agents+over+SIP+and+WebRTC;Data+pipelines%2C+vision+and+forecasting+on+AWS+and+Azure;Every+request+traced+with+OpenTelemetry+into+ClickHouse" alt="What I build" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-zaafir--rizwan-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/zaafir-rizwan)
[![Email](https://img.shields.io/badge/Email-zaafir.rizwan%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:zaafir.rizwan@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-zaafir--rizwan.tech-111827?style=for-the-badge&logo=vercel&logoColor=white)](https://zaafir-rizwan.tech)

</div>

<br/>

## Right now

**Senior AI Engineer at TriFusionTech.** I own the Python runtime behind a multi-tenant voice-AI platform: autonomous phone agents that answer, route, and resolve live customer calls, running across **600+ production agents**. I own it from the first audio frame to the SIP transfer that hands the caller to a human, plus the RAG stack, Redis cache layer, observability, and the Next.js dashboards and public API around it.

Before that: ELT pipelines on Azure Data Factory, a video-intelligence pipeline on Gemini and Grounding DINO, and real-time inference APIs on AWS SageMaker.

<div align="center">
<img src="assets/pipeline.svg" alt="Animated diagram: one call flowing through the voice agent runtime" width="100%" />
</div>

<table>
<tr>
<td width="33%" valign="top">

### 🎙️ Voice runtime
- Streaming STT → LLM → TTS pipeline (Python, LiveKit Agents)
- Turn-taking, barge-in, endpointing, DTMF
- Blind + warm transfers over **SIP REFER**, REFER+Replaces, DTMF confirm, BLF checks
- Answering-machine + IVR detection for outbound
- Screen sharing into multimodal LLM calls

</td>
<td width="33%" valign="top">

### 📚 Retrieval & reliability
- Ingestion worker: S3 → MinerU → chunking → embeddings → **Qdrant**
- In-call retriever with query rewriting, per-KB isolation
- Fallback chains across OpenAI, Anthropic, xAI, Deepgram, Cartesia, ElevenLabs
- First-token stall guard that fails over mid-turn
- Supabase → **Redis** config cache with realtime sync

</td>
<td width="33%" valign="top">

### 🧩 Platform & product
- In-call payments on **Stripe Connect** with idempotency + guardrails
- Tool integrations: calendars, PBX SMS, webhooks, **MCP** servers, ERPs
- **OpenTelemetry → ClickHouse** metrics, cost and usage per org
- Next.js 15 dashboards, public v1 REST API, feature gating
- 130+ pytest modules incl. LLM-judged behavioral tests

</td>
</tr>
</table>

<br/>

## Featured projects

| Project | What it shows | Stack |
| --- | --- | --- |
| [**luma-bistro-livekit-voice-agent**](https://github.com/ZaafirRizwan/luma-bistro-livekit-voice-agent) | Browser voice call with streaming STT/TTS, interruption-aware turns, and guarded, idempotent reservation tools | `LiveKit` `Deepgram Flux` `Cartesia` `FastAPI` |
| [**mini-agentic-rag-system**](https://github.com/ZaafirRizwan/mini-agentic-rag-system) | Agentic RAG with graph-style retrieval, custom tools, memory, and multi-step execution | `LangGraph` `Python` |
| [**Rag_log_analysis**](https://github.com/ZaafirRizwan/Rag_log_analysis) | Hybrid BM25 + FAISS retrieval with self-corrective query rewriting over logs | `Gemini` `FAISS` `Flask` |
| [**resume-fit**](https://github.com/ZaafirRizwan/resume-fit) | Resume-to-job match scoring with skill-gap analysis, shipped as a full product | `FastAPI` `React` `PostgreSQL` `Celery` |
| [**Inventory_Monitoring…Sagemaker**](https://github.com/ZaafirRizwan/Inventory_Monitoring_at_Fullfillment_Centers_using_Sagemaker) | Item-counting pipeline with deep learning and real-time inference endpoints | `SageMaker` `PyTorch` |
| [**Predict-Bike-Sharing-Demand**](https://github.com/ZaafirRizwan/Predict-Bike-Sharing-Demand-with-AutoGluon) | Demand-forecasting regression with AutoML and automated hyperparameter tuning | `AutoGluon` |

<br/>

## Stack

<div align="center">

**Voice & agents**<br/>
![LiveKit](https://img.shields.io/badge/LiveKit-0D1117?style=for-the-badge&logo=livekit&logoColor=22D3EE)
![OpenAI](https://img.shields.io/badge/OpenAI-0D1117?style=for-the-badge&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic-0D1117?style=for-the-badge&logo=anthropic&logoColor=white)
![Deepgram](https://img.shields.io/badge/Deepgram-0D1117?style=for-the-badge&logoColor=white)
![Cartesia](https://img.shields.io/badge/Cartesia-0D1117?style=for-the-badge&logoColor=white)
![SIP](https://img.shields.io/badge/SIP%20%2F%20WebRTC-0D1117?style=for-the-badge&logo=webrtc&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-0D1117?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-0D1117?style=for-the-badge&logo=langchain&logoColor=white)

**Data & retrieval**<br/>
![Qdrant](https://img.shields.io/badge/Qdrant-0D1117?style=for-the-badge&logo=qdrant&logoColor=DC244C)
![Redis](https://img.shields.io/badge/Redis-0D1117?style=for-the-badge&logo=redis&logoColor=DC382D)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0D1117?style=for-the-badge&logo=postgresql&logoColor=4169E1)
![Supabase](https://img.shields.io/badge/Supabase-0D1117?style=for-the-badge&logo=supabase&logoColor=3FCF8E)
![ClickHouse](https://img.shields.io/badge/ClickHouse-0D1117?style=for-the-badge&logo=clickhouse&logoColor=FFCC01)
![S3](https://img.shields.io/badge/AWS%20S3-0D1117?style=for-the-badge&logo=amazons3&logoColor=569A31)

**Languages & web**<br/>
![Python](https://img.shields.io/badge/Python-0D1117?style=for-the-badge&logo=python&logoColor=3776AB)
![TypeScript](https://img.shields.io/badge/TypeScript-0D1117?style=for-the-badge&logo=typescript&logoColor=3178C6)
![SQL](https://img.shields.io/badge/SQL-0D1117?style=for-the-badge&logo=postgresql&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-0D1117?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-0D1117?style=for-the-badge&logo=react&logoColor=61DAFB)
![FastAPI](https://img.shields.io/badge/FastAPI-0D1117?style=for-the-badge&logo=fastapi&logoColor=009688)
![Stripe](https://img.shields.io/badge/Stripe-0D1117?style=for-the-badge&logo=stripe&logoColor=635BFF)

**Infra & observability**<br/>
![AWS](https://img.shields.io/badge/AWS-0D1117?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)
![Azure](https://img.shields.io/badge/Azure-0D1117?style=for-the-badge&logo=microsoftazure&logoColor=0078D4)
![Docker](https://img.shields.io/badge/Docker-0D1117?style=for-the-badge&logo=docker&logoColor=2496ED)
![Kubernetes](https://img.shields.io/badge/Kubernetes-0D1117?style=for-the-badge&logo=kubernetes&logoColor=326CE5)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-0D1117?style=for-the-badge&logo=opentelemetry&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-0D1117?style=for-the-badge&logo=grafana&logoColor=F46800)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-0D1117?style=for-the-badge&logo=githubactions&logoColor=2088FF)
![pytest](https://img.shields.io/badge/pytest-0D1117?style=for-the-badge&logo=pytest&logoColor=0A9EDC)

</div>

<br/>

## How I think

> Users judge an AI product in the second after they stop talking or press enter. Everything I build serves that moment: streaming everywhere, failover before silence, tools that fail closed, and telemetry on every span so the next incident is a query, not a guess.

- **Production over demo.** Idempotency keys, guardrails, and audit rows are part of the feature, not follow-ups.
- **Measure, don't assume.** Model capabilities, latencies, and provider quirks get tested, then recorded.
- **Tests that would catch the bug.** Mutation-check the test before trusting it.
- **Own the whole path.** Runtime, retrieval, dashboards, API, and docs, so the seams don't leak.

<br/>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=ZaafirRizwan&show_icons=true&hide_border=true&bg_color=0B1020&title_color=22D3EE&icon_color=A78BFA&text_color=94A3B8&hide=contribs&rank_icon=github" height="165" alt="GitHub stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ZaafirRizwan&layout=compact&hide_border=true&bg_color=0B1020&title_color=22D3EE&text_color=94A3B8&langs_count=6" height="165" alt="Top languages" />

<br/><br/>

### Building agents, retrieval, voice, or data systems that have to work at 3 a.m.? Let's talk.

[![Connect on LinkedIn](https://img.shields.io/badge/Connect%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/zaafir-rizwan)
[![Email Me](https://img.shields.io/badge/Email%20Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:zaafir.rizwan@gmail.com)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1020,50:22D3EE,100:A78BFA&height=100&section=footer" width="100%" alt="" />

</div>
