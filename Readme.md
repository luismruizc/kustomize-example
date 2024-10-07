### First commit


argocd app create votapp \
--repo https://github.com/luismruizc/kustomize-example \
--path overlays/dev \
--dest-namespace votapp \
--dest-server https://kubernetes.default.svc \
--self-heal \
--sync-policy automated \
--sync-retry-limit 2 \
--revision main