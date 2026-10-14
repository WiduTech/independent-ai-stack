# AI Model Landscape Analysis
**WiduTech — Independent AI**  
**Last updated: October 2026**

A comprehensive analysis of all major AI models — both the closed commercial giants and the open source alternatives tested for an Independent AI service.

---

## Part 1: The Closed Commercial Giants

These models are powerful, but all share the same fundamental problem: **your data leaves your infrastructure and goes to US servers**.

---

### 🟠 OpenAI — GPT Family
**Company:** OpenAI 🇺🇸 (Microsoft-backed)  
**License:** Proprietary, closed source  
**Data:** Sent to OpenAI servers (US)

#### Current Models (October 2026):

| Model | Context | Best For | Price (per 1M tokens) |
|-------|---------|----------|----------------------|
| **GPT-5.5** | 400K | Most capable, complex reasoning | ~$15 input / $60 output |
| **GPT-5.6 Sol** | 400K | Complex reasoning, professional workflows | Premium |
| **GPT-5.6 Terra** | 400K | Balanced general use | Mid-range |
| **GPT-5.6 Luna** | 400K | Fast, cost-sensitive workloads | Low |
| **GPT-5 Mini** | 400K | Everyday tasks, fast | Low |
| **GPT-5 Nano** | 400K | High volume, simple tasks | Very low |

**Key characteristics:**
- GPT-5 is a "unified system" — internal router decides which tier to use based on query complexity
- Strong coding, math, multimodal (text + images)
- Tool use and function calling
- Excellent multilingual support
- Context window: 272K input + 128K output

**WiduTech verdict:**
> ❌ **Not suitable for government.** All queries and documents sent to Microsoft/OpenAI US servers. CLOUD Act applies. No data sovereignty. No auditability of the model itself.

---

### 🔵 Anthropic — Claude Family
**Company:** Anthropic 🇺🇸 (Amazon-backed)  
**License:** Proprietary, closed source  
**Data:** Sent to Anthropic servers (US)

#### Current Models (October 2026):

| Model | Context | Best For | Price (per 1M tokens) |
|-------|---------|----------|----------------------|
| **Claude Fable 5.1** | 1M | Absolute frontier, research | $10 / $50 |
| **Claude Opus 5.5** | 1M | Complex reasoning, coding | $4 / $20 |
| **Claude Sonnet 5.5** | 1M | Best balance, daily use ⭐ | $2 / $10 |
| **Claude Haiku 4.5** | 1M | Fast, cost-efficient | $1 / $5 |

**Key characteristics:**
- 1 million token context window (largest in class)
- Claude Sonnet 5.5 preferred over Opus 5 (older) by developers 59% of the time
- Outstanding at long document analysis, coding, writing
- Excellent instruction following
- Strong safety alignment
- No open source weights

**WiduTech verdict:**
> ❌ **Not suitable for EU government and public sectors.** Amazon-backed US company. All data processed on US infrastructure. 

---

### 🟢 Google — Gemini Family
**Company:** Google/Alphabet 🇺🇸  
**License:** Proprietary, closed source  
**Data:** Sent to Google servers (US)

#### Current Models (October 2026):

| Model | Context | Best For | Notes |
|-------|---------|----------|-------|
| **Gemini 3.1 Pro** | 1M+ | Current flagship | Best multimodal |
| **Gemini Ultra** | 1M+ | Most capable | Google One AI Ultra plan |
| **Gemini Flash** | 1M | Fast, efficient | High volume tasks |

**Key characteristics:**
- Best multimodal model (text, image, video, audio, code)
- 1M+ context window
- Trained on Google's massive data infrastructure
- Deep integration with Google Workspace (massive risk)
- Gemma (open weights version) uses restrictive Gemma license

**WiduTech verdict:**
> ❌ **Not suitable for EU government and public sectors.** Google's entire business model is data analysis. Using Gemini while on Google Workspace means your internal data feeds directly into Google's AI. Maximum sovereignty risk. Gemma (open weights) excluded due to Gemma license restrictions.

---

### 🟣 xAI — Grok Family
**Company:** xAI 🇺🇸 (Elon Musk)  
**License:** Proprietary  
**Data:** Sent to xAI servers (US)

