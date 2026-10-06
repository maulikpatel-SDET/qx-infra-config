# qx-infra-config  (Repo 4 of 4)

Deployment configuration. Holds algorithm names and key paths used by the other repos.

| File | What it defines | Test case |
|---|---|---|
| config/signing.yaml | SIGNING_ALG = ES256 for qx-payment-service | CR-06 |
| k8s/payment-deployment.yaml | env var + mounts keys from qx-key-service | CR-06, CR-01 |
| nginx/payment.conf | TLS cert from qx-key-service/certs/server.crt | CR-08 |
