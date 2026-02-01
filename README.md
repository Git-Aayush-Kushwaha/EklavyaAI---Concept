# EklavyaAI---Concept
Ekalavya AI is a Generative AI-powered "Super Tutor" designed specifically for rural students in India who cannot afford expensive coaching for competitive exams like IIT-JEE, NEET, and CAT.

**Quality education should not be a luxury.**
In India, millions of talented students in rural areas fail to crack competitive exams (JEE/NEET/CAT) due to two barriers: **Language** and **Cost**.

**BharatShiksha AI** is an open-source initiative to build a "Super Tutor" that lives in a ₹5,000 smartphone. It uses Generative AI to teach complex concepts in local dialects (Bhojpuri, Tamil, Marathi, etc.) and works seamlessly on 2G/3G networks.

---

## ✨ Key Features

- **🗣️ Vernacular Voice-First Interface**
  - Students speak in their mother tongue; the AI replies in the same language.
  - Powered by **AWS Transcribe** (ASR) and **AWS Polly** (TTS).
  
- **🧠 Socratic AI Tutor**
  - Unlike chatbots that just give answers, this agent asks follow-up questions to build logic.
  - Powered by **Amazon Bedrock (Claude 3 Sonnet)**.

- **📷 Visual Doubt Solving (OCR)**
  - Support for handwritten notes and textbook images.
  - Powered by **Amazon Textract**.

- **📉 Low-Bandwidth Mode (Edge AI)**
  - Optimized for rural internet (2G/3G).
  - Uses compression and local caching for offline study.

- **📚 Syllabus-Grounded RAG**
  - Strictly follows NCERT/IIT-JEE curriculum using Retrieval Augmented Generation (RAG).

---

## 🏗️ Tech Stack

| Domain | Technology |
| :--- | :--- |
| **Cloud Provider** | AWS (Amazon Web Services) |
| **LLM Orchestration** | LangChain / Amazon Bedrock |
| **Backend** | Python (FastAPI) + AWS Lambda (Serverless) |
| **Frontend** | Flutter (Android/iOS) |
| **Vector DB** | Amazon Kendra / ChromaDB |
| **Voice Stack** | Amazon Transcribe (STT) + Amazon Polly (TTS) |

---

## 🚀 Getting Started

We welcome contributors! Follow these steps to set up the project locally.

### Prerequisites
* Node.js & NPM
* Python 3.9+
* Flutter SDK
* AWS Account (for API keys)

### Installation

1.  **Clone the Repository**
    ```bash
    https://github.com/Git-Aayush-Kushwaha/EklavyaAI---Concept.git
    ```

2.  **Backend Setup**
    ```bash
    cd backend
    pip install -r requirements.txt
    ```

3.  **Environment Variables**
    Create a `.env` file in the `backend` folder:
    ```env
    AWS_ACCESS_KEY_ID=your_access_key
    AWS_SECRET_ACCESS_KEY=your_secret_key
    AWS_REGION=ap-south-1
    BEDROCK_MODEL_ID=anthropic.claude-3-sonnet-20240229-v1:0
    ```

4.  **Run the Server**
    ```bash
    uvicorn main:app --reload
    ```

5.  **Frontend Setup**
    ```bash
    cd ../frontend
    flutter pub get
    flutter run
    ```

---

## 🤝 How to Contribute

We love pull requests! If you want to help democratize education, here's how:

1.  **Fork** the repo on GitHub.
2.  **Clone** the project to your own machine.
3.  **Create a branch** for your feature (`git checkout -b feature/AmazingFeature`).
4.  **Commit** changes to your own branch.
5.  **Push** your work back up to your fork.
6.  **Submit a Pull Request** so that we can review your changes.

### 🌱 Good First Issues
Check out the [Issues tab](https://github.com/your-username/bharat-shiksha-ai/issues) for tasks labeled `good first issue`. These are great for newcomers!

---

## 🗺️ Roadmap

- [ ] **Phase 1:** Core Voice AI Prototype (Hindi & English).
- [ ] **Phase 2:** Integration of Vision (OCR) for solving math problems.
- [ ] **Phase 3:** Offline synchronization module for no-internet zones.
- [ ] **Phase 4:** Community peer-to-peer learning features.

---

## 🛡️ License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙏 Acknowledgments

* **AWS** for the infrastructure and AI tools.
* **NCERT** for the open curriculum framework.
* All the open-source contributors helping build Bharat's future.

---
<p align="center">
  Made with ❤️ for 🇮🇳 Bharat
</p>