| Model | Notes |
|-------|-------|
| **Grok 4.7** | Current flagship, competitive with GPT-5.5 |

**WiduTech verdict:**
> ❌ Not suitable. US company, proprietary, cloud-only.

---

### � Microsoft — Copilot Family
**Company:** Microsoft 🇺🇸  
**License:** Proprietary, closed source  
**Data:** Sent to Microsoft servers (US)  
**Underlying models:** OpenAI GPT-5.x family (Microsoft has exclusive commercial license)

#### Current Models (October 2026):

Microsoft 365 Copilot now uses **GPT-5.6** as the preferred model across all apps (Word, Excel, PowerPoint, Teams, Outlook, Chat). The system automatically routes between:
- **GPT-5.6 Sol** — Complex reasoning, strategic insights
- **GPT-5.6 Terra** — Balanced everyday work
- **GPT-5.6 Luna** — Fast, high-volume tasks

**Previous versions still available in Copilot Studio:**
- GPT-5.4 Thinking — Deep reasoning on technical prompts
- GPT-5.2 — General work tasks
- GPT-5 — Original release

#### Pricing (October 2026):

| Plan | Price/user/month | Requires | Notes |
|------|-----------------|----------|-------|
| **Microsoft 365 Copilot** | $30 | Microsoft 365 E3/E5 or Business Premium | Standard enterprise |
| **Copilot Business** | $21 | Microsoft 365 Business Standard | SMB tier |
| **Business Standard + Copilot** | $23.50 | Bundled | New July 2026 SKU |
| **Business Premium + Copilot** | $32 | Bundled | New July 2026 SKU |
| **E7 Frontier Suite** | $99 | Enterprise | Includes Copilot + advanced features |

**Additional costs:**
- Requires qualifying Microsoft 365 base license ($8–$57/user/month depending on tier)
- **Total cost:** $38–$87/user/month for most government institutions and public sectors.

**For a 100-person Belgian municipality:**
- Copilot: $30 × 100 = **$3,000/month** = **€33,000/year**
- Plus M365 E3 base licenses: ~$36/user/month = **€39,000/year**
- **Total: ~€72,000/year** (before VAT)

#### Key characteristics:
- Deeply integrated into Microsoft 365 apps (Word, Excel, PowerPoint, Outlook, Teams)
- Analyzes emails, documents, meetings, chats across the tenant
- Can summarize years of communications automatically
- No opt-out at document level — if Copilot is enabled, it can see everything in M365
- All processing happens on Microsoft US servers
- Uses OpenAI models exclusively (Microsoft partnership)

#### The AI Risk Angle (from WiduTech's positioning):

Before Copilot, the risk of data on Microsoft 365 was:
- US CLOUD Act applies to data at rest
- Manual extraction required to understand document contents at scale

**With Copilot, the risk fundamentally changes:**
- AI can now automatically analyze years of emails, meeting notes, internal docs
- Pattern recognition across unstructured data happens automatically
- What was practically difficult (understanding organizational decisions from scattered documents) is now trivial
- The same infrastructure hosting your data now understands it at scale

**This is the Belgian government use case:**
> A municipality stores 10 years of internal communications, citizen correspondence, policy discussions, and budget documents on Microsoft 365. With Copilot, queries like "summarize all internal discussions about the social housing budget over the last 5 years" become possible. The AI that can answer that question has already read and indexed those documents. That AI runs on US servers, subject to US legal jurisdiction.

#### WiduTech verdict:
> ❌ **Highest sovereignty risk for EU governments and public sectors.** Not just storage, but AI-powered analysis of your entire organizational memory on US infrastructure. This deepens the dependency on US infrastructure more than anyone has thought before.

---

### �🔴 Mistral AI — Commercial Tier
**Company:** Mistral AI 🇫🇷  
**License:** Commercial API (proprietary at API level)  
**Data:** Sent to Mistral servers (France/EU)

#### Current Models (October 2026):

| Model | Parameters | Context | Notes |
|-------|-----------|---------|-------|
| **Mistral Large 4** ("le Chonk") | 1.05T total / 52B active | 1M | Brand new — Oct 6 2026 |
| **Mistral Small 4** | 24B | 128K | Fast, efficient |

