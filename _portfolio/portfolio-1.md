---
title: "Cloud-Based Face Recognition System"
excerpt: "Built a scalable, cloud-based face recognition system on AWS with autoscaling and efficient real-time image processing.<br/>"
collection: portfolio
---

I built a cloud-based face recognition system designed to handle image processing at scale using AWS services. The system follows a distributed, message-driven architecture with components like EC2, SQS, Lambda, and S3 working together to process images asynchronously. I developed the application tier on EC2 and implemented an autoscaling controller that adjusts the number of instances based on queue load, ensuring the system can handle varying traffic efficiently without over-provisioning resources.

To improve scalability and reliability, I containerized key components using Docker and designed the system with loosely coupled services, making it more fault-tolerant and easier to maintain. The pipeline performs face detection and embedding generation in a scalable way, supporting real-time inference workloads. I also focused on optimizing latency and throughput, which helped the system respond quickly even under heavy load. This project gave me strong hands-on experience with cloud architecture, distributed systems, and building production-ready, scalable applications.
