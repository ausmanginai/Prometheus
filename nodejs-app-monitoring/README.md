#### This project is for the Devops bootcamp module "Monitoring"

##### Metrics
The project exposes metrics on /metrics endpoint

To run the nodejs application:

    npm install 
    node app/server.js

To build the project:

    docker build -t repo-name/image-name:image-tag .
    docker push repo-name/image-name:image-tag


To deploy the application on a Kubernetes cluster:

    kubectl apply -f config-k8s.yaml 
    
To scrape the endpoint of your application, for Prometheus, deploy the ServiceMonitor:

    kubectl apply -f nodejs-servicemonitor.yaml 
    





