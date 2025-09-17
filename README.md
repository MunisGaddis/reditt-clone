Deploy a Redit Clone with Kubernetes Ingress
minikube service reddit-clone-service --url
curl - L URL

To run app on browser we need to expose deployment

kubectl expose deployment reddit-clone-deployment --type=NodePort

kubectl port-forward svc/reddit-clone-service 3000:3000 --address 0.0.0.0 &

Access app: IP:Port

Enable ingress minikube
kubectl apply -f ingress.yml
curl -L domain.com/test

YouTube link: https://www.youtube.com/watch?v=9tl0A_rwgu4&t=698s
