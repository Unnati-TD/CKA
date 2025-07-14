# Kubernetes YAML Templates for CKA Practice

This folder contains Kubernetes YAML templates aligned with the **Certified Kubernetes Administrator (CKA)** curriculum.

Each file is intended for **manual practice** — download it using `curl`, make changes if needed, and then apply it to your cluster.

---

## How to Use (with `curl` + modify before apply)

You can fetch any template file using `curl`:

```bash
curl -O https://raw.githubusercontent.com/Unnati-TD/CKA/main/YML-Template/<file-name>.yaml
```
## Then open it in your editor (like nano or vim), make modifications, and apply it:

```bash
kubectl apply -f <file-name>.yaml
```

## Example:

```bash
curl -O https://raw.githubusercontent.com/Unnati-TD/CKA/main/YML-Template/4-deployment.yaml
nano 4-deployment.yaml   # Edit the varialbes.
kubectl apply -f 4-deployment.yaml
```
# Available Templates

| File                              | Description               |
| --------------------------------- | ------------------------- |
| `1-pod.yaml`                      | Simple Pod                |
| `2-multi-container-pod.yaml`      | Multi-container Pod       |
| `3-replication-controller.yaml`   | ReplicationController     |
| `4-deployment.yaml`               | Deployment                |
| `5-service-clusterip.yaml`        | ClusterIP Service         |
| `6-service-nodeport.yaml`         | NodePort Service          |
| `7-service-loadbalancer.yaml`     | LoadBalancer Service      |
| `8-configmap.yaml`                | ConfigMap                 |
| `9-secret.yaml`                   | Secret                    |
| `10-persistent-volume.yaml`       | PersistentVolume          |
| `11-persistent-volume-claim.yaml` | PersistentVolumeClaim     |
| `12-pod-with-pvc.yaml`            | Pod using PVC             |
| `13-hpa.yaml`                     | Horizontal Pod Autoscaler |
| `14-taint-toleration.yaml`        | Taint & Toleration        |
| `15-node-selector.yaml`           | Node Selector             |
| `16-affinity.yaml`                | Affinity Rules            |
| `17-namespace.yaml`               | Namespace                 |
| `18-role.yaml`                    | Role                      |
| `19-rolebinding.yaml`             | RoleBinding               |
| `20-resourcequota.yaml`           | ResourceQuota             |
| `21-limitrange.yaml`              | LimitRange                |

`Note: These templates are intentionally minimal. Feel free to add labels, annotations, limits, and probes as per your learning goals.`

Happy Learning & Good Luck with CKA! ☸️

Made with ❤️ by `Team Unnati`

