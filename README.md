# codeeval


| Benchmark | Release / Focus Period | Description | Performance Improvements / Notes |
|---|---:|---|---|
| **SWE-Bench** | 2023 | Repo-level benchmark evaluating LLMs on resolving real GitHub issues by producing patches that pass project test suites. <br> **Paper:** https://arxiv.org/abs/2310.06770 <br> **GitHub:** https://github.com/SWE-bench/SWE-bench <br> **Dataset:** https://huggingface.co/datasets/princeton-nlp/SWE-bench <br> **Leaderboard:** https://www.swebench.com/ | Rapid improvement in resolve rates; evolved into an open community benchmark with variants like SWE-Bench Verified and Pro. |
| **SWE-Bench Pro** | 2024–2025 | Long-horizon, contamination-resistant enterprise-style SWE tasks with containerized execution. <br> **Paper:** https://arxiv.org/abs/2509.16941 <br> **GitHub:** https://github.com/scaleapi/SWE-bench_Pro-os <br> **Dataset:** https://huggingface.co/datasets/ScaleAI/SWE-bench_Pro <br> **Leaderboard:** https://scale.com/leaderboard/swe_bench_pro_public | Targets enterprise-grade realism: multi-file edits, long contexts, regression-free fixes. |
| **HumanEval (OpenAI)** | 2021 | Function-level Python benchmark (164 problems) with unit tests; introduced pass@k metric. <br> **Paper:** https://arxiv.org/abs/2107.03374 <br> **GitHub:** https://github.com/openai/human-eval <br> **Dataset:** Included in repo | Canonical baseline for code generation; widely used in LLM evaluation. |
| **MBPP (Mostly Basic Python Problems)** | 2021 | ~974 crowd-sourced Python programming problems with test cases. <br> **Paper:** https://arxiv.org/abs/2108.07732 <br> **GitHub:** https://github.com/google-research/google-research/tree/master/mbpp <br> **Dataset:** Included in repo | Measures basic coding competence; common secondary benchmark to HumanEval. |
| **APPS** | 2021 | Large-scale coding challenge benchmark (~10k problems) from competitive programming. <br> **Paper:** https://arxiv.org/abs/2105.09938 <br> **GitHub:** https://github.com/hendrycks/apps <br> **Dataset:** Included in repo | Tests reasoning across introductory, interview, and competition-level tasks. |
| **CodeXGLUE** | 2020 | Multi-task benchmark for code intelligence (translation, summarization, repair, classification). <br> **Paper:** https://arxiv.org/abs/2102.04664 <br> **GitHub:** https://github.com/microsoft/CodeXGLUE <br> **Website:** https://microsoft.github.io/CodeXGLUE/ | Widely used suite for comparing pretrained code models. |
| **CodeSearchNet** | 2019–2020 | Large multilingual dataset for semantic code search (NL ↔ code). <br> **Paper:** https://arxiv.org/abs/1909.09436 <br> **GitHub:** https://github.com/github/CodeSearchNet <br> **Dataset:** https://huggingface.co/datasets/code_search_net | Standard benchmark for code retrieval and embedding models. |
| **Project CodeNet** | 2021 | Massive dataset (~14M code samples, 55+ languages) for program analysis and synthesis. <br> **Paper:** https://arxiv.org/abs/2105.12655 <br> **Website:** https://developer.ibm.com/exchanges/data/all/project-codenet/ | Large-scale, multilingual evaluation resource. |
| **BigCodeBench** | 2024–2025 | Function-level benchmark with complex instructions and diverse API usage (1140 tasks). <br> **Paper:** https://arxiv.org/abs/2404.09970 <br> **GitHub:** https://github.com/bigcode-project/bigcodebench | Reveals large gap between AI and human coding performance. |
| **EDIT-Bench** | 2025 | Real-world code editing benchmark using in-the-wild developer edits. <br> **Paper:** https://arxiv.org/abs/2501.06789 <br> **GitHub:** https://github.com/edit-bench/edit-bench | Focuses on editing ≠ generation (refactors, fixes, incremental changes). |
| **CodeEditorBench** | 2024–2025 | Benchmark for code editing tasks such as debugging, polishing, and requirement switching. <br> **Paper:** https://arxiv.org/abs/2409.02099 <br> **GitHub:** https://github.com/CodeEditorBench/CodeEditorBench | Targets real-world IDE-style editing scenarios. |
| **ARCADE** | 2023 | NL→code benchmark for interactive data-science notebooks. <br> **Paper:** https://arxiv.org/abs/2305.11332 <br> **GitHub:** https://github.com/allenai/arcade | Evaluates stateful, multi-cell notebook reasoning. |
| **NumpyEval** | 2022 | Benchmark for NumPy-specific numerical programming tasks. <br> **Paper:** https://arxiv.org/abs/2211.09614 | Tests API-level correctness in numerical computing. |
| **PandasEval** | 2022 | Data-manipulation benchmark focused on Pandas workflows. <br> **Paper:** https://arxiv.org/abs/2210.14868 | Evaluates data-wrangling and dataframe reasoning. |
| **APIBench / Gorilla** | 2023 | Benchmarks for API invocation and tool-use accuracy. <br> **Paper:** https://arxiv.org/abs/2305.15334 <br> **GitHub:** https://github.com/ShishirPatil/gorilla | Core benchmark for tool-augmented LLMs. |
| **RepoBench** | 2023–2024 | Repository-level code completion and retrieval benchmark. <br> **Paper:** https://arxiv.org/abs/2306.03091 <br> **GitHub:** https://github.com/microsoft/RepoBench | Tests cross-file and repo-context understanding. |
| **ToolBench** | 2023–2024 | Multi-step tool-use benchmark for LLM agents. <br> **Paper:** https://arxiv.org/abs/2307.16789 <br> **GitHub:** https://github.com/OpenBMB/ToolBench | Measures planning and execution with external tools. |
| **SWT-Bench** | Oct 2024 | Benchmark for automated test generation and bug reproduction. <br> **Paper:** https://arxiv.org/abs/2406.12952 <br> **GitHub:** https://github.com/logic-star-ai/swt-bench | Focuses on testing agents rather than patch generation. |
| **CVE-Bench** | 2025 | Sandbox benchmark for exploiting and fixing real-world vulnerabilities. <br> **Paper:** https://arxiv.org/abs/2502.03289 | Highlights both capability and security risks of agents. |
| **τ-Bench (tau-bench)** | Jun 2024 | Multi-turn, tool-enabled agent benchmark with policy constraints. <br> **Paper:** https://arxiv.org/abs/2406.12045 <br> **GitHub:** https://github.com/sierra-research/tau-bench | Focuses on long-horizon reliability and rule-following. |
| **Terminal-Bench** | May 2025 | Terminal-based benchmark for multi-step command-line workflows. <br> **GitHub:** https://github.com/laude-institute/terminal-bench <br> **Website:** https://www.tbench.ai/ | Evaluates real shell competence and recovery. |
| **Context-Bench** | Oct 2025 | Agentic context engineering benchmark (long-running context, file chains). <br> **Paper:** https://arxiv.org/abs/2510.04618 | Evaluates cost–performance trade-offs in long-context agents. |
| **Spring AI Bench** | Oct 2025 | Enterprise Java / Spring ecosystem agent benchmark. <br> **GitHub:** https://github.com/spring-ai-community/spring-ai-bench | Domain-specific enterprise evaluation. |
| **DPAI Arena (JetBrains)** | Oct 2025 | Cross-ecosystem developer productivity benchmarking platform. <br> **Website:** https://dpaiarena.jetbrains.com <br> **Announcement:** https://blog.jetbrains.com/ | Evaluates end-to-end developer workflows. |
| **DS-1000** | 2023 | Data-science code generation benchmark (1000 tasks). <br> **Paper:** https://arxiv.org/abs/2301.13588 <br> **GitHub:** https://github.com/xlang-ai/DS-1000 | Focused on data-science APIs and notebook workflows. |





