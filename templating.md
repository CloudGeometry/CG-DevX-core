# Templating

This section describes platform reference implementation templating process. All the values templated with - `<>`` under
/platform folder will bre replaced with corresponding values generated by the system during setup process.

## Input values placeholder reference

Templating variables reference to input parameters

- `<OWNER_EMAIL>` - email
- `<CLOUD_PROVIDER>` - cloud-provider
- `<CLOUD_PROFILE>` - cloud-profile
- `<CLOUD_ACCOUNT_ACCESS_KEY>` - cloud-account-key
- `<CLOUD_ACCOUNT_ACCESS_SECRET>` - cloud-account-secret
- `<CLOUD_REGION>` - cloud-region
- `<PRIMARY_CLUSTER_NAME>` - cluster-name
- `<DNS_REGISTRAR>` - dns-registrar
- `<DNS_REGISTRAR_ACCESS_TOKEN>` - dns-registrar-token
- `<DNS_REGISTRAR_ACCESS_KEY>` - dns-registrar-key
- `<DNS_REGISTRAR_ACCESS_SECRET>` - dns-registrar-secret
- `<DOMAIN_NAME>` - domain-name
- `<GIT_PROVIDER>` - git-provider
- `<GIT_ORGANIZATION_NAME>` - git-org
- `<GIT_ACCESS_TOKEN>` - git-access-token
- `<GITOPS_REPOSITORY_NAME>` - gitops-repo-name
- `<GITOPS_REPOSITORY_TEMPLATE_URL>` - gitops-template-url
- `<GITOPS_REPOSITORY_TEMPLATE_BRANCH>` - gitops-template-branch

## Generated

Templating variables generated during setup process

### Internal values

- `<GIT_REPOSITORY_GIT_URL>` - Target git repository Git URL
- `<GIT_REPOSITORY_ROOT>` - Git repository URL used for referencing repos including wildcard
- `<CC_CLUSTER_FQDN>` - K8s Control Center (AKA primary) cluster FQDN
- `<HARBOR_REGISTRY_URL>`

### IAM roles

IAM roles for core components created during setup process

- `<VAULT_IAM_ROLE_RN>`
- `<ARGO_CD_IAM_ROLE_RN>`
- `<ARGO_WORKFLOW_IAM_ROLE_RN>`
- `<ATLANTIS_IAM_ROLE_RN>`
- `<HARBOR_IAM_ROLE_RN>`
- `<CERT_MANAGER_IAM_ROLE_RN>`
- `<EXTERNAL_DNS_IAM_ROLE_RN>`

### Ingress

Ingress URLs for core components. Note!: URL does not contain protocol prefix

- `<VAULT_INGRESS_URL>`
- `<ARGO_CD_INGRESS_URL>`
- `<ARGO_WORKFLOW_INGRESS_URL>`
- `<ATLANTIS_INGRESS_URL>`
- `<HARBOR_INGRESS_URL>`
- `<GRAFANA_INGRESS_URL>`
- `<SONARQUBE_INGRESS_URL>`

### Atlantis
Secret for Atlantis webhook

- `<ATLANTIS_WEBHOOK_SECRET>`

### Github
bot user's keypair

- `<VCS_BOT_SSH_PUBLIC_KEY>`
- `<VCS_BOT_SSH_PRIVATE_KEY>`

### OIDC

OIDC provider configuration Note!: URL does not contain protocol prefix

- `<OIDC_PROVIDER_URL>`
- `<OIDC_PROVIDER_AUTHORIZE_URL>`
- `<OIDC_PROVIDER_TOKEN_URL>`
- `<OIDC_PROVIDER_USERINFO_URL>`
- `<ARGO_CD_OAUTH_CALLBACK_URL>`

### K8s

- `<CC_CLUSTER_ENDPOINT>`
- `<CC_CLUSTER_OIDC_PROVIDER>`
- `<K8S_AWS_SERVICE_ACCOUNT_ROLE_MAPPING>`
- `<K8S_AZURE_SERVICE_ACCOUNT_ROLE_MAPPING>`

### Network

- `<NETWORK_ID>`
- `<PUBLIC_SUBNET_ID>`
- `<PRIVATE_SUBNET_ID>`
- `<AZ_IDS>`
