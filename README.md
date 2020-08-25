# kafkabench

Scripts and utlities for benchmarking Kafka on Kubernetes

# Installing Strimzi

```
./scripts/deploy_strimzi.sh
```

# Creating a cluster and generating config

```
./scripts/create_cluster.sh cluster1
```

NOTE: Add local host mappings for the hosts generated by the script, i.e. bootstrap.cluster1, broker-0.cluster1 etc.

# Run locally

```
export OMB_DIR=<path to openmessaging-benchmark checkout>
./scripts/run-omb.sh -d omb-drivers/driver-cluster1.yaml omb-workloads/1-topic-1-partition-1kb.yaml
```