| Benchmark | Design Principles | Target Tasks | Evaluation Environments | Underlying Datasets |
|----------|------------------|--------------|--------------------------|---------------------|
| **SWE-Bench Pro** | Contamination-resistant; uses copyleft OSS and private commercial repositories to prevent training data overlap | Enterprise-grade software engineering tasks: bug fixes, feature requests, optimizations, security updates, UI/UX changes; moderate-to-large multi-file edits (avg. 107.4 LoC across 4.1 files) | Reproducible, containerized Docker-based environments with full dependencies | 1,865 instances across 41 professional repositories (731 public, 276 commercial, 858 held-out) |
| **SWE-Bench Verified** | Human-validated subset of SWE-Bench; removes underspecified issues and unfair tests | Resolving real-world GitHub issues from open-source Python projects | Containerized Docker environments | 500 samples from the original SWE-Bench test set (12 repositories) |
| **HumanEval** | Minimal, unit-test-based functional correctness | Function-level Python code generation from natural-language docstrings | Standard Python execution environment | Not explicitly detailed |
| **MBPP (Mostly Basic Python Problems)** | Focus on simplicity and basic coding competence | Short Python programs from simple natural-language descriptions | Standard Python execution environment | Not explicitly detailed |
| **MLE-Bench** | End-to-end evaluation of ML agents | Machine learning tasks (training, tuning, evaluation) | Not explicitly detailed | Tasks derived from 75 Kaggle competitions |
| **DS-1000** | Data-science–centric code generation | Data science problems across seven Python libraries | Not explicitly detailed | 1,000 curated data science problems |
| **BigCodeBench** | Instruction-following with complex APIs | Python coding problems with diverse function calls and complex instructions | Not explicitly detailed | 1,140 diverse Python questions |
| **ClassEval** | Manually designed for structural reasoning | Class-level code generation tasks | Not explicitly detailed | 100 manually crafted tasks |
| **SciCode** | Scientist-curated, research-oriented | Code generation for scientific research problems (math, physics, chemistry, biology, materials science) | Not explicitly detailed | 65 expert-curated problems |
| **APPS (Automated Programming Progress Standard)** | Competitive-programming–style difficulty scaling | Python programming tasks at introductory, interview, and competition levels | Not explicitly detailed | 1,000 introductory, 3,000 interview, 1,000 competition-level tasks |
| **AgentBench** | General-purpose agent evaluation | Evaluating LLMs as autonomous agents | Not explicitly detailed | Not explicitly detailed |
| **CORE-Bench** | Emphasis on scientific reproducibility | Computational reproduction of results from scientific papers | Not explicitly detailed | Not explicitly detailed |
| **USACO** | Olympiad-level rigor | Algorithmic programming problems across four difficulty levels | Not explicitly detailed | Official USA Computing Olympiad problem sets |
| Benchmark | Design Principles | Target Tasks | Evaluation Environments | Underlying Datasets |
|----------|------------------|--------------|--------------------------|---------------------|
| **SWE-Bench Pro** | Contamination-resistant; uses copyleft OSS and private commercial repositories to prevent training data overlap | Enterprise-grade software engineering tasks: bug fixes, feature requests, optimizations, security updates, UI/UX changes; moderate-to-large multi-file edits (avg. 107.4 LoC across 4.1 files) | Reproducible, containerized Docker-based environments with full dependencies | 1,865 instances across 41 professional repositories (731 public, 276 commercial, 858 held-out) |
| **SWE-Bench Verified** | Human-validated subset of SWE-Bench; removes underspecified issues and unfair tests | Resolving real-world GitHub issues from open-source Python projects | Containerized Docker environments | 500 samples from the original SWE-Bench test set (12 repositories) |
| **HumanEval** | Minimal, unit-test-based functional correctness | Function-level Python code generation from natural-language docstrings | Standard Python execution environment | Not explicitly detailed |
| **MBPP (Mostly Basic Python Problems)** | Focus on simplicity and basic coding competence | Short Python programs from simple natural-language descriptions | Standard Python execution environment | Not explicitly detailed |
| **MLE-Bench** | End-to-end evaluation of ML agents | Machine learning tasks (training, tuning, evaluation) | Not explicitly detailed | Tasks derived from 75 Kaggle competitions |
| **DS-1000** | Data-science–centric code generation | Data science problems across seven Python libraries | Not explicitly detailed | 1,000 curated data science problems |
| **BigCodeBench** | Instruction-following with complex APIs | Python coding problems with diverse function calls and complex instructions | Not explicitly detailed | 1,140 diverse Python questions |
| **ClassEval** | Manually designed for structural reasoning | Class-level code generation tasks | Not explicitly detailed | 100 manually crafted tasks |
| **SciCode** | Scientist-curated, research-oriented | Code generation for scientific research problems (math, physics, chemistry, biology, materials science) | Not explicitly detailed | 65 expert-curated problems |
| **APPS (Automated Programming Progress Standard)** | Competitive-programming–style difficulty scaling | Python programming tasks at introductory, interview, and competition levels | Not explicitly detailed | 1,000 introductory, 3,000 interview, 1,000 competition-level tasks |
| **AgentBench** | General-purpose agent evaluation | Evaluating LLMs as autonomous agents | Not explicitly detailed | Not explicitly detailed |
| **CORE-Bench** | Emphasis on scientific reproducibility | Computational reproduction of results from scientific papers | Not explicitly detailed | Not explicitly detailed |
| **USACO** | Olympiad-level rigor | Algorithmic programming problems across four difficulty levels | Not explicitly detailed | Official USA Computing Olympiad problem sets |

