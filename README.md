## Hi, I'm Ye-Seul Jang

Ph.D. researcher in System Integration Engineering at the University of Yamanashi, Japan, affiliated with Mao Laboratory (MaoLab). I work on computer vision and deep learning, and on turning models into practical AI systems, from detection and segmentation pipelines to real-time camera–projector applications.

## VisionGrader Research Series

Two related but independent computer vision research projects on projection-guided produce grading: a camera detects and grades each item, and a projector displays the result directly on it. Each repository contains the model training and evaluation code and the real-time system.

### [LemonVision Grader](https://github.com/gondry-ai/lemonvision-grader)

Lemon detection, occlusion-aware target selection and 3-class grading (Best / Second / Juice), in two studies:

- **Cyberworlds 2026 (accepted):** single-sided grading in a projection-guided free-placement workspace (YOLO11n detection, EfficientNet-B0 grading).
- **Journal of Agriculture and Food Research (under review):** a two-stage workflow linking front- and back-side observations for packed harvest baskets. It combines RF-DETR Seg detection, a NORI + RDNet-Tiny occlusion classifier, and EfficientNet-B0 grading with logit averaging.

### [OkraVision Grader](https://github.com/gondry-ai/okravision-grader)

Okra pod grading (A / B / C) from a multi-stage pipeline: YOLOv8s-seg segmentation, YOLO11n-pose keypoints for length and curvature, an EfficientNet-B0 appearance-defect classifier, and a fixed rule-based fusion step. Research code with a real-time system; results so far are on a validation split only, with no independent test set or external field validation yet.

## Other Projects

### [EAG](https://github.com/gondry-ai/EAG): biomedical signal classification

Knee electroarthrography (EAG) classification research that began during my master's studies and led to a published study I co-authored ([Lee, Jang & Chang, *BMC Musculoskeletal Disorders*, 2025](https://doi.org/10.1186/s12891-025-08939-8)). The repository is a PyTorch reimplementation of the original TensorFlow/Keras pipeline, checked against it with a parity test, plus an additional subject-independent leave-one-subject-out evaluation that the paper did not perform.

### [FinBridgeAI](https://github.com/gondry-ai/finbridge-ai): bilingual banking onboarding MVP

An AI-extensible, bilingual banking onboarding MVP for foreign residents in South Korea, developed for the [2026 Finance AI Challenge](https://daker.ai/public/hackathons/2026-finance-ai-challenge). It gives customers English guidance and bank staff Korean summaries and status keywords. The current implementation is **rule-based**, with no LLM calls at runtime. It defines an `AiProvider` interface so LLM-backed features could be integrated in the future.

## Technical Skills

- **Languages:** Python, TypeScript
- **Frameworks:** PyTorch, TensorFlow/Keras
- **Computer Vision:** Classification, Object Detection, Instance Segmentation, Keypoint Estimation
- **Architectures:** CNNs, Transformers, YOLO, RF-DETR
- **Machine Learning:** Time-Series Classification, Model Evaluation, Data Preprocessing
- **Tools:** OpenCV, Git, Linux, React, Vite
