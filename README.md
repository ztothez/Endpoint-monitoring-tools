# Endpoint Monitoring Tools
Python-based utilities for collecting host-level telemetry and supporting security monitoring workflows.

This repository focuses on **endpoint visibility, system state inspection, and foundational telemetry collection**, designed to support detection engineering, SOC analysis, and local security monitoring use cases.

## Overview
This project provides lightweight scripts that gather **key system metrics and state information** from endpoints.

The tools are designed to act as **early-stage telemetry sources**, which can be:
* analyzed locally
* forwarded into SIEM pipelines
* extended into detection and alerting logic

The emphasis is on **understanding how endpoint data can be collected and used for security purposes**, rather than building full monitoring agents.

## Features
* **Host Telemetry Collection**
  Capture system-level metrics relevant to performance and security visibility.

* **System State Monitoring**
  Inspect runtime conditions such as resource usage and service status.

* **Modular Script Design**
  Each script operates independently and can be reused or integrated.

* **Extensible for Detection Use Cases**
  Designed to be adapted into alerting, baselining, or anomaly detection workflows.

## Included Tools
* **Disk Monitoring**
  Tracks disk usage and basic disk health indicators.

* **Memory Monitoring**
  Provides insight into memory consumption and system pressure.

* **Load Monitoring**
  Observes system load and execution pressure.

* **Service Status Checks**
  Verifies availability and state of system services.

## Use Cases
* **SOC Lab Environments**
  Simulating endpoint telemetry collection for analysis pipelines.

* **Detection Engineering Experiments**
  Building and testing detection logic using real system data.

* **SIEM Ingestion Prototyping**
  Generating structured data for log pipelines and correlation.

* **Local Troubleshooting & Visibility**
  Quick inspection of system state during analysis or debugging.

## Example Workflow
```text
[Endpoint Scripts]
        ↓
[Telemetry Output (JSON / logs)]
        ↓
[Log Forwarder / Collector]
        ↓
[SIEM / Analysis Platform]
        ↓
[Detection Logic / Alerts]
```

These tools are intended to represent the **first stage of a monitoring pipeline**.

## Tech Stack
* **Python**
* Standard system libraries (`os`, `psutil`, etc.)

## Design Principles
* **Minimal by Design**
  Focus on clarity and core functionality.

* **Composable**
  Scripts can be combined into larger workflows.

* **Transparent**
  Easy to understand, modify, and extend.

* **Security-Oriented Thinking**
  Built with detection and monitoring use cases in mind.

## Limitations
* Not a full endpoint detection or monitoring agent
* No built-in alerting or correlation logic
* No centralized management or scaling

These tools are intended as **building blocks for learning and prototyping**, not production systems.

## Positioning
A hands-on project demonstrating:
* Endpoint telemetry collection
* System monitoring fundamentals
* Detection engineering mindset
* Security-focused scripting and automation

## Future Improvements (Optional Ideas)
* Structured JSON output for SIEM ingestion
* Integration with log forwarders (e.g., syslog, Fluent Bit)
* Basic anomaly detection or threshold-based alerts
* Scheduled execution (cron / systemd timers)
* Centralized aggregation service
