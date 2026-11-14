# Kubernetes practice inventory / Lisitry ny exercices

This inventory records resources and outcomes reported by the learner. It is not a live query of the Minikube cluster. Resource existence and YAML contents have not been independently verified in this repository.

| Kind | Reported name | Exercise / note |
|---|---|---|
| Deployment | `config-demo` | ConfigMap exercise |
| Deployment | `nginx` | NGINX workload |
| Deployment | `secret-demo` | Secret exercise |
| Deployment | `secret-volume-demo` | Secret mounted as volume |
| Service | `config-service` | ConfigMap-related service |
| Service | `nginx` | NGINX service |
| Service | `nginx-lb` | LoadBalancer exercise |
| Ingress | `nginx-ingress` | NGINX Ingress; host `school.local` |
| PVC | `school-pvc` | Persistent storage claim |
| Pod | `storage-test` | Storage persistence test |
| Pod | `ingress-test` | Ingress connectivity test |
| StorageClass | `standard` | Dynamic provisioning |
| Controller | NGINX Ingress Controller | Installed for ingress exercise |
| ConfigMap | Name not recorded here | Environment-variable exercise |
| Secret | Name not recorded here | Pod volume exercise |

## Reported test outcomes / Vokatra notaterina
- Ingress test: browser displayed the NGINX welcome page after configuring the `school.local` host and using port-forwarding.
- Storage test: the text `Hello Kubernetes Storage` was written/read under `/data`; it reportedly remained after deleting and recreating the Pod.

## Evidence still to add / Porofo mbola ampidirina
- Original YAML manifests (for example `storage-test.yaml` and `school-pvc.yaml`).
- Exact commands and sanitized outputs.
- Kubernetes version, Minikube version and relevant configuration.
- Screenshots or logs where useful.

Do not invent manifests from resource names. Add the exact files that were tested, and remove sensitive values before committing.
