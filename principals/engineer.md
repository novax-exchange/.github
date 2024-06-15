# Meta principal for Engineering team
- API first strategy. It also applies for data.
- If you need it, you build it. While others are happy to help, they ensure it can be rebuilt.
- In non-office hours, we enjoy hackathon and open source community
- Deterministic applies a lot
## Principal for Data team
- No excel swamp
- data pipeline should be reproducible
- 

## Principal for App team
- ConnectionLess and serverless are preferred
- Idempotent API. Make them like blockchain oracle
- Avoid VM
  - VM as bastion: for operation purpose only, as another desktop, as a control plane for thick client 
  - VM as k8s Node: -> serverless k8s,  -> container as service (aws Fargate, Azure Function, GCP Cloud Run)
  - VM as static web site hosting -> S3
- BM for Trading core

