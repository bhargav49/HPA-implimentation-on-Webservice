🚀 Project: HPA Implementation on Apache Service
✅ Pre-requisite
Install the Metrics Server to enable resource metrics collection:


🧩 Apache Service Setup
You have a Kubernetes service named apache-service in the apache namespace, which is targeted by HPA.

🔄 Load Testing with BusyBox
To simulate load on the Apache service:

Run a BusyBox pod interactively:


Inside the BusyBox shell, run an infinite loop to generate traffic:


📈 HPA Behavior
This loop continuously sends requests to the Apache service, increasing CPU usage on the pods. The HPA monitors this usage and scales the number of pods accordingly based on the defined thresholds.

Would you like help writing the HPA YAML file or visualizing the scaling behavior over time?




