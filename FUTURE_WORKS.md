\# Future Works and Research Roadmap



CrashSight establishes a foundational baseline for infrastructure-centric crash understanding. Based on our failure analysis, we outline the following actionable directions for future model development:



\## 1. Adaptive Visual Token Budgets

Current models suffer from temporal coverage loss due to uniform frame sampling. Future work should explore:

\* \*\*Event-driven Key Frame Selection:\*\* Concentrating temporal coverage around pre-crash and impact intervals.

\* \*\*Adaptive Sampling Algorithms:\*\* Dynamically allocating token budgets to moments of high physical interaction rather than static aftermaths.



\## 2. Unfreezing and Adapting Visual Encoders

Surveillance geometry (oblique angles, distant objects) is structurally out-of-distribution for models pretrained heavily on dashcam and web imagery. 

\* \*\*Domain Pretraining:\*\* Updating visual backbone weights to better parse wide-angle overhead footage.

\* \*\*Curriculum Learning:\*\* Staging training from coarse scene recognition to fine-grained mechanics-level attribution.



\## 3. Spatial Grounding and 3D-Aware Reasoning

Persistent failures in the \*Involved Parties\* and \*Accident Mechanics\* categories highlight the limitations of text-only QA supervision.

\* \*\*Explicit Spatial Grounding:\*\* Integrating bounding boxes and trajectory plotting directly into the VLM output.

\* \*\*Physics-Informed Perception:\*\* Connecting entity motion and collision mechanics through 3D-aware reasoning modules.



\## 4. Expanding the Evaluation Paradigm

While multiple-choice VQA ensures reproducibility, it does not fully capture the complexity of forensic investigation.

\* \*\*Multi-Turn QA:\*\* Stress-testing model consistency through sequential questioning.

\* \*\*Explanatory Generation:\*\* Requiring models to generate structured, multi-step causal explanations alongside their answers.

