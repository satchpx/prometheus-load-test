# prometheus-load-test

Deploy a load testing tool for prometheus. The headless service will enable prometheus within the cluster to scrape metrics. If prometheus is running outside the cluster, point it to the NodePort.

## To deploy
```
git clone https://github.com/satchpx/prometheus-load-test.git
cd prometheus-load-test
kubectl apply -f avalance.yaml
```

To run the load tester standalone, and point prometheus to srape:
```
git clone https://github.com/satchpx/prometheus-load-test.git
cd prometheus-load-test
./run
```

Note that this will serve metrics on localhost:9030. This can be picked up by prometheus by adding <node-ip>:9030 as a target for prometheus


### Credits: https://github.com/open-fresh/avalanche
