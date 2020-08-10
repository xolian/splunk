
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

## References
https://www.splunk.com/en_us/blog/search.html?query=%22Deploy%2BSplunk%2BEnterprise%2Bon%2BKubernetes%22
https://www.splunk.com/en_us/blog/it/an-insider-s-guide-to-splunk-on-containers-and-kubernetes.html
https://medium.com/faun/logging-in-kubernetes-using-splunk-c2785948fdc0
