kubectl port-forward -n argocd svc/argocd-server 8080:443

kubectl -n argocd get secret argocd-initial-admin-secret -o yaml

echo password | base64 --decode

kubectl apply -f application.yaml