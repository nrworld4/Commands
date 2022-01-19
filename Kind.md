### Create Cluster
kind create cluster --name kafka-local --config kafka.yml

### Info
kubectl cluster-info --context kind-kafka-local

### Start
Create cluster starts it

### Stop
kind get nodes --name kafka-local | xargs docker stop
