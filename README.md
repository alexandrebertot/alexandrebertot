# Hi, I'm Alexandre 👋

## 🚀 About Me
Final-year Computer Science student at École Centrale de Lyon, seeking a 6-month
end-of-studies internship from **March 2027** in Data Science, Machine Learning or AI.
I've built forecasting models in production (airline baggage at Wiremind), a multimodal
deep learning model in research (medical imaging), and I'm currently building an LLM
agent end-to-end.

## 💼 Experience

**ML Engineer Intern - Wiremind (Cargo Team)**
*Paris, France · Mar 2026 – Aug 2026*
- Built and deployed LightGBM-based baggage weight and volume forecasting models for a new
  client, from data cleaning to deployment.
- Removed the dependency on an external passenger forecast provider using only the
  client's own history: 95% of volume forecasts within ±1 container (the team's
  best-performing model) and an MdAPE of 22% on weight.
- Led R&D on automated model monitoring, training secondary models on
  prediction residuals to detect anomalies and performance drift, using SHAP
  to interpret which features drove the largest errors.
- Monitored production baggage weight and volume forecasting models for Etihad
  & WestJet, using datasets of up to ~1M forecast rows/month for Etihad;
  identified error causes and proposed fixes.

**Computer Vision Research Intern - Center for Visual Computing, CentraleSupélec - Université Paris-Saclay**
*Paris-Saclay, France · Sep 2025 – Feb 2026*
- Developed a multimodal deep learning model to predict survival time for liver
  cancer patients from histopathology slides and CT scans, in collaboration
  with hospitals in Île-de-France.
- Since whole slides are too large for a neural network, split them into patches
  encoded with pretrained models, and used attention-based Multiple Instance Learning (MIL)
  to learn which tissue regions are most informative.
- Combined the two sources by averaging their predictions rather than merging their
  features, an approach suited to the small cohort of 70 patients: mean absolute
  error (MAE) of 2.5 months on patients with survival ≤ 12 months.

## 🛠 Selected Projects

**[Football AI Agent — LLM & Match Prediction](https://github.com/alexandrebertot/football-match-analyst)** · 🚧 *In progress*
LLM agent that answers questions about the top 5 European leagues and the Champions League
by calling tools: current fixtures, results and standings from the football-data.org API and a LightGBM match outcome predictor.
Tool-calling loop written from scratch, local Qwen 3.5 9B LLM served locally with Ollama, a local chat
interface, FastAPI, Docker, CI with GitHub Actions. The predictor, tracked and registered with
MLflow, closes 44% of the log-loss gap between a naive baseline and bookmakers' odds on
held-out seasons.
*Next: an LLM evaluation set, then QLoRA fine-tuning of a small model.*

**[ASL Alphabet Recognition](https://github.com/alexandrebertot/asl-recognition)**
Built a real-time American Sign Language alphabet recognition system (MediaPipe
landmarks + MLP classifier, live webcam demo), trained on 24,000 images with a
signer-disjoint split, achieving a macro F1 of 0.856 on unseen signers.

## 🧰 Technical Skills

<p align="center"><b>Languages</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge" />
</p>

<p align="center"><b>AI &amp; Data Science</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/LightGBM-2E8B57?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SHAP-8A2BE2?style=for-the-badge" />
</p>

<p align="center"><b>Tools</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white" />
</p>