## Multi-layered Evaluation of Coding Agents

Evaluating the performance of coding agents requires a **multi-layered evaluation framework** that captures not only the correctness of generated code, but also reasoning quality, efficiency, security, and real-world usability. Such evaluations combine **quantitative metrics** (e.g., test pass rates, latency, cost) with **qualitative assessments** (e.g., human judgment, readability, safety) to ensure reliability, identify systematic failure modes, enable iterative improvement, and manage operational constraints.

Modern benchmarking frameworks (e.g., SWE-Bench Pro, SWE-Bench Verified, AgentBench) adopt this holistic perspective by integrating multiple KPIs across different abstraction levels—ranging from function-level correctness to repository-level task resolution and long-horizon agent behavior.

---

## Key Performance Indicators (KPIs) and Metrics

### 1. Correctness Metrics

**Exact Match**  
Measures how precisely an agent’s output aligns with an expected, predefined reference result. This metric is critical for tasks with a single correct output or strict formatting requirements.

**Semantic Correctness**  
Evaluates whether generated code or explanations are *factually and logically correct* beyond syntactic matching. This includes:
- **Faithfulness**: outputs are grounded in provided or retrieved context and avoid hallucinations.
- **Semantic Similarity**: embedding-based comparison that allows functionally equivalent but structurally different solutions.

