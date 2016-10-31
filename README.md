# OpenSips Metrics
==================
Part of IMS Dynamics VoIP Metrics

20161030 Sam J. Muller

Description
-----------

VoIP statistics for OpenSips. The module xmlrpc is polled every 5 seconds using Celery task, then the stats are parsed then pushed to InfluxDB.


Requirements
------------
- Python 2.7.x
- Celery
- Influxdb
- Supervisor
- OpenSips with module fifo, xmlrpc or unixsock

Overview
--------
Using Grafana as GUI:

opensips dialogs number (active + early states)

![opensips dialogs](http://195.154.255.170/img/cscf-gh.png)

opensips release causes (using redis for opensips "onreply" log storage)

![opensips releases](http://195.154.255.170/img/rel-gh.png)
