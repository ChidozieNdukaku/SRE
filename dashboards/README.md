## Grafana Monitoring Dashboards

[Grafana](https://grafana.com/oss/grafana) is a multi-platform open source analytics and interactive visualization tool. It allows you to query, create dashboards, explore, and alert on metrics when connected to supported data sources.
For each of the Operate First managed services and applications, we have created example Grafana dashboards which can be used to visualize our [SLI/SLOs](https://github.com/operate-first/SRE/tree/master/sli-slo) defined for each of the applications.

These monitoring dashboards are useful for visualizing the metrics (such as Prometheus metrics) collected from the applications to track and analyze the system's overall health.
The dashboards can be altered, saved and reused as per your specific monitoring needs.

Dashboards are represented by the `GrafanaDashboard` custom resource. You can find example monitoring dashboards defined in separate `yaml` files for each of the Operate First managed applications in this folder. For more information on how these `yaml` files are defined, please refer to [this documentation](https://github.com/integr8ly/grafana-operator/blob/master/documentation/dashboards.md).

## Using the Dashboards

Grafana dashboards can easily be exported and imported, either from the UI or from the HTTP API.
Dashboards are exported in Grafana JSON format, and contain everything you need (layout, variables, styles, data sources, queries, etc) to import the dashboard at a later time.

You can import these dashboards in Grafana either by pasting the dashboard JSON text directly into the text area or directly uploading the JSON file. Make sure to add/connect your [data sources](https://grafana.com/docs/grafana/latest/datasources/) to Grafana and pick what data source you want the dashboard to use.

For more details on importing/exporting dashboards, you can refer to the Grafana documentation [here](https://grafana.com/docs/grafana/latest/dashboards/export-import/).