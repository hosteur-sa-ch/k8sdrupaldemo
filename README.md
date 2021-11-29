# k8sdrupaldemo
K8s deployment demo for Drupal

Script d'installation de Drupal 

>Prerequis : K8s v1.20, Ingress Nginx
```
OPERATOR_NAMESPACE=drupal
kubectl create namespace "$OPERATOR_NAMESPACE"
kubectl apply -f https://raw.githubusercontent.com/hosteur-sa-ch/k8sdrupaldemo/main/drupal-persistentvolumeclaim.yaml
kubectl apply -f https://raw.githubusercontent.com/hosteur-sa-ch/k8sdrupaldemo/main/drupal-mysql.yaml
kubectl apply -f https://raw.githubusercontent.com/hosteur-sa-ch/k8sdrupaldemo/main/drupal.yaml
```
