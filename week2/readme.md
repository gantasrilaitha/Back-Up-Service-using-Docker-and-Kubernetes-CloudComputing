1. minikube start
2. 
```cd container/
docker build -t backup .
cd ..
```
3. docker image save -o backup.tar backup:latest
4. minikube image load backup.tar
5. kubectl create secret generic google-token --from-file=credentials/
6. kubectl apply -f pvc.yaml
7. kubectl apply -f cronjob.yaml

kubectl get pods --watch

cleanup:
8. kubectl delete cronjob backup-cronjob

9.
```minikube ssh
docker rmi backup
exit

minikube stop
```
