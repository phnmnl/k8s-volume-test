# Kuberbetes persistent volume test
This repository contains read/write speed tests for Kubernetes Persistent Volumes (PVs).

## How to run the test

### Prerequisites
We assume you have:

- A Kubernetes cluster up and running with configured kubectl CLI
- A PV that supports ReadWriteMany with at least 5GB of capacity

### Running the tests

Please clone this repository, and locate into it:

```bash
git clone https://github.com/phnmnl/k8s-volume-test.git
cd k8s-volume-test
```

Create a PersistentVolumeClaim using `pvc.yml`:

```bash
kubectl apply -f pvc.yml
```
