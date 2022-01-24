# Twitter Application - DevOps

Deploy a twitter application using docker image on Azure Elastic Kubernetes service (aks) with terraform, perform HPA autoscaling based on cpu and memory, monitoring with Prometheus and Grafana. Alert messages can be send to slack using alert manager. Locust was used for load testing.

## Technologies Used:
- Azure Elastic Kubernetes service (AKS) with terraform
- Horizontal Pod Scaler (HPA)
- Metric server
- Kube state metrics
- Prometheus
- Grafana
- Locust
- AlertManager
- React ( Frontend)
- Python Flask (Backend)


## Setup to run the Project
- Clone or fork this repository

### Python Flask (locally)

1. Install with pip
   ```
   py -m pip install -r requirements.txt
   ```
2. Start the flask server
   ```
   py <name of file>.py
   ```

### React

1. Install all requirements packages for the file
   ```
   npm install
   ```
2. Build and run the file
   ```
   npm build
   ```
   ```
   npm run
   ```
3. Or the below command to perform any necessary building/prep tasks for your project
   ```
   npm run build

### Docker

1. Build the docker image by running:

```
docker build -t <YOUR_DOCKER_ID>/<name of the  file>
```

2. Push the image to Docker registry by running

```
docker push <YOUR_DOCKER_ID>/<name of the  file>
```


### Kubernets - Create deployment,service and pod for the file and execute the below comments to run

1. Generate yaml file create it by running the below command 

```
kubectl create -f <name of the  file>.yaml
```
2. Generate yaml file for the deployment and create it by running the below command 

```
kubectl apply -f <name of the  file>.yaml
```
3. Generate yaml file for the service and create it by running the below command 

```
kubectl create -f service-<name of the  file>.yaml
```

For detailed running instruction please click [here](Documents/project_cheatsheet.txt).

## Personal Details
- Name: Anjali Sajeevan
- NUID: 001563277
