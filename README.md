# ELK Stack Security Monitoring Platform

## Objectives

Deploy a modern ELK Stack environment using Docker to perform centralized security monitoring, log ingestion, event analysis, and security visualization.

## Technologies Used

* Docker
* Docker Compose V2
* Elasticsearch 8.15
* Logstash 8.15
* Kibana 8.15
* Linux Syslog
* JSON
* cURL
* jq

## Key Skills Demonstrated

* SIEM architecture deployment
* Centralized log aggregation
* Security event parsing
* Log ingestion pipelines
* Elasticsearch indexing and querying
* Kibana dashboarding
* Security monitoring workflows
* Threat detection logic
* Dockerized observability infrastructure

## Security Events Monitored

* Failed SSH login attempts
* Privilege escalation activity (sudo)
* Suspicious authentication behavior
* Source IP tracking

## Troubleshooting and Modernization

### Updated Docker Compose Usage

Replaced deprecated:
docker-compose up -d

With modern Docker Compose V2:
docker compose up -d

### Updated ELK Stack Version

Replaced outdated ELK 7.10.2 images with modern 8.15.3 versions for:

* Better security
* Modern Docker compatibility
* Long-term maintainability

### Resource Optimization

Reduced JVM memory allocations for low-memory cloud lab environments:

* Elasticsearch: 768MB heap
* Logstash: 384MB heap
* Kibana: 512MB node memory

### Logstash Pipeline Improvements

Implemented:

* Structured Grok parsing
* Event classification
* Timestamp normalization
* Security event tagging

## Outcome

Successfully deployed a complete Dockerized SIEM pipeline capable of ingesting, parsing, indexing, and visualizing Linux security events in real time.
