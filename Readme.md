# Build and run Prometheus and Grafana locally
1.     docker build -t prometheus . 
2.     docker run -p 9090:9090 prometheus
3.     docker run -p 3000:3000 grafana/grafana

For å nå prometheus gå til http://localhost:9090 og grafana http://localhost:3000

For en test kan du kjøre denne i consolen.

    up{instance="host.docker.internal:8080", job="spring-actuator"}

Hvis du nå slår av og på serveren burde du se i grafen at den endres fra 0 til 1 og motsatt. 

### Legge til datasource for grafana 

bruk host.docker.internal:8080 som ipadresse
