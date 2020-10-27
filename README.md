# Monitoring
Collection of examples for monitoring and visualization of host- and app-based metrics based on Prometheus and Grafana. Additionally, an example posting alarm messages to a Slack channel using the Alertmanager of Prometheus is presented.

The following metrics are monitored, visualized and partly integrated in an alarm:
* host-based metrics:
	* CPU usage
	* used disk space, RAM
	* uptime
* app-based metrics:
	* availability of specific standalone docker containers
	* availability of postgreSQL DB
	* number of transactions, active/ idle sessions in postgreSQL DB
	* number of returned, fetched, inserted, updated rows in postgreSQL DB
	* size of schemas in postgreSQL DB

## Grafana Dashboards
* General Dashboard: Overview about general health status of the servers based on host-based metrics (current RAM usage, current used disk space of relevant drives, current CPU usage).
* Sysadmin Overview Dashboard: Overview about the current values of the host-based metrics of the server (current RAM usage, current used disk space of relevant drives, current CPU usage) 
* Sysadmin Longterm Dashboard: Overview about the longterm trend of the host-based metrics of the server (RAM usage, used disk space of relevant drives) 
* Database Overview Dashboard: Overview about the current values of the app-based metrics of the database (used disk space for each complete DB/ DB schema)
* Database Longterm Dashboard: Overview about the longterm trend of the app-based metrics of the database (number of transactions per minute, number of idle/ active sessions, Inserted/ Updated/ Fetched/ Retuned Rows per Minute)
