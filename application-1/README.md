# PrometheusRule Helm Chart

This chart installs a resource kind: `PrometheusRule`, that can specify alerting and recording rules for Prometheus.

For details on alerting and recording rules check the official docs:

- [Alerting Rules](https://prometheus.io/docs/prometheus/latest/configuration/alerting_rules/)
- [Recording Rules](https://prometheus.io/docs/prometheus/latest/configuration/recording_rules/)

Check the [values.yaml](values.yaml) file for a description and examples of all the possible settings.

## Configuration

| Parameter                        | Description                                                            | Default                             |
|----------------------------------|------------------------------------------------------------------------|-------------------------------------|
| applicationName                  | Application name to be monitored                                       | ""                                  |
| prometheusRule.namespace         | ServiceMonitor namespace                                               | ""                                  |
| prometheusRule.additionalLabels  | Any additional Label to be added to the ServiceMonitor                 | lma: enabled                        |
| alertingRules                    | List of alerting rules                                                 | []                                  |
| recordingRules                   | List of recording rules                                                | []                                  |
