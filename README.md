# metrics-demo-infra

This Repository is used for the "CI/CD für Applikationsmonitoring" Webinar.

_Prerequisites_

- Activate the [User Workload Monitoring](https://docs.openshift.com/container-platform/4.6/monitoring/enabling-monitoring-for-user-defined-projects.html) Feature of OpenShift
- Install the community Grafana Operator

The main storyline consist of:

- Deploy a sample application "metrics-demo" which is exposing metrics
  - run `kustomize build ./manifests/argocd/apps/product-metrics | oc apply -f -`
- Deploy a `ServiceMonitor` to extract custom metrics from the application
- Deploy a custom Grafana Instance using the community Grafana Operator
- Deploy a custom Grafana Dashboard for the application
- Introduce a new metric in the application together with the edit of the Grafana Dashboard showing that metric
- Deploy a custom `PrometheusRule` to define an alert
