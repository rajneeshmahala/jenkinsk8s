# Jenkins on Kubernetes (Traefik Ingress)

## Apply
kubectl apply -f .

## Add Host Entry
<TRAEFIK-IP> jenkins.k8s.local

## Get Admin Password
kubectl exec -n jenkins deploy/jenkins -- cat /var/jenkins_home/secrets/initialAdminPassword
