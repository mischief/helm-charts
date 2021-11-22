# charts

# tl;dr

Helm:

	helm repo add mischief https://mischief.github.io/helm-charts
	helm repo update mischief
	helm install mischief-nginx mischief/nginx

Terraform:

```hcl
resource "helm_release" "test" {
  name       = "test-release"
  namespace  = "test-namespace"
  repository = "https://mischief.github.io/helm-charts"
  chart      = "nginx"
}
```

