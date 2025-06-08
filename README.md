🚢 From Docker Build to Node Drain – A Hands-On Kubernetes Journey ⚙️🐳

I took a deep dive into the gritty side of Kubernetes—not on the cloud, not on some fancy managed platform, but entirely local using KIND (Kubernetes IN Docker). Why? Because mastering orchestration should be about understanding the engine before driving the car.

🔧 Here’s what I built:
➡️ A Flask web app from scratch
➡️ Containerized it using Docker
➡️ Pushed it to Docker Hub
➡️ Deployed on a multi-node Kubernetes cluster (yes, even load-balanced across nodes!)
➡️ Simulated a production-style node drain with 0 downtime
➡️ Rolled back the node, rescheduled pods, scaled, restarted, and validated it like a real-world SRE would.

💡 The twist? No cloud provider, no billing meter running. Just raw YAMLs, Docker containers as nodes, and clean command-line automation.

📂 Project Highlights:

- Custom kind-2node-cluster.yaml
- Hands-on with kubectl drain, cordon, rollout restart, and NodePort service exposure
- Built alias shortcuts to move faster in kubectl operations
- Simulated production scenarios like node maintenance and balanced rescheduling

This wasn’t just about “getting it to work” — it was about thinking like an SRE, designing for resilience, and breaking things safely to understand how they heal.

🎯 Tools used: Docker, Kubernetes, KIND, Flask
📄 Infra destroyed cleanly at the end
