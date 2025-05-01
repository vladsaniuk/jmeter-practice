# JMeter performance testing 
Via GUI: Install JMeter, start server, open perf_testing_homework.jmx, run tests by clicking "Start" button.

## Influx and Grafana setup
Install Docker, run `docker-compose -f docker-compose.yaml up --detach`
### To configure integaration between Grafana and InfluxDB
1) Open Grafana at http://localhost:3000
2) Go to Connections -> Data Sources, search for InfluxDB
3) Set:
    * URL = http://influxdb:8086 
    * Database = mybucket 
    * User = admin 
    * Password = my-super-secret-auth-token 
### Import JMeter Grafana dashboard
1) Go to Dashboards -> New -> Import 
2) Input 4026 and click Load

## Screenshots 
Grafana dashboard
![Alt text](screenshots/grafana.png?raw=true "Grafana dashboard")
JMeter
![Alt text](screenshots/jmeter.png?raw=true "JMeter")
