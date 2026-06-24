# Hi, I'm Udayan 👋

**Second-year CS student** focused on **AI infrastructure** and **applied ML** — and just as happy going low-level. I build systems that have to actually work under load, and I care about *why* they break when they do.

I work across two layers:
- 🧠 **AI systems** — LLMs, RAG pipelines, history-aware retrieval, agentic architectures (LangChain / LangGraph)
- ⚙️ **The infra underneath** — async backends, dynamic batching, observability, and storage engines built from scratch

I learn fastest when I'm building something that has to hold up in the real world, not a tutorial.

---

## 🚀 Featured Projects

### 🗄️ [ColStore — Columnar Storage Engine](https://github.com/azycr4yy/ColStore) · `C++`
A columnar analytics engine built from scratch that's **17.7× faster than SQLite** on aggregation queries over **3M rows** of NYC Taxi data (15ms vs 266ms, 4 threads).
- Custom binary file format with typed, per-column headers and zero-copy access
- Adaptive compression — dictionary encoding (cardinality `< 0.05`) / RLE (avg run length `> 4.0`) / raw, chosen automatically per column
- Buffer pool with LRU eviction, pin counts, and dirty-page write-back
- Lock-free multithreaded parallel scan with per-thread result slots

### ⚡ [Lightweight ML Inference Server](https://github.com/azycr4yy/inference_server) · `Python` · `FastAPI` · `PyTorch`
A production-style inference server with an **async dynamic batching engine** that cuts **p50 latency 2.7× (35ms → 13ms)** under 50 concurrent users.
- Bounded-queue backpressure (HTTP 503 on overload, zero client hangs on failure)
- Full **Prometheus + Grafana** observability — p95 latency, batch-size distribution, queue depth
- Containerized with Docker Compose; **load-tested to 15,000+ requests at 140 req/s with 0 failures**
- Serves a DistilBERT model fine-tuned to **88.6% F1** on SST-2

### 🤖 [PatchPilot — Agentic Code Migration System](https://github.com/azycr4yy/PATCHPILOT) · `LangGraph` · `RAG` · `React`
A multi-step agent (**Retrieve → Plan → Patch → Verify → Reflect**) that automates framework and dependency migrations across multi-file repos.
- RAG grounded in official documentation to reduce hallucinations
- Dependency-aware patching with test-driven failure detection and automatic retry
- React observability dashboard for full traceability over agent decisions and migration state

---

## 💻 Tech Stack

**Languages**
![C](https://img.shields.io/badge/c-%2300599C.svg?style=flat-square&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=flat-square&logo=openjdk&logoColor=white)

**AI / ML**
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat-square&logo=PyTorch&logoColor=white) ![HuggingFace](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-FFD21E?style=flat-square) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-FF6F61?style=flat-square) ![CUDA](https://img.shields.io/badge/cuda-000000.svg?style=flat-square&logo=nVIDIA&logoColor=green)

**Backend & Infra**
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=Prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=flat-square&logo=grafana&logoColor=white)

**Databases & Tools**
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=flat-square&logo=mysql&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=flat-square&logo=github&logoColor=white)

---

## 📊 GitHub Stats

![](https://github-readme-stats.vercel.app/api?username=azycr4yy&theme=gotham&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=azycr4yy&theme=gotham&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=azycr4yy&theme=gotham&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

---

## 🌐 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN-SLUG) [![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/ud8yan) [![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/uday4n)

<a href="https://visitcount.itsvg.in"><img src="https://visitcount.itsvg.in/api?id=azycr4yy&icon=0&color=0" alt="visitor count"/></a>
