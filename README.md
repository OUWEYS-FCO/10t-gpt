# 10T GPT
Final project for the Building AI course

## Summary
10T GPT is a high-performance generative AI specialized in analyzing massive technical datasets. It is designed to process up to 10TB of industrial logs, technical documentation, and real-time sensor data to provide instant diagnostic solutions and predictive maintenance insights for large-scale infrastructure.

## Background
* Data silos in large industries make it impossible for humans to find specific technical errors quickly.
* General LLMs cannot handle the specific context of proprietary industrial data.
* Personal motivation: To create a "Big Data" specialist that doesn't just chat, but solves complex engineering bottlenecks.
* Importance: Minimizing downtime in factories and infrastructure saves millions in operational costs.

## How is it used?
The system is integrated into a company's private cloud. Engineers query 10T GPT via a secure terminal or API. For example: "Analyze the last 48h of pressure logs from Sector 7 and compare them with the 2024 maintenance manual." The AI then points out the exact discrepancy.

## Data sources and AI methods
* Data: Industrial IoT logs, PDF technical manuals, historical repair databases, and CAD specifications.
* Methods: 
    * Vector Databases (Milvus/Pinecone) for efficient data retrieval.
    * RAG (Retrieval-Augmented Generation) to ground the GPT model in factual, private data.
    * Fine-tuning on domain-specific technical language.

## Challenges
* Processing Power: Requires significant GPU resources to handle "10T" scale data.
* Data Accuracy: The model must be strictly audited to avoid "hallucinations" in critical safety procedures.
* Security: Handling sensitive industrial secrets requires air-gapped or highly secure cloud environments.

## What next?
Moving from "Reactive" to "Proactive": Developing a module where 10T GPT automatically flags anomalies before an engineer even asks, effectively becoming an autonomous industrial supervisor.

## Acknowledgments
* Inspired by the Building AI course by Reaktor and the University of Helsinki.
* Built using open-source frameworks like LangChain and Hugging Face.
