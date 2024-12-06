
#  Cosmocloud Kubernetes Deployment Challenge


### Project Overview
Deployed a full-stack application using Kubernetes and Helm on Google Cloud Platform (GKE), featuring:
- Backend Service
- Frontend Service
- Redis Database

### Tech Stack
- Kubernetes
- Helm
- Google Cloud Platform
- Docker Images

### Key Learning Moments

#### Kubernetes Fundamentals
- Understood Pods as smallest deployable units
- Learned about Deployments for scalability
- Explored Service types (ClusterIP, NodePort)
- Configured environment variables using ConfigMaps

#### Helm Chart Magic
- Created modular, reusable deployment configurations
- Used templating with `values.yaml`
- Simplified complex Kubernetes deployments

### Challenges

#### Helm Linting
**Problem:** Helm lint recommended adding an icon


#### GCP Quota Limitations
**Problem:** Insufficient storage quota
**Solution:** 
- Reduced cluster node count
- Adjusted machine type

### Deployment Steps
```bash
# Initialize GKE Cluster
gcloud container clusters create cosmocloud-cluster

# Deploy Helm Chart
helm install testapp . --atomic --timeout 30s
```

### 🖼 Screenshots
![alt text](<Screenshot 2024-12-06 201802.png>) ![alt text](<Screenshot 2024-12-06 202035.png>) ![alt text](<Screenshot 2024-12-06 201802-2.png>)
