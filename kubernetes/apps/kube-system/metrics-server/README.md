# Overview
Metrics Server is a scalable, efficient source of container resource metrics for Kubernetes built-in autoscaling pipelines.

Metrics Server collects resource metrics from Kubelets and exposes them in Kubernetes apiserver through Metrics API for use by Horizontal Pod Autoscaler and Vertical Pod Autoscaler. Metrics API can also be accessed by kubectl top, making it easier to debug autoscaling pipelines.

Caution

Metrics Server is meant only for autoscaling purposes. For example, don't use it to forward metrics to monitoring solutions, or as a source of monitoring solution metrics. In such cases please collect metrics from Kubelet /metrics/resource endpoint directly.

Metrics Server offers:

A single deployment that works on most clusters (see Requirements)
Fast autoscaling, collecting metrics every 15 seconds.
Resource efficiency, using 1 mili core of CPU and 2 MB of memory for each node in a cluster.
Scalable support up to 5,000 node clusters.
