**Helm Install Command – Kube-Prometheus-Stack

Command:
''
helm install [RELEASE_NAME] oci://ghcr.io/prometheus-community/charts/kube-prometheus-stack
''

Use:
This command is used to install the Kube-Prometheus-Stack in a Kubernetes cluster using Helm.

Benefits:
1. Installs Prometheus to collect Kubernetes metrics.
2. Installs Grafana to visualize metrics using dashboards.
3. Installs Alertmanager to manage monitoring alerts.
4. Installs Node Exporter to monitor Linux server CPU, memory, and other resources.
5. Helps monitor the health and performance of an EKS/Kubernetes cluster.
6. Saves time because multiple monitoring tools are installed together using one Helm chart.
Example:
helm install monitoring oci://ghcr.io/prometheus-community/charts/kube-prometheus-stack


Here, monitoring is the release name.

In simple words: This command installs a complete monitoring stack in Kubernetes so we can monitor our cluster, nodes, and applications from Grafana dashboards using Prometheus metrics.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  commands:
  ''
  kubectl port-forward svc/grafana-prom-stack 9090:80 -n namespace --address 0.0.0.0
  ''
    

