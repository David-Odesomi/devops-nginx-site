Devops-Nginx-Site

devops-nginx-site/
├── site/
│ ├── index.html ← your static site
│ └── style.css
├── nginx/
│ └── nginx.conf ← custom Nginx config
├── Dockerfile ← packages site + nginx into an image
├── k8s/
│ ├── deployment.yaml ← tells K8s how to run your container
│ └── service.yaml ← exposes it so you can access it
└── .github/
└── workflows/
└── ci.yml ← builds & pushes image on every push to main

This is a simple project that implements a CI/CD pipeline using GitHub Actions and Kubernetes.
