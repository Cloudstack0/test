# test

test3

## Architecture & Deployment

This service was scaffolded using the **Cloudstack0 Golden Path** on Red Hat Developer Hub.

- **Port**: `80`
- **Base Image**: `nginx:alpine`
- **Container Image**: `ghcr.io/cloudstack0/test:latest`
- **CI/CD Pipeline**: `Enabled (Tekton)`
- **GitOps Management**: Managed via Argo CD in [Cloudstack0/devops](https://github.com/Cloudstack0/devops) under `platform/config/instances/proxmox/central/test`.
- **Internal Domain**: `https://test.central.internal.beftraelec.ma`

## Local Development

```bash
docker build -t test:latest .
docker run -p 80:80 test:latest
```
