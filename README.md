## Hi, I'm Ye-Seul Jang

Computer Vision / Machine Learning Engineer focused on deep learning for visual and signal data and on turning models into practical AI systems. My recent work covers detection, segmentation and classification pipelines, and real-time camera–projector applications for agricultural grading.

## VisionGrader Research Series

Two related but independent research projects on projection-guided produce grading: a camera detects and grades each item, and a projector displays the result directly on it. Each repository contains the model training and evaluation code and the real-time system.

### [LemonVision Grader](https://github.com/gondry-ai/lemonvision-grader)

Lemon detection, occlusion-aware target selection and 3-class grading (Best / Second / Juice), in two studies:

- **Cyberworlds 2026 (accepted):** single-sided grading in a projection-guided free-placement workspace (YOLO11n detection, EfficientNet-B0 grading).
- **Journal of Agriculture and Food Research (under review):** a two-stage workflow linking front- and back-side observations for packed harvest baskets. It combines RF-DETR Seg detection, a NORI + RDNet-Tiny occlusion classifier, and EfficientNet-B0 grading with logit averaging.

### [OkraVision Grader](https://github.com/gondry-ai/okravision-grader)

Okra pod grading (A / B / C) from a multi-stage pipeline: YOLOv8s-seg segmentation, YOLO11n-pose keypoints for length and curvature, an EfficientNet-B0 appearance-defect classifier, and a fixed rule-based fusion step. Research code and a real-time system; results so far are on a validation split only, with no independent test set or external field validation yet.

## Other Projects

### [EAG](https://github.com/gondry-ai/EAG): knee electroarthrography classification

PyTorch implementation accompanying a published study I co-authored ([Lee, Jang & Chang, *BMC Musculoskeletal Disorders*, 2025](https://doi.org/10.1186/s12891-025-08939-8)). The repository ports the published TensorFlow/Keras pipeline to PyTorch, checks it against the original with a parity test, and adds a subject-independent leave-one-subject-out benchmark that the paper did not perform.

### [FinBridgeAI](https://github.com/gondry-ai/finbridge-ai): bilingual banking onboarding MVP

A hackathon project ([2026 Finance AI Challenge](https://daker.ai/public/hackathons/2026-finance-ai-challenge)) that helps foreign residents in South Korea prepare for bank onboarding: English guidance for the customer and Korean summaries and status keywords for bank staff. The current MVP is **rule-based** (no LLM calls at runtime). It defines an `AiProvider` interface so LLM-backed features can be added later.
[**Live demo**](https://temporary-racing-olive-bilv8bc.vercel.app) (temporary deployment)

## Technical Skills

- **Computer vision:** object detection, instance segmentation, pose/keypoint estimation, image classification (YOLO, RF-DETR, EfficientNet)
- **Machine learning:** deep learning for images and time series, model evaluation, reproducible experiments
- **Languages and frameworks:** Python, PyTorch, TypeScript, React
- **Systems:** real-time camera–projector applications, OpenCV, PyQt5