**Mistral Large 4 — Breaking News:**
- Just launched October 6, 2026 (this week!)
- 1.05 trillion parameters (MoE, 52B active per token)
- 1 million token context window
- Multimodal (text + images)
- **Open weights promised by end of October 2026**
- Price: $1.36 input / $4.18 output per million tokens
- Benchmark score jumped from 9.3 to 38.4 (Artificial Analysis)
- **This will be the most powerful open source model when weights release**

**WiduTech verdict:**
> ⚠️ **API = cloud, not self-hosted.** BUT: open weights releasing end of October 2026 means you will be able to run Mistral Large 4 locally. This is a game-changer for EU's Independent AI landscape. Watch this space very closely.

---

## Part 2: Open Source / Self-Hostable Models

These models can run on your own infrastructure. Your data never leaves your building.

---

### 🇫🇷 Mistral Family (Mistral AI, France)
**License:** Apache 2.0 ✅  
**Self-hostable:** Yes

| Model | Parameters | Size | Context | Notes |
|-------|-----------|------|---------|-------|
| **Mistral 7B** | 7B | 4.4 GB | 32K | Fast, efficient |
| **Mistral Nemo 12B** | 12B | 7.1 GB | 128K | Best balance — installed |
| **Mixtral 8x7B** | 47B (8B active) | 26 GB | 32K | Too slow for Mac Studio |
| **Mistral Large 4** | 1.05T | TBD | 1M | Open weights ~end Oct 2026 |

**Dutch/French quality:** Good (French company, strong European language training)  
**Best use for WiduTech:** General purpose conversations, demos where EU origin matters

---

### 🇨🇳 Qwen Family (Alibaba)
**License:** Apache 2.0 ✅  
**Self-hostable:** Yes

| Model | Parameters | Size | Context | Notes |
|-------|-----------|------|---------|-------|
| **Qwen2.5:7b** | 7B | 4.7 GB | 128K | Fast |
| **Qwen2.5:14b** | 14B | 8.9 GB | 128K | **Best general model for Mac Studio** ⭐ |
| **Qwen2.5:32b** | 32B | 19 GB | 128K | High quality, slower |
| **Qwen2.5:72b** | 72B | 41 GB | 128K | Best quality, needs large RAM |
| **Qwen2.5-Coder:7b** | 7B | 4.9 GB | 128K | **Best coding model for Mac Studio** ⭐ |
| **Qwen3-235B-A22B** | 235B total / 22B active | Large | 128K | Flagship MoE, not local |

**Dutch/French quality:** Excellent (strongest multilingual of all tested models)  
**Best use for WiduTech:** General purpose, document analysis, coding, social media posts

---

### 🇪🇺 EuroLLM (European Research Consortium)
**License:** Apache 2.0 ✅  
**Self-hostable:** Yes  
**Developers:** Unbabel, IST Lisbon, U. Edinburgh, U. Paris-Saclay, U. Amsterdam, Naver Labs, Sorbonne  
**Funded by:** European Union  
**Trained on:** MareNostrum 5 supercomputer (EuroHPC)

| Model | Parameters | Size | Context | Notes |
|-------|-----------|------|---------|-------|
| **EuroLLM-1.7B** | 1.7B | ~1 GB | 4K | Fast, lightweight |
| **EuroLLM-9B** | 9B | 5.6 GB | 4K | **Official EU model, installed** ⭐ |
| **EuroLLM-22B** | 22B | 13 GB (Q4) | 32K | Best EU model, needs manual install |

**Dutch/French quality:** Very good (all 24 EU official languages)  
**Best use for WiduTech:** Government demos — emphasizes EU sovereignty, trained from scratch (not Google/Meta derivative)  
**Limitation:** Does not support function calling/tools — use in Open WebUI only, not Kilo Code

---

### 🌍 StarCoder 2 (BigCode)
**License:** Apache 2.0 ✅  
**Self-hostable:** Yes

| Model | Parameters | Size | Notes |
|-------|-----------|------|-------|
| **StarCoder2:3b** | 3B | 1.9 GB | Fast |
| **StarCoder2:7b** | 7B | 4 GB | Best balance |
| **StarCoder2:15b** | 15B | 8.5 GB | High quality |

