# Nexus Repository Manager 3 Pro Helm Chart 

This Helm chart configures the Kubernetes resources 
that are needed for a resilient Nexus Repository deployment on AWS 

## Deployment
1. Pull the [nxrm-resiliency-aws-helmchart](https://github.com/sonatype/nxrm-resiliency-aws-helmchart).
1. Ensure you have updated your values.yaml with appropriate values for your environment.
1. Install the chart using the following:
```helm install nxrm aetion/nxrm3 --values values.yaml```
1. Get the Nexus Repository link using the following:
```kubectl get ingresses -n nexus```

## Uninstall
To uninstall the deployment, use the following:
  ```helm uninstall nxrm```
