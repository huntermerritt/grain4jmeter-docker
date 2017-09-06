# grain4jmeter-docker
Docker container for Grafana &amp; InfluxDB for JMeter.

Inspired by https://github.com/sarkershantonu/jmeter-grafana-influxdb-docker but changed to have both Grafana and InfluxDB in the same image.

Purpose of this image is to show realtime results of JMeter testing in testing and demonstration environments.
Sample dashboard is configured to show requests/seconds, average response time/second and couple of others.



# Usage

Get container from Dockerhub:

- docker pull kazhar/grain4jmeter

Or build docker image using:

- docker build -t grain4jmeter .

Run docker container, expose port 3000 and 2003:

- docker run -it --rm -p 3000:3000 -p 2003:2003 kazhar/grain4jmeter

Open Grafana dashboard:

- http://127.0.0.1:3000/dashboard/db/jmeter

Configure JMeter:

- http://jmeter.apache.org/usermanual/realtime-results.html


# License

MIT for my stuff. Files not mine may have other licenses.