**Best use for WiduTech:** Legacy code analysis, IT modernization demos, 600+ programming languages

---

### 🇨🇭 Meditron (EPFL, Switzerland)
**License:** Apache 2.0 ✅  
**Self-hostable:** Yes

| Model | Parameters | Notes |
|-------|-----------|-------|
| **Meditron-7b** | 7B | In Ollama library |
| **Meditron-70b** | 70B | Manual install needed |

**Limitation:** Base/pretrained model only — not instruction-tuned for chat. Completes text rather than answering questions. Needs fine-tuning for production use.  
**Best use for WiduTech:** Research context only, or as a base for fine-tuning on Belgian medical guidelines

---

### 🇨🇳 Kimi Family (Moonshot AI)
**License:** Open weights  
**Self-hostable:** Only K2 family

| Model | Parameters | Self-hostable | Notes |
|-------|-----------|--------------|-------|
| **Kimi K2** | 1T total / 32B active | ✅ (needs ~200GB RAM) | Open weights |
| **Kimi K2.5** | 1T total / 30B active | ✅ (needs ~180GB RAM) | Open weights |
| **Kimi K2.6** | 1T total / 32B active | ⚠️ Cloud or large hardware | Open weights or cloud |
| **Kimi K3** | 2.8T total / 104B active | ❌ Needs 650GB+ RAM | Cloud only in practice |

**WiduTech verdict:** K2 family is open but requires enterprise hardware (200GB+ RAM). Cannot run on local machines but can on an enterprise setting.

---

## Part 3: Side-by-Side Comparison

### For local machine (Mac Studio M1 (32GB RAM))

| Model | Type | Size | Dutch/FR | Tools | Best For |
|-------|------|------|----------|-------|----------|
| **Qwen2.5:14b** | General | 8.9 GB | ⭐⭐⭐⭐⭐ | ✅ | Everything — best all-rounder |
| **Qwen2.5-Coder:7b** | Coding | 4.9 GB | ⭐⭐⭐ | ✅ | VSCodium/Kilo Code |
| **Mistral Nemo 12B** | General | 7.1 GB | ⭐⭐⭐ | ✅ | Fast general use |
| **EuroLLM-9B** | General | 5.6 GB | ⭐⭐⭐⭐ | ❌ | Gov demos, EU sovereignty |
| **EuroLLM-22B** | General | 13 GB | ⭐⭐⭐⭐⭐ | ❌ | Best EU model locally |
| **StarCoder2:7b** | Coding | 4 GB | ⭐⭐ | ✅ | Legacy code analysis |
| **Meditron:7b** | Medical | 4.7 GB | ⭐⭐ | ❌ | Research only, not chat |
| **Mixtral 8x7B** | General | 26 GB | ⭐⭐⭐⭐ | ❌ | Too slow — remove it |

---

### Frontier Closed vs Best Open Source

| Capability | Best Closed | Best Open Source | Gap |
|------------|-------------|-----------------|-----|
| **General reasoning** | Claude Opus 5.5 | Qwen2.5:72b | Significant |
| **Coding** | GPT-5.5 | Qwen3-Coder 480B | Small |
| **Multilingual** | Gemini 3.1 Pro | Qwen2.5:72b | Small |
| **EU languages** | Claude Sonnet 5.5 | EuroLLM-22B | Medium |
| **Long context** | Claude Fable 5.1 (1M) | Mistral Large 4* (1M) | None* |
| **Data sovereignty** | N/A | All open source | Open source wins |
| **Auditability** | None | Full | Open source wins |
| **Cost at scale** | High API costs | Hardware only | Open source wins |

*Mistral Large 4 open weights expected end of October 2026

---

## Part 4: The WiduTech Decision Framework

### When to Use What:

**For government:**
→ EuroLLM-22B or EuroLLM-9B  
→ Messaging: "EU-funded, EU-trained, fully auditable, never leaves your server"

**For document analysis and general questions:**
→ Qwen2.5:14b  
→ Best multilingual quality, fits Mac Studio

**For coding and DevOps:**
→ Qwen2.5-Coder:7b in Kilo Code/VSCodium

**For creative writing and social posts:**
→ Qwen2.5:14b or Mistral Nemo with a good system prompt

