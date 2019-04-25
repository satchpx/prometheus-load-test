# prometheus-load-test

Deploy a load testing tool for prometheus. The headless service will enable prometheus within the cluster to scrape metrics. If prometheus is running outside the cluster, point it to the NodePort.

## To deploy
```
git clone https://github.com/satchpx/prometheus-load-test.git
cd prometheus-load-test
kubectl apply -f avalance.yaml
```

### Credits: https://github.com/open-fresh/avalanche