Benchmarks such as **HumanEval** and **MBPP** implicitly evaluate both exact match (via unit tests) and semantic correctness.

**Pass@k**  
A standard metric in code generation benchmarks. An agent generates *k* independent solutions; if at least one passes all unit tests, the task is considered solved.  
In **SWE-Bench Pro**, a related concept is **Resolve Rate**, which requires fixing the issue while introducing no regressions.

---

### 2. Code Efficiency and Operational Metrics

**Efficiency and Step Count**  
Measures how efficiently an agent completes tasks by minimizing unnecessary actions and avoiding unproductive loops. Closely related is **Step Utility**, which ensures each action contributes meaningfully to progress.

**Latency**  
Total time from task submission to final output, including model inference, tool execution, and data retrieval.

**Cost**  
Computational resources consumed, such as token usage, API calls, and infrastructure costs—critical for real-world deployment.

---

### 3. Code Quality and Readability

**Readability (Clarity and Conciseness)**  
Assesses whether generated code and responses are well-structured, easy to understand, appropriately concise, and adhere to common coding conventions. Readable code is essential for maintainability and collaboration.

---

### 4. Security and Safety Metrics

**Robustness to Adversarial Inputs**  
Evaluates resilience against prompt injection, malicious inputs, or data poisoning.

**PII Detection**  
Ensures that agents do not leak personally identifiable or sensitive information.

