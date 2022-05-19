= BK NOTES

In multi-tenancy-gitops-apps/apic/environments/single-cluster/config/secrets/:
- Renamed generated file:
  ibm-entitlement-key-secret.yaml --> ibm-entitled-registry-credentials-secret.yaml 

Had an error when APIC was being instantiated: "issuers.cert-manager.io already exist".
- Deleting the APIC operator instance fixed it, ArgoCD instantiated it again.

ArgoCD certificate creation task may get blocked. Try deleting.