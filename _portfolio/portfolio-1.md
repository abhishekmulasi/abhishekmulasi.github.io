---
title: "AWS Distributed Face Recognition Pipeline"
excerpt: "Scalable, cloud-native face recognition system on AWS achieving ~30% latency reduction through parallel processing, autoscaling, and queue-based decoupling.<br/>"
collection: portfolio
---

I designed and built a production-grade, distributed face recognition pipeline on AWS, combining a message-driven architecture with intelligent autoscaling to handle real-time inference workloads at scale. The system orchestrates EC2, SQS, Lambda, and S3 to process images asynchronously: incoming requests are enqueued in SQS, consumed by EC2 application-tier workers, and results are persisted in S3 with post-processing triggered via Lambda.

A core contribution was the autoscaling controller I implemented, which dynamically provisions EC2 instances (0–15) based on live queue depth metrics. This eliminated over-provisioning during low-traffic windows while ensuring the system could absorb traffic spikes without degradation. By parallelizing the processing pipeline and leveraging queue-based decoupling to remove inter-component dependencies, I reduced end-to-end latency by approximately 30%.

The ML pipeline performs face detection and embedding generation in a distributed, fault-tolerant manner, with Docker containerization ensuring environment consistency across all worker instances and simplifying horizontal scaling. The loosely coupled service design improved both fault isolation and maintainability. This project gave me deep hands-on experience with cloud-native architecture, distributed systems engineering, and optimizing ML inference pipelines for production workloads.
