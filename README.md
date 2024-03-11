# Grafana-Prometheus
What is the use case of Grafana and Prometheus

Grafana is a multi-platform open source analytics and interactive visualization web application. It provides charts, graphs, and alerts for the web when connected to supported data sources.

Prometheus is a free software application used for event monitoring and alerting. It records metrics in a time series database built using an HTTP pull model, with flexible queries and real-time alerting.

Install Grafana on Debian or Ubuntu

1. Install the prerequisite packages:
   
   sudo apt-get install -y apt-transport-https software-properties-common wget

3. Import the GPG key:
   
   sudo mkdir -p /etc/apt/keyrings/
   wget -q -O - https://apt.grafana.com/gpg.key | gpg --dearmor | sudo tee /etc/apt/keyrings/grafana.gpg > /dev/null

4. To add a repository for stable releases, run the following command:

   echo "deb [signed-by=/etc/apt/keyrings/grafana.gpg] https://apt.grafana.com stable main" | sudo tee -a /etc/apt/sources.list.d/grafana.list

5. To add a repository for beta releases, run the following command:
   
   echo "deb [signed-by=/etc/apt/keyrings/grafana.gpg] https://apt.grafana.com beta main" | sudo tee -a /etc/apt/sources.list.d/grafana.list

6. Run the following command to update the list of available packages:
   
   # Updates the list of available packages
     sudo apt-get update

7. To install Grafana Enterprise, run the following command:
   
   # Installs the latest Enterprise release:
     sudo apt-get install grafana-enterprise

9. Restart the Grafana service
   
   systemctl restart garfana.service

10. Check the status Grafana service running or not
    
   systemctl staus garfana.service

   If all working good then copy your localhost IP and use port number 3000, by defult Grafana use port number 3000
   http://localhost:3000/


   PROMETHEUS & NODE_EXPORTER INSTALLATION 
   
   [https://prometheus.io/docs/prometheus/latest/installation/](https://prometheus.io/download/)

   PROMETHEUS use defult port number : 9090
   
   NODE_EXPORTER use defult port number : 9100





