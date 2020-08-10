
## Install Docker
'''
docker run -p 8000:8000 -e "SPLUNK_PASSWORD=<password>" \
             -e "SPLUNK_START_ARGS=--accept-license" \
             -it --name splunk-master-1 splunk/splunk:latest
'''

## Install K8s
'''
kubectl apply -f k8-splunk-single-instance.yaml
kubectl get pods
kubectl get pvc
'''
