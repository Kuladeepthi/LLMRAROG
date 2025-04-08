- TEAM MEMBERS
- HARITEJA - 23BDS019
- VINAY - 23BDS068
- TEJASWI - 23BDS064
- HARIPRASAD - 23BDS022
- MANOJ - 23BDS056
- KULA DEEPTHI - 23BDS013

------------------------------------------
#  AI Research Assistants

This repository contains the code and resources for the project that evaluates AI research assistants leveraging large language models (LLMs). The project compares Retrieval-Augmented Generation (RAG)-enhanced systems with pure LLM approaches across several key performance metrics, such as information retrieval accuracy, response speed, and computational resource usage.

---

## Table of Contents

- [Overview](#overview)
- [Project Objectives](#project-objectives)
- [Research Significance](#research-significance)
- [System Implementation](#system-implementation)
- [Installation](#installation)
- [Usage](#usage)
- [Experiments and Evaluation](#experiments-and-evaluation)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [References](#references)

---

## Overview

This project presents a comprehensive performance analysis of AI research assistants. It focuses on benchmarking and comparing two major architectures:
- **RAG-enhanced Systems:** Combine information retrieval with LLM-generated responses to improve factual accuracy.
- **Pure LLM Approaches:** Leverage the internal parametric knowledge of pre-trained models, providing faster but potentially less grounded responses.

Experiments were conducted across multiple platforms and query types, addressing issues like retrieval precision, latency, resource consumption, and ethical considerations such as potential biases and citation fairness.

---

## Project Objectives

- **Benchmarking:** Develop a robust framework to evaluate AI research assistants using standardized metrics.
- **Performance Comparison:** Provide a head-to-head analysis of RAG-enhanced vs. pure LLM systems.
- **System Evaluation:** Measure the impact of varying query complexities and domain-specific requirements on system performance.
- **Guidance for Researchers:** Assist developers and academics in selecting the most appropriate AI tools based on empirical evidence and performance trade-offs.

---

## Research Significance

The integration of LLMs into research workflows is transforming literature reviews, hypothesis formulation, and data analysis. However, selecting the right tool requires understanding its strengths and limitations. This project addresses that gap by offering:
- Empirical insights into the trade-offs between accuracy and speed.
- A detailed look at resource requirements and cost implications.
- Recommendations for future enhancements in AI research assistant technologies.

---

## System Implementation

The repository includes:
- **Frontend:** Built with React.js to display and interact with research queries and visualized results.
- **Backend:** Implemented with FastAPI to handle API calls, model integrations, and retrieval operations.
- **Storage:** Utilizes a vector database for embeddings and PostgreSQL for metadata management.
- **Benchmarking Tools:** Scripts for running experiments based on TREC, BEIR, SciDocs, and SCIFACT datasets.

---

## Installation

### Prerequisites
- Python 3.8 or higher
- Node.js and npm (for frontend)
- PostgreSQL database
- Docker (optional, for containerization)

### Backend Setup

1. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure your PostgreSQL database and update the connection settings in the configuration file.

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. Start the frontend server:
   ```bash
   npm start
   ```

---

## Usage

1. **Start the Backend Server:**
   ```bash
   uvicorn main:app --reload
   ```

2. **Access the Frontend:**
   Open your browser and navigate to `http://localhost:3000` to interact with the application.

3. **Submit Research Queries:**
   Enter academic queries into the system, and the backend will process them using both RAG-enhanced and pure LLM methods. The system will then display comparative results including response time, accuracy, and resource usage.

---

## Experiments and Evaluation

- **Evaluation Metrics:**  
  - Retrieval Precision & Recall
  - Response Accuracy
  - Latency
  - Resource Consumption (RAM, CPU, GPU utilization)
  - Cost Analysis

- **Experiment Setup:**  
  Experiments were conducted on multiple platforms such as high-performance servers and cloud VMs (e.g., AWS EC2). Detailed scripts and configurations are provided under the `experiments` directory.

- **Benchmark Datasets:**  
  Integration with TREC, BEIR, and SciDocs benchmarks to ensure standard and comparable evaluation.

---

## Results

The evaluation results include:
- **Performance Comparison:** Graphs and tables comparing the effectiveness of different systems on key metrics.
- **Ethical Considerations:** Analysis of bias, citation fairness, and system limitations.
- **Visual Aids:** Diagrams such as activity and state diagrams illustrating the system workflow.

For detailed results, refer to the figures and analysis sections within the report.

---

## Future Work

- Expanding experiments to more specialized research domains.
- Incorporating multimodal data capabilities for enhanced visualization.
- Improving retrieval efficiency through hierarchical indexing and smarter query routing.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your suggestions or improvements. For major changes, please open an issue first to discuss your ideas.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

Special thanks to Prof. Animesh Chaturvedi for his invaluable guidance throughout this project. We also appreciate the support from the open-source community in developing and testing these tools.

---

## References

1. Vaswani, A., et al. "Attention Is All You Need." NeurIPS, 2017.
2. Bender, E. M., et al. "On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?" FAccT, 2021.
3. Devlin, J., et al. "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding." NAACL, 2019.
4. OpenAI. "GPT-4 Technical Report," 2023.
5. Lewis, P., et al. "Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks." NeurIPS, 2020.

---

This README provides an overview of the project, guiding both users and potential contributors through setup, usage, and detailed experiment methodologies. Enjoy exploring and contributing to the project!