**For medical healthcare:**
→ Qwen2.5:14b with medical system prompt

---

## Part 5: What to Watch

### Near-term (October-December 2026):

1. **Mistral Large 4 open weights** (end of October 2026)
   - 1T parameter model, fully open source, Apache 2.0
   - Will be the most powerful self-hostable model available
   - Too large for Mac Studio (needs ~600GB+ RAM) but deployable on Kubernetes

2. **EuroLLM larger models**
   - Team announced more powerful models with multimodal capabilities in development
   - Will strengthen the EU sovereignty further

3. **Qwen3.5 and beyond**
   - Alibaba continues rapid iteration
   - Apache 2.0 on mid-size models
   - Best open source multilingual keeps improving

### Longer term:

- The gap between open source and closed models is closing rapidly
- By 2027, open source models will likely match closed models for most government and public sector use cases
- EU AI Act compliance will increasingly favor auditable open source models

---

## Part 6: ROI

Lcal deployment pays off at scale:

| Model | Input (per 1M tokens) | Output (per 1M tokens) |
|-------|----------------------|------------------------|
| Claude Fable 5.1 | $10 | $50 |
| Claude Opus 5.5 | $4 | $20 |
| Claude Sonnet 5.5 | $2 | $10 |
| Claude Haiku 4.5 | $1 | $5 |
| GPT-5.5 | ~$15 | ~$60 |
| Mistral Large 4 | $1.36 | $4.18 |
| Gemini 3.1 Pro | ~$3.50 | ~$10.50 |

**1 million tokens ≈ ~750,000 words ≈ roughly 1,500 pages of text**

A government institution processing 100M tokens/month (moderate use) would pay:
- Claude Sonnet: **€180,000/year**
- GPT-5.5: **€540,000+/year**
- Self-hosted Qwen2.5:14b: **€0/year** (hardware cost only, already owned, see part 8 of this document)

---

*Document maintained by WiduTech*  
*"We do tech. You stay independent."*

---

## Part 7: Do Open Source Models Phone Home?

This is a critical question for the sovereignty positioning. The answer has two layers: the **model weights** themselves, and the **infrastructure** running them.

---

### The Model Weights — Short Answer: No

When you run Qwen, Mistral, EuroLLM or any other open source model via Ollama locally:

- The weights are static files on your disk — math, not software
- They have no network stack, no ability to initiate connections
- They cannot phone home because they are not programs — they are data
- The model itself is incapable of exfiltrating anything

**This is verifiable.** Apache 2.0 license requires the source to be published. The weights are on Hugging Face. Researchers worldwide audit them. If Alibaba had embedded a backdoor in Qwen's weights, it would be found.

---

### Ollama — The Runtime Layer

Ollama is what actually runs on your machine and serves the model. This matters more:

**What Ollama does NOT do:**
- ❌ Does not collect, store or transmit your prompts
- ❌ Does not log your conversations
- ❌ Does not send queries to any external server
- ❌ No analytics on your usage

**What Ollama DOES do:**
- ⚠️ The **desktop tray app** checks `ollama.com` hourly for updates
- ✅ The **headless server** (`ollama serve`) makes zero outbound connections
- ✅ All model inference stays on `localhost:11434`

**For government deployments:** Run Ollama in headless server mode only (no desktop tray app). Zero outbound connections. Fully air-gapped if needed.

**Verified from:** Ollama's privacy policy explicitly states: *"Ollama runs on your local device. We do not collect, store, transmit, or have access to your prompts, responses, model interactions, or other content you process locally."* Ollama is open source — this is code-verifiable.

---

### Open WebUI

- Open source (MIT license)
- Stores conversations in local SQLite/PostgreSQL
- No external connections for core functionality
- ⚠️ Optional features like web search DO make outbound calls — disable these for air-gapped deployments
- All data stays in your infrastructure

---

### The Chinese Model Question Specifically

**Qwen (Alibaba):**
- Weights are Apache 2.0, published on Hugging Face
- No network capability in the weights themselves
- Alibaba has no access to your inference once weights are downloaded
- Running via Ollama = zero connection to Alibaba

