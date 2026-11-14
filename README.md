# Linux Practice — Cloud, DevOps & Cybersecurity

**EN | English**  
A hands-on learning portfolio documenting practical work with Linux/Ubuntu on WSL2, Git/GitHub, Docker and Kubernetes. The repository separates exercises already reported as completed from topics still on the learning roadmap.

**MG | Malagasy**  
Portfolio fianarana sy fanazaran-tena momba ny Linux/Ubuntu amin'ny WSL2, Git/GitHub, Docker ary Kubernetes. Avahana eto ny exercices efa notaterina fa vita sy ireo mbola ao anatin'ny roadmap.

> **Status note / Fanamarihana:** Completed items below are based on the learner's reported practice. The original local files, cluster state and test evidence have not all been independently verified or committed yet. Do not interpret these exercises as production-level experience.

## Learning progress / Fandrosoana

| Area / Sehatra | Current status / Sata |
|---|---|
| Linux & Ubuntu WSL2 | Fundamentals practiced / Fototra nampiharina |
| Git & GitHub | Basic commands practiced; workflow to strengthen / Commandes fototra; hamafisina |
| Docker | Docker Desktop, Engine, WSL integration and contexts practiced / Nampiharina |
| Kubernetes fundamentals | Pods, Deployments, ConfigMaps, Secrets, Services, Ingress and storage exercises reported complete / Exercices voalaza fa vita |
| Advanced Kubernetes | Planned / Mbola kasaina |
| CI/CD, Terraform, monitoring, cloud | Planned / Mbola kasaina |

## Repository map / Firafitry ny repository

- `linux/` — Ubuntu/WSL2 notes, commands, files and permissions.
- `git/` — Git workflow and command reference.
- `docker/` — Docker learning notes and future hands-on examples.
- `kubernetes/` — notes grouped by Kubernetes topic; see the evidence and manifest status before assuming a YAML file is included.
- `cicd/` — GitHub Actions learning area (planned).
- `terraform/` — Infrastructure as Code learning area (planned).
- `monitoring/` — Prometheus, Grafana, logging and alerting (planned).
- `cloud/` — cloud fundamentals and deployment notes (planned).
- `app/` — existing shell practice files.

## Reported practical work / Asa efa notaterina

### Linux & Docker
- Ubuntu on WSL2; Linux terminal commands; Nano for YAML editing.
- Docker Desktop, Docker Engine, WSL integration and Docker contexts.
- Docker and Minikube environment relationship explored.

### Kubernetes
- Pods and Deployments; `kubectl get`, `apply`, `describe`, `exec`, `delete`.
- ConfigMaps and environment variables; Secrets and mounting a Secret as a volume.
- ClusterIP, NodePort and LoadBalancer Services; Minikube tunnel and Pod connectivity tests.
- NGINX Ingress Controller, an Ingress named `nginx-ingress`, host `school.local`, port-forwarding and browser test showing the NGINX welcome page.
- PersistentVolume (PV), PersistentVolumeClaim (PVC), StorageClass `standard`, dynamic provisioning and persistence test using `/data`. Reported test: data `Hello Kubernetes Storage` remained after replacing the Pod.

See [Kubernetes practice inventory](kubernetes/INVENTORY.md) for resource names and evidence limitations.

## Roadmap / Tohin'ny fianarana

1. Strengthen Linux, Git/GitHub and Docker: permissions, branching, pull requests, Dockerfiles, Compose, networks, volumes and image management.
2. Continue Kubernetes: Namespaces, StatefulSets, Helm, RBAC, Jobs/CronJobs, resource requests/limits and troubleshooting.
3. Build CI/CD with GitHub Actions: automated tests, image build and deployment.
4. Learn Terraform and Infrastructure as Code.
5. Add monitoring and logging with Prometheus, Grafana and alerts.
6. Learn cloud fundamentals and deployment. No AWS account is required for the first learning steps.

Detailed checklist: [roadmap.md](roadmap.md).

## How to use this repository / Fomba fampiasana
1. Read the topic notes.
2. Recreate exercises in a local learning environment.
3. Save the exact commands, YAML manifests and test outputs used.
4. Add screenshots or sanitized logs where useful; never commit credentials, tokens or real Secret values.
5. Update each topic's status only when the exercise has been repeated and evidence is recorded.

## Safety and evidence
- Kubernetes Secret examples must use dummy values only. Do not commit real credentials or decoded Secret data.
- Cluster resource names in the inventory are learner-reported; they are not proof that those resources still exist.
- No production deployment, CI/CD pipeline, Terraform infrastructure or monitoring stack is claimed as completed.

---
**Goal / Tanjona:** Build practical foundations toward a Cloud DevOps and Cybersecurity engineering role, while documenting progress honestly.
