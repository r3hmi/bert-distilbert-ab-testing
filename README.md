# A/B Testing BERT vs DistilBERT for Question Answering on SQuAD v1.1

## 1. 📘 Technical Framing & Motivation

This project implements a **head-to-head A/B testing framework** to evaluate the performance trade-offs between **BERT** and **DistilBERT** on the **Stanford Question Answering Dataset (SQuAD v1.1)**. BERT has set the benchmark for extractive QA tasks due to its deep transformer-based architecture, while DistilBERT offers a compressed alternative with significantly reduced inference time and memory footprint.

The central question driving this project is:  
> _How does DistilBERT perform relative to BERT in terms of accuracy, latency, and efficiency under identical evaluation conditions in a real-world QA scenario?_

Through a systematic A/B testing pipeline, this project supports practitioners and researchers in understanding the performance-cost trade-offs involved in deploying full-size vs. distilled models in production-level Question Answering systems.

---

## 2. ⚙️ Tech Stack & Architecture

### **Languages & Frameworks**
- **Python 3.10+**
- **PyTorch** with **Hugging Face Transformers**
- **Hugging Face Datasets & Evaluate**
- **FastAPI** and/or **Streamlit** for deployment
- **Docker** for containerization

### **Architecture Overview**

![Model Architecture Diagram](./assets/architecture.png "Model Architecture Diagram")


---

## 3. 🚀 Key Capabilities

- **Pre-trained QA Pipeline** using `bert-base-uncased` and `distilbert-base-uncased`
- **A/B Testing Engine** with randomized or parallel model evaluation
- **Performance Metrics Logging**:  
  - Accuracy: F1 Score, Exact Match (EM)  
  - Efficiency: Inference Time, Memory Usage  
- **Statistical Significance Testing**: McNemar's Test, Paired t-tests
- **Visual Dashboards**: Latency histograms, Accuracy comparison plots
- **Interactive Interface** via Streamlit or REST API via FastAPI
- **Container-Ready Deployment** using Docker

---

## 4. 💼 Example Use Cases

- **Benchmarking Efficiency**: Compare model performance under identical QA tasks to choose the best model for production deployment.
- **Latency-Constrained Applications**: Test feasibility of deploying DistilBERT in mobile or edge environments.
- **Educational Demos**: Demonstrate the concepts of model compression, knowledge distillation, and A/B testing in a QA context.
- **Research Evaluation**: Provide reproducible evidence for trade-offs between large and compact models using SQuAD.

---

## 5. 🛣️ Roadmap

| Milestone                                    | Status      |
|---------------------------------------------|-------------|
| ✅ Data Preprocessing & QA Pipelines         | Complete    |
| ✅ A/B Testing Framework                     | Complete    |
| ✅ Evaluation Metrics & Logging              | Complete    |
| ✅ Offline Static Evaluation                 | Complete    |
| ⬜ Streamlit Demo UI                         | In Progress |
| ⬜ FastAPI Service with Model Routing        | Planned     |
| ⬜ Integration with Triton Server or MLFlow  | Planned     |
| ⬜ Support for SQuAD v2.0 and multilingual datasets | Planned     |

---

## 6. 📄 License

This project is licensed under the **MIT License**.  
See the [LICENSE](./LICENSE) file for details.




