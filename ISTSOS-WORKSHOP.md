# OGRS 2016 - istSOS Workshop

[IstSOS](http://istsos.org) is an OGC SOS server implementation written in Python.

## The istSOS software

* istsoslib: service only, no interface
* walib: web administration through RESTful API
* wainterface: web administration interface
* PostgreSQL & PostGIS

## With istSOS you get...

* QI, native quality index, quality assessment of data
* MQTT for pubsub (http://mqtt.org)
* Virtual procedures (procedure == sensor): on-the-fly transformation of another sensor's data (similar to database view), e.g. virtual celsius temperature sensor based on actual kelvin sensor

## MQTT support

* Time series analysis
* Broker channel