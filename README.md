InfluxDB Container With External Storage
========================================

Prerequisites
=============

* Git
* Docker
* Internet Access

Build The Docker Container
==========================

* Clone the repository - git clone https://github.com/InfoSec812/InfluxDB-Docker.git
* Change into the repo directory - cd InfluxDB-Docker
* Build the Docker container - docker build -t InfluxDB ./

Run The Docker Container
========================

* Create a data directory where the persistent data will be stored <datadir>
* Run the container - docker run -d -v <datadir>:/data -p 8083:8083 -p 8084:8084 -p 8086:8086 InfluxDB

