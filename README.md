elasticsearch-1.0-collectd-plugin
=====================

A [ElasticSearch](http://elasticsearch.org) plugin for [collectd](http://collectd.org) using collectd's [Python plugin](http://collectd.org/documentation/manpages/collectd-python.5.shtml).

Data captured includes:

 * JVM Memory
 * Search Time
 * Threads
 * Transport Bytes
 * and many more ...

Install
-------
 1. Place elasticsearch.py in collectd'opt/collectd/lib/collectd/plugins/python (assuming you have collectd installed to /opt/collectd).
 2. Configure the plugin (see below).
 3. Restart collectd.

Configuration
-------------
See elasticsearch.conf

Requirements
------------
 * collectd 4.9+
 * Elasticsearch 1.0
