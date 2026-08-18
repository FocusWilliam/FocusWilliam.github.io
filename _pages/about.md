---
permalink: /
title: ""
excerpt: ""
author_profile: true


redirect_from:
  - /about/
  - /about.html

---


<!-- 
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}
-->

# Hi there 👋

I am an AI / Applied AI engineer building the platform layer that puts large language models into production — agent tooling and orchestration, low-latency inference pipelines, and the backend services and APIs that ship them, taken from design through deployment.

I hold an M.S. in Biomedical Image Computing (focus on AI for Imaging) from the University of Illinois Urbana-Champaign and a B.S. in Computer Science and Technology from Hong Kong Baptist University. My background spans LLM agent systems, inference optimization for medical imaging, and full-stack cloud-native services.

<!-- 
I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>).
-->

<!-- 
# 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2016</div><img src='images/500x300.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Paper Title](https://example.com)

**Author A**, Author B, Author C

- Short description of the contribution.
</div>
</div>
-->

# 💼 Work Experience
- *2026.06 - Present*, **SRE Intern — Agent Tooling for Production Release Automation**, Tencent America LLC, New York, USA.
  - Built the agent-facing tooling layer for an LLM release copilot, packaging a 6,000-line Node.js/Python/shell system as a model-invocable Skill plus MCP tools that turn unstructured release spreadsheets into schema-validated, immutable execution plans — removing manual entry of 40+ parameters per deployment.
  - Hardened the agent-to-shell interface with an argv-only execution model that structurally eliminates command injection, added cryptographic plan-integrity verification, and enforced fail-closed human-in-the-loop escalation on ambiguous input.
  - Cut release planning and task setup from roughly 30 minutes to about 1 minute per deployment; authored a 50-case regression suite covering concurrency, state-tampering, and injection defense.

- *2026.02 - 2026.06*, **Software Engineer Intern, SoulLink – AI Companion Platform**, SoulForge Tech LLC, Houston, USA.
  - Built and deployed a production hybrid search pipeline on AnythingLLM combining dense embedding retrieval, BM25, and Gemini 2.5 Flash reranking, letting users construct personalized virtual characters from uploaded documents.
  - Engineered a three-tier online memory system on Mem0 (3/14/90-day TTL) with query-time expiration and probabilistic lazy eviction, and extended RAGAS into a 6-dimension offline evaluation framework; the product reached 260+ testers and 8,400+ interactions with 9× week-over-week growth.

- *2025.08 - 2025.12*, **Machine Learning Engineer, Sponsored Capstone**, Siemens Healthineers, Champaign, USA.
  - Owned an inference optimization pipeline end-to-end — distillation, structured pruning, evaluation, latency profiling — on a physics-guided SigmaNet MRI reconstruction architecture.
  - Cut per-slice inference latency from 296.74ms to 136.67ms (~2.2× faster) and compressed the model from 53.90M to 13.87M parameters, while keeping reconstruction quality close to the teacher (43.70→43.39 PSNR, 0.9745→0.9728 SSIM).

- *2025.02 - 2025.08*, **Research Assistant, Quantitative Multiscale Imaging Group**, Beckman Institute for Advanced Science and Technology, Champaign, USA.
  - Designed an on-premise data lake for large scientific datasets using prefix-partitioned directories and metadata indexing, enabling streamed mini-batch loading and faster training throughput.
  - Containerized training jobs with Docker on HPC clusters and automated a multi-stage atlas-registration workflow (DeepSlice + nonlinear alignment) across 35 high-resolution image slices at 3.5µm.

# 📖 Educations
- *2024.09 - 2026.01*, University of Illinois Urbana-Champaign, M.S. in Biomedical Image Computing (focus on AI for Imaging).
- *2020.09 - 2024.06*, Hong Kong Baptist University (Zhuhai), B.S. in Computer Science and Technology.

# 🎖 Honors and Awards
- *2023.09* Kaggle Silver Medal (Top 6%) — Bengali Speech Recognition from Out-of-Distribution Audio
- *2024.09* Lonnie Edelheit Scholarship
- *2023.12* Xu Jialu Whole Person Education Scholarship

# 🔬 Research Experience
- *2023.09 - 2024.06*, **Efficient Cubic Regional Attention Transformer (CRAT) for 3D Tumor Segmentation** (First Author)
  - Proposed a 3D cubic Transformer architecture that concentrates attention on informative regions by balancing latent weights and pruning irrelevant key–value pairs, matching baseline segmentation performance while cutting computational cost by over 75% (down to 25.45 GFLOPs); nominated to the FST Poster Conference, supervised by the Department Head, Prof. Weifeng Su.

# 💻 Projects
- **[SIM Card E-Commerce Platform](https://github.com/FocusWilliam/sim-card-shop)** ([Live Demo](http://3.16.157.181/)) — *2026.03 - 2026.04*
  - Full-stack prepaid SIM card storefront as 5 containerized services (NestJS/TypeScript API, Next.js 14 frontend, PostgreSQL, Redis, Nginx) on AWS EC2, with stateless JWT auth, decorator-based RBAC, and a Redis read-through cache on the highest-traffic endpoint.
  - Integrated Stripe Checkout with webhook-driven fulfillment, wrote 38 Jest unit/integration tests, and built a GitHub Actions CI/CD pipeline that cut deploy time from ~15 minutes to under 60 seconds.

- **Bengali Speech Recognition from Out-of-Distribution Audio** ([Kaggle Profile](https://www.kaggle.com/focuswilliam)) — *2023.09 - 2023.10*
  - Won a Kaggle Silver Medal (Top 6%) with a wav2vec-based speech pipeline extracting semantic representations from Bengali audio, fine-tuned with selective layer freezing for better generalization on unseen acoustic conditions.

<!-- 
# 💬 Invited Talks
- *2021.06*, Talk title.
-->
