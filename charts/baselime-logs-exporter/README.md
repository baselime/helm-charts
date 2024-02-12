# Baselime Logs exporter Helm Chart

Adds DaemonSet, ServiceAccount and ConfigMap, and exports all the pod logs
automatically to Baselime console.

### Usage

Create `custom-values.yaml` file:
```yaml # :icon-code: custom-values.yaml
apiKey: "YOUR_API_KEY" # Obtain the key from Baselime console
```

```bash
helm repo add baselime-logs-exporter https://github.com/baselime/helm-charts
helm repo update
helm install baselime-logs-exporter baselime-logs-exporter/baselime-logs-exporter-logs-exporter --values custom-values.yaml
```