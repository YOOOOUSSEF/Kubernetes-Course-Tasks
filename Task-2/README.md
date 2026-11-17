# Task_2
## 1) uploading 2 images (webapp-mysql:task2 and webapp-api:task2):
![2-images-loaded](images/2-images-loaded.png)


## 2) checking on configMap and secret after creation:
![configMap-secret](images/configMap-secret.png)

## 3) pv and pvc creation (connecting pvc to pv through storageclassName,accessMode,volumeName,storage): 
![pv-pvc-creation](images/pv-pvc-creation.png)


## 4) logs of mysql pod ( "ready for connections" ) and endpoint of its service:
![logs-of-mysql-pod](images/logs-of-mysql-pod.png)
![endpoint-of-mysql-service](images/endpoint-of-mysql-service.png)

## 5) env vars of webapp-api pod:
![env-vars-(secrets+configMap)-of-webapp](images/env-vars-(secrets+configMap)-of-webapp.png)

## 6) after createing 2 webapp-api pods (3 pods running):
![3pods-running](images/3pods-running.png)

## 7) some checks ( pod mysql on which node => minikube-m02 (because pv is located there)) and some requests:
![some-checks-on-system](images/some-checks-on-system.png)


## 8) Write a message (return response with id and pod name):
![post-request](images/post-request.png)

## 9) Read messages:
![get-request-all-messages](images/get-request-all-messages.png)

## 10) Data survives a restart (because the new mysql pod has the same volumes and volumeMounts config, so it mounts mysql-pvc at /var/lib/mysql and finds the existing data):
![data-persisted](images/data-persisted.png)



