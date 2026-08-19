<div align="center">

# Hi, I'm Beau David

### AI / Computer Vision Engineer | Junior AI Software Engineer

Hi There!, This is Bryan David,  I m building production-grade computer vision and deep learning systems — from dataset curation and model training to full-stack deployment.
Currently exploring LLM fine-tuning and multimodal architectures under the **Aegis** project portfolio.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/beaunix)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/BeauBryanDev)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bryan.beau.186@gmail.com)
[![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD133?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/beaunixer)
[![Location](https://img.shields.io/badge/Bogota,_Colombia-000000?style=for-the-badge&logo=googlemaps&logoColor=white)]()

</div>

---

## About Me

I'm a self-taught developer based in Colombia, focused on computer vision, deep learning, and full-stack ML system design. My work centers on a portfolio of independent projects under the **Aegis** brand — real-time detection systems, segmentation models, and anomaly detection pipelines — each shipped as a complete product: trained model, backend API, and frontend dashboard.

I'm currently:
- Building **Aegis Scientist**, an expert LLM for industrial boiler systems and CFD simulation, with a curated 40K-record training dataset
- Developing **Aegis MLOps**, a full-stack ML lifecycle on every project: data curation, training, evaluation, ONNX export, and production deployment (FastAPI/Crow + PostgreSQL + AWS EC2)
- Fine tuning **Aegis CyberSec-Guard**, a LLM for detecting and classifying threats in real-time Logs and Events data for security monitoring SOC.
- Working through the full ML lifecycle on every project: data curation, training, evaluation, ONNX export, and production deployment (FastAPI/Crow + PostgreSQL + AWS EC2)

I work mainly in Google Colab (GPU-accelerated) and deploy to AWS. Interested in roles where I can keep building this kind of end-to-end AI infrastructure.

---

## Tech Stack

<div align="center">

**AI / ML**
<br>
<img src="https://skillicons.dev/icons?i=python,pytorch,opencv,tensorflow,sklearn,keras" />

**Backend**
<br>
<img src="https://skillicons.dev/icons?i=python,fastapi,cpp,postgres,mongodb,docker" />

**Frontend**
<br>
<img src="https://skillicons.dev/icons?i=js,ts,react,tailwind,css,vite" />

**Infra & Tools**
<br>
<img src="https://skillicons.dev/icons?i=aws,git,github,linux" />

</div>

---

## Featured Projects

All of the projects below are complete systems: fine-tuned/trained model, backend API, and (where noted) a frontend dashboard, deployed on a shared AWS EC2 instance.

### [Aegis-Sentinel-Net](https://github.com/BeauBryanDev/AegisSentinel-Net)
Real-time violence and weapon detection for security monitoring. ResNet50 + custom temporal attention MLP for violence classification, running only when a YOLOv11-nano-pose contact trigger fires (IoU ≥ 0.40 between person boxes) — keeping GPU load minimal until a real interaction is detected.
- **F1 (violence classification): 0.935** | Weapon detection mAP@50: 0.680
- Stack: PyTorch, ONNX Runtime, YOLOv11-nano/pose, FastAPI, PostgreSQL, React + Tailwind

### [Aegis-Safe-Work](https://github.com/BeauBryanDev/aegis-safe-work)
Industrial workplace safety monitor combining three independent CV models: browser-side fire/smoke detection (YOLOv8n + ONNX.js), server-side PPE compliance (YOLOv11s, 8 classes), and per-worker fall detection (EfficientNet-Lite0 + temporal attention).
- **Fall detection F1: 0.973** | Recall: 0.989 (deployment threshold tuned to 0.65 to reduce false alarms)
- Stack: PyTorch, EfficientNet-Lite0, YOLOv8/v11, FastAPI, PostgreSQL

### [RiverWatch (Aegis-River-Sentinel)](https://github.com/BeauBryanDev/aegis-river-sentinel)
River anomaly detection and surface flow monitoring from fixed-camera footage. Fine-tuned SegFormer-B2 segments the water surface; RAFT-Small computes optical flow restricted to the water ROI; a sliding-window Z-score flags flash floods and abnormal velocity spikes. Validated on real footage from Andean rivers in Santander, Colombia.
- Multi-dataset segmentation training (RIWA + Parepare Flood, partial-label supervision)
- Stack: PyTorch, SegFormer-B2, RAFT, Celery + Redis, FastAPI, PostgreSQL

### [RockPulseAPI](https://github.com/BeauBryanDev/RockPulseAPI)
B2B computer vision service for mining conveyor belts: detects and measures rock fragments in real time, computing sphericity, volume, and a custom Fragment Index per rock, plus D30/D50/D80 granulometric curves. Built entirely in C++ for high-throughput industrial inference.
- **mAP50 (mask): 0.83** | ArUco-calibrated real-world metrology, per-location API token scoping
- Stack: C++17, Crow, ONNX Runtime, OpenCV, PostgreSQL

### [SmartCrackLens](https://github.com/BeauBryanDev/SmartCrackLens)
End-to-end structural crack detection and severity analysis for concrete, metal, and asphalt surfaces. Fine-tuned YOLOv8n-seg on ~13K images, paired with fractal-dimension analysis (box-counting) for automated severity classification.
- Trained on ~13,000 images, full MLOps pipeline (training → ONNX export → deployment)
- Stack: PyTorch, YOLOv8-seg, FastAPI, MongoDB, React + TypeScript

### [Aegis-Traffic-Sentinel](https://github.com/BeauBryanDev/aegis-traffic-sentinel)
Car crash detection for a smart-city road safety application. MobileNetV2 + temporal attention MLP, trained on ~6,100 videos combining three public crash datasets with crash-centered and biased temporal sampling strategies. Backend inference only for now — frontend is planned next.
- **Test set: F1 0.983 | Recall 1.000** (zero missed crashes on held-out test set)
- Stack: PyTorch, MobileNetV2, ONNX Runtime, FastAPI, PostgreSQL (AWS RDS)

### [SphinxEyes](https://github.com/BeauBryanDev/Sphinx)
Full computer vision + NLP pipeline that reads Middle Egyptian hieroglyphs from raw photographs: YOLOv11-Large glyph detection, geometric reading-order assembly, a Viterbi/bigram language model for sign correction, and GPT-4o for scholarly transliteration.
- **mAP50: 0.884** (V4) across 150 Gardiner sign classes
- Stack: PyTorch, YOLOv11, FastAPI, PostgreSQL, GPT-4o, React + TypeScript

---

## Recent Activity 

<!--RECENT_ACTIVITY:start--> 
1. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/oryza_mind](https://github.com/BeauBryanDev/oryza_mind)<br>
2. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/oryza_mind](https://github.com/BeauBryanDev/oryza_mind)<br>
3. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/oryza_mind](https://github.com/BeauBryanDev/oryza_mind)<br>
4. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/oryza_mind](https://github.com/BeauBryanDev/oryza_mind)<br>
5. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/oryza_mind](https://github.com/BeauBryanDev/oryza_mind)<br>
<!--RECENT_ACTIVITY:end-->
1. ⭐ Starred [gauravsdeshmukh/FlowPy](https://github.com/gauravsdeshmukh/FlowPy)<br>
2. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/Itaca_capstone_project](https://github.com/BeauBryanDev/Itaca_capstone_project)<br>
3. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/Itaca_capstone_project](https://github.com/BeauBryanDev/Itaca_capstone_project)<br>
4. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/aegis_art_atelier](https://github.com/BeauBryanDev/aegis_art_atelier)<br>
5. ⬆️ Pushed undefined commit(s) to [BeauBryanDev/Itaca_capstone_project](https://github.com/BeauBryanDev/Itaca_capstone_project)<br>

## GitHub Stats

<div align="center">
<img height="165" src="https://github-readme-stats-indol-mu-58.vercel.app/api?username=BeauBryanDev&theme=dark&hide_border=false&include_all_commits=true&cache_seconds=86400" />
<img height="165" src="https://github-readme-stats-indol-mu-58.vercel.app/api/top-langs/?username=BeauBryanDev&theme=dark&hide_border=false&include_all_commits=true&layout=compact&cache_seconds=86400" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=BeauBryanDev&theme=dark&hide_border=false" />
</div>

---

<div align="center">

**Let's connect** — [LinkedIn](https://www.linkedin.com/in/beaunix) · [X](https://twitter.com/BeauBryanDev) · [Email](mailto:bryan.beau.186@gmail.com)

</div>