**EuroLLM:**
- EU-funded research consortium
- Weights on Hugging Face under Apache 2.0
- No telemetry possible

**The honest nuance:**
> The weights are safe. The risk is in how you run them. A poorly configured Open WebUI with web search enabled, running on a cloud server with loose firewall rules, is a risk — not because of the model, but because of the infrastructure.
---

### What DOES Phone Home (For Reference)

| Tool | Phones Home? | Notes |
|------|-------------|-------|
| Ollama headless server | ❌ No | Fully silent |
| Ollama desktop tray app | ⚠️ Update checks | To ollama.com only, hourly |
| Open WebUI | ❌ No | Local only |
| LM Studio | ⚠️ Yes | Closed source, update + opt-out usage stats |
| Model weights (any) | ❌ No | Static files, no network capability |
| Microsoft 365 Copilot | ✅ Always | All content to Microsoft US servers |
| ChatGPT / OpenAI API | ✅ Always | All content to OpenAI US servers |

---

### Recommendation for Air-Gapped Deployments

For high-security institutions (federal government, healthcare, defence):

1. Download model weights once on a connected machine
2. Transfer to air-gapped network via USB/internal transfer
3. Run Ollama headless server only (no tray app)
4. Block outbound internet at firewall level
5. Open WebUI with web search and image generation disabled
6. All traffic stays on internal network

This gives you **zero outbound connections** — fully verifiable, fully auditable.

---

## Part 8: Hardware Cost Analysis

Running self-hosted AI has an upfront hardware cost but eliminates ongoing API fees. Here's the full breakdown across three deployment models.

---

### Option A: Mac Studio (Apple Silicon)

**Why Mac Studio for AI:**
- Unified memory architecture — GPU and CPU share the same RAM pool
- 32GB unified memory handles models up to ~20GB efficiently
- 96GB/192GB Ultra models handle 70B+ parameter models
- Native Metal acceleration for Ollama
- Silent, low power (~30W idle, ~150W under load)
- No driver/CUDA complexity

**Current Mac Studio Pricing (October 2026):**

| Model | Memory | Price (New) | Price (Refurb) | Best For |
|-------|--------|------------|----------------|----------|
| M1 Max (yours) | 32GB | N/A (discontinued) | ~€1,300 | 14B models, demos |
| M2 Max | 32GB | N/A (discontinued) | ~€1,600 | 14B models |
| M2 Ultra | 64GB | N/A (discontinued) | ~€3,800 | 70B models |
| M2 Ultra | 128GB | N/A (discontinued) | ~€5,500 | 70B+ models |
| **M5 Max** | **64GB** | **€2,499** | - | **Sweet spot 2026** |
| **M5 Ultra** | **128GB** | **€5,499** | - | **70B models** |
| **M5 Ultra** | **192GB** | **€7,999** | - | **Full frontier models** |

**Running costs:**
- Power: ~€150/year (30W average × 24/7 × €0.30/kWh)
- Maintenance: Near zero (no moving parts, no fans issues)
- Total 3-year TCO (M5 Max 64GB): ~€2,949

**Capacity with M5 Max (64GB):**
- Qwen2.5:14b ✅ (fast)
- EuroLLM-22B ✅ (good)
- Qwen2.5:32b ✅ (comfortable)
- 70B models ⚠️ (slow, needs quantization)

**Capacity with M5 Ultra (192GB):**
- All models up to 70B ✅ (fast)
- Mistral Large 4 (when weights release) ✅ (52B active parameters)
- Multiple models simultaneously ✅

---

### Option B: Dedicated Linux Server (On-Premise)

For institutions wanting a proper server in their own data center or server room.

**NVIDIA GPU Server Options:**

| GPU | VRAM | Server Price | Best For |
|-----|------|-------------|----------|
| RTX 4090 | 24GB | ~€4,000–€6,000 | Small teams, 14B–30B models |
| RTX 4000 Ada | 20GB | ~€3,500–€5,000 | Efficient inference |
| A100 40GB | 40GB | ~€8,000–€15,000 | 70B models, production |
| A100 80GB | 80GB | ~€15,000–€25,000 | Large models, high throughput |
| H100 | 80GB | €25,000–€40,000 | Frontier models, enterprise |

