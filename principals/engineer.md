# Principals for Engineering team
- API first strategy. It also applies for data.
  - ConnectionLess data service is an example of data API
- If you need it, you build it. While others are happy to help, they ensure it can be rebuilt.
- In non-office hours, we enjoy hackathon and open source community
- Deterministic applies a lot
- Adopts evolutional architecture
- Keep stateless and sessionless. Only persistent data is exempted to be stateful.
- 
## Principal for Data team
- Deterministic: data pipeline should be reproducible


## Principal for App team
- ConnectionLess Data Service is preferred
- Serverless/BEaaS are preferred
- Build API idempotent. Make them like blockchain oracle
- Avoid VM
  - VM as bastion: for operation purpose only, as another desktop, as a control plane for thick client 
  - VM as k8s Node: -> serverless k8s,  -> container as service (aws Fargate, Azure Function, GCP Cloud Run)
  - VM as static web site hosting -> S3
- BM for Trading core only
- Versionless： use latest
- `.gitignore` defined for the right-scope
   - Reuse Novax global `.gitignore`
   - `.gitignore` in project folder only exclude folder scope, even it is in root folder
