# metrics-demo-infra

This Repository is used for the "CI/CD für Applikationsmonitoring" Webinar.

The main storyline consist of:

- Deploy a sample application "metrics-demo" which is exposing metrics
- Activate the [User Workload Monitoring](https://docs.openshift.com/container-platform/4.6/monitoring/enabling-monitoring-for-user-defined-projects.html) Feature of OpenShift
- Deploy a `ServiceMonitor` to extract custom metrics from the application
- Deploy a custom Grafana Instance using the community Grafana Operator
- Deploy a custom Grafana Dashboard for the application
- Introduce a new metric in the application together with the edit of the Grafana Dashboard showing that metric
- Deploy a custom `PrometheusRule` to define an alert

