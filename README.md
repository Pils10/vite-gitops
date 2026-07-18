# vite-gitops

Desired Kubernetes state for two Argo CD Applications:

- `apps/vite-demo/overlays/dev`
- `apps/vite-demo/overlays/production`

Jenkins edits the relevant `newTag` field. Argo CD notices that Git commit and
reconciles the cluster.
