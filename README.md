elasticsearch-collectd-plugin
=====================

A [ElasticSearch](http://elasticsearch.org) plugin for [collectd](http://collectd.org) using collectd's [Python plugin](http://collectd.org/documentation/manpages/collectd-python.5.shtml).

Common Stats :
 * Docs (Total docs & Deleted docs)
 * Store size 
 * Indexing (Total, time, Total delete, Delete time)
 * Get (Total, Time, Exists otal, Exists time, Missing total, Missing Time)
 * Search (Total query, total time, total fetch, total fetch time)
 * JVM Memory (Heap commited, Heap Used, Non heap commited, Non heap used)
 * JVM Threads (Count & Peak)
 * JVM GC (Time & Count)
 * Transport stats (Server open, RX count, RX size, TX count, TX size)
 * HTTP Stats (Current open & Total open)

ES 1.0 Stats :
 * Cache (Field Eviction, Field Size, Filter evictions, Filter size)
 * JVM Collectors
 * FLush (Total count, total time)
 * Merges (Current count, current docs, current size, Merge total size, docs a time)
 * Refresh (Total & Time)

Install
-------
 1. Place elasticsearch.py in collectd'opt/collectd/lib/collectd/plugins/python (assuming you have collectd installed to /opt/collectd).
 2. Configure the plugin (see below).
 3. Restart collectd.

Configuration
-------------
 * See elasticsearch.conf
 * Set the version (0.9 or 1.0), default is 1.0

Requirements
------------
 * collectd 4.9+
 * Elasticsearch 0.9.x or 1.0.x
