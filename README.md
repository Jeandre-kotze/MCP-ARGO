GitOps repo for Argo CD

Replace the `repoURL` and `path` in `apps/my-app.yaml` with your application repository and manifest path, then push this repo to GitHub and add it as a repository in Argo CD.

Quick steps:

1. Update `apps/my-app.yaml` with your repo URL and path.
2. Push this repo to GitHub.
3. In Argo CD, either add this repo via the UI (Settings → Repositories) or apply the Application manifest directly:

```bash
kubectl apply -f apps/my-app.yaml
```

Then open Argo CD UI at http://localhost:8080 and sync the application.
