# argocd
argocd configuration
By default, Argo CD periodically checks the Git repository for changes. The default reconciliation interval is typically up to about 3 minutes.

You can configure it in Argo CD's argocd-cm ConfigMap: kubectl get cm argocd-cm -n argocd
we will chnage under :
    data:
        timeout.reconciliation: 180s