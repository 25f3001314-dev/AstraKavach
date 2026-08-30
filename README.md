# AstraKavach
Architecture and conceptual framework for ASTRAKAVACH: Autonomous Find-Patch-Prove for Indian Defence Software.
# AstraKavach
Architecture and conceptual framework for ASTRAKAVACH: Autonomous Find-Patch-Prove for Indian Defence Software.

**Overview**
A closed-loop cyber-reasoning system combining fuzzing, static/dynamic analysis, deterministic patching, and an offline LLM as a controlled patch assistant[cite: 1]. 

**Core Methodology**
Traditional-first, LLM-last: a closed loop that proves itself[cite: 1].
1. **Discover:** Find reproducible failures using tools like AFL++ and Atheris[cite: 1].
2. **Localize:** Turn failure into a repair target using ASan and Clang SA[cite: 1].
3. **Patch:** Attempt deterministic repair using CWE templates before utilizing an offline Qwen LLM[cite: 1].
4. **Prove:** Verify the fix holds using PoC Replay, pytest, and a 60s Re-fuzz[cite: 1].

**Mandated Stack**
* **Fuzzing:** AFL++, Atheris, ASan/UBSan[cite: 1]
* **Static Analysis:** Clang SA, Bandit, Semgrep, Joern[cite: 1]
* **LLM:** Quantized Qwen (Offline Inference)[cite: 1]

*Note: This repository currently holds the architectural framework and conceptual presentation for the qualifier phase.*