**Vulnerability Detection / Introduction**  
Assesses an agent’s ability to identify existing vulnerabilities or avoid introducing new ones during code generation. Benchmarks such as **CVEBench** focus on this dimension.

---

### 5. Testing Metrics

**Test Coverage**  
Measures the extent to which generated or modified code is exercised by tests. A capable coding agent should either generate well-tested code or automatically produce tests for its outputs.

---

### 6. Human Evaluation

Human evaluation is indispensable for complex, nuanced, or safety-critical tasks that automated metrics cannot fully capture. Domain experts validate correctness, assess subtle quality attributes, judge safety and appropriateness, and uncover edge cases.

Frameworks such as **SWE-Bench Pro** and **SWE-Bench Verified** rely heavily on human review to ensure benchmark clarity, fairness, and real-world relevance. Human judgment often guides how quantitative metrics are interpreted.

---

### 7. Additional Metrics and Evaluation Strategies

Beyond core KPIs, several complementary metrics are commonly used:
- **Task Success Rate / Resolve Rate**
- **Agent Trajectory Quality**
- **Tool Selection Accuracy**
- **User Satisfaction**
- **Consistency**
- **Adaptability / Generalization**

Evaluation strategies include:
- **Automated Evaluation** (unit tests, BLEU, ROUGE, rule-based checks)
- **LLM-as-Judge Evaluation** for subjective quality assessment
- **Simulation-Based Evaluation** using controlled or synthetic environments
- **Online Evaluation** for continuous monitoring of deployed agents

---

## Summary Table: KPIs for Coding Agent Evaluation

| Category | Metric | What It Measures | Description | Example Benchmarks |
|--------|--------|------------------|-------------|--------------------|
| Correctness | Exact Match | Output precision | Exact alignment with expected outputs | HumanEval, MBPP |
| Correctness | Semantic Correctness | Meaning-level accuracy | Functional and factual correctness beyond syntax | HumanEval, SWE-Bench |
| Correctness | Faithfulness | Grounding | Avoidance of hallucinations; grounded outputs | SWE-Bench Pro |
| Correctness | Pass@k | Probabilistic success | At least one of *k* samples passes all tests | HumanEval, MBPP |
| Task Success | Resolve Rate | End-to-end completion | Issue resolved with no regressions | SWE-Bench Pro |
| Efficiency | Step Count / Utility | Action efficiency | Minimization of redundant or useless steps | AgentBench |
| Performance | Latency | Response time | End-to-end execution time | Production agents |
| Cost | Computational Cost | Resource usage | Tokens, API calls, infrastructure cost | Production agents |
| Code Quality | Readability | Maintainability | Clarity, structure, conciseness | Human evaluation |
| Security | Adversarial Robustness | Safety | Resistance to prompt injection and attacks | Security benchmarks |
| Security | PII Detection | Privacy | Avoidance of sensitive data leakage | Privacy audits |
| Security | Vulnerability Handling | Secure coding | Detecting or avoiding vulnerabilities | CVEBench |
| Testing | Test Coverage | Reliability | Portion of code covered by tests | SWE-Bench |
| Human Eval | Expert Judgment | Qualitative quality | Domain-specific correctness and safety | SWE-Bench Verified |
| Agent Behavior | Trajectory Quality | Reasoning quality | Coherence of multi-step decisions | AgentBench |
| Tool Use | Tool Accuracy | Tool effectiveness | Correct tool selection and usage | Tool-based agents |
| UX | User Satisfaction | Perceived value | User feedback and acceptance | Production systems |
| Reliability | Consistency | Stability | Output stability across runs | General evaluation |
| Generalization | Adaptability | OOD performance | Performance on novel tasks | AgentBench |