**Full server build (recommended for most Belgian governments):**
- 2× RTX 4090 + server chassis + RAM + storage
- Total: ~€10,000–€15,000
- Handles: All models up to 70B with 2-GPU setup
- Runs: 20–50 concurrent users with vLLM

**Running costs (on-premise server, Belgium):**
- Power: ~€1,200–€2,400/year (300–600W × 24/7 × €0.30/kWh)
- Rack space/cooling: depends on existing infrastructure
- Maintenance: ~€500–€1,000/year

**3-year TCO:** €15,000–€25,000 (hardware + power + maintenance)

---

### Option C: European Cloud Hosting

For institutions who want managed infrastructure without buying hardware.

**Hetzner (Germany 🇩🇪) — Best Value for EU**

| Server | GPU | VRAM | Price/month | Best For |
|--------|-----|------|------------|----------|
| GEX44 | RTX 4000 Ada | 20GB | €184/month | Small deployments |
| Custom dedicated | A100 80GB | 80GB | ~€800–€1,200/month | Production |

**OVHcloud (France 🇫🇷)**
- GPU instances from ~€2.50/hour
- Bare metal GPU servers available
- EU data centers (Paris, Frankfurt, Warsaw)
- H100 available at ~€6–€8/hour

**Cloud GPU spot pricing (for reference):**

| Provider | GPU | Price/hour | EU Data Center? |
|----------|-----|-----------|----------------|
| Hetzner | RTX 4000 Ada | ~€0.50/hr | ✅ Germany |
| OVHcloud | A100 | ~€2.50/hr | ✅ France |
| RunPod | A100 | ~€0.43/hr | ⚠️ US/EU mixed |
| Lambda | H100 | ~$2.49/hr | ❌ US only |

**⚠️ Important for WiduTech:** US cloud providers (AWS, GCP, Azure) are excluded — same sovereignty problem as the software. Stick to Hetzner or OVHcloud for European hosting.

---

### ROI Comparison: Self-Hosted vs API (Per Year)

Based on a medium-sized Belgian municipality (50 staff, moderate AI use):
- Estimated usage: ~50 million tokens/month = 600M tokens/year

| Solution | Year 1 Cost | Year 2 Cost | Year 3 Cost | 3-Year Total |
|----------|------------|------------|------------|-------------|
| **ChatGPT (GPT-5.5)** | €54,000 | €54,000 | €54,000 | **€162,000** |
| **Claude Sonnet 5.5** | €18,000 | €18,000 | €18,000 | **€54,000** |
| **Microsoft Copilot** | €12,000+ | €13,000+ | €14,000+ | **€39,000+** |
| **Mac Studio M5 Ultra** | €8,500* | €200 | €200 | **€8,900** |
| **Linux GPU Server** | €17,000* | €1,500 | €1,500 | **€20,000** |
| **Hetzner cloud (EU)** | €2,208 | €2,208 | €2,208 | **€6,624** |

*Hardware + setup cost included

**The self-hosted break-even point:**
- vs Claude: ~6 months
- vs GPT-5.5: ~2 months
- vs Microsoft Copilot: ~12–18 months

---

### Recommended Hardware by institution's Size

| Institution Size | Users | Recommended Hardware | Estimated Setup Cost |
|-------------|-------|---------------------|---------------------|
| Small municipality | <20 | Mac Studio M5 Max (64GB) | €2,500–€3,500 |
| Medium municipality | 20–100 | Mac Studio M5 Ultra (128GB) or Linux + 2× RTX 4090 | €6,000–€15,000 |
| Large government org | 100–500 | Dedicated GPU server or EU cloud | €20,000–€50,000 |
| Regional government | 500+ | Multi-GPU cluster or EU cloud (Hetzner/OVH) | Custom |

---

### WiduTech Positioning on Hardware

WiduTech does not sell hardware — we recommend and configure it. Our value is:

1. Selecting the right hardware for the government's or institution's actual usage
2. Deploying and configuring the full stack
3. Ensuring zero data leakage at infrastructure level
4. Training staff on the deployed system

For the audit deliverable, include a hardware recommendation section with TCO analysis. The ROI argument is often what closes the deal.

---

*Document maintained by WiduTech*  
*"We do tech. You stay independent."*
