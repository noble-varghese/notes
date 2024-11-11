---
date: 2024-11-11
title: "Understanding K9s Pod Information"
tags: [interpreting, k9s]
---

When using K9s to monitor Kubernetes infrastructure, you'll see several columns of information about your pods. Here's what each column in the display means:

![K9s interface showing pod information](/assets/notes/k9s-image.png)

| Column   | Description                                                                             |
| -------- | --------------------------------------------------------------------------------------- |
| NAME     | Pod name                                                                                |
| READY    | Number of pods in ready state / number of pods to be in ready state                     |
| RESTARTS | Number of times the pod has been restarted so far                                       |
| STATUS   | State of the pod life cycle (e.g., Running, Completed)                                  |
| CPU      | Current CPU usage (in milli-vCPU)                                                       |
| MEM      | Current main memory usage (in MiB)                                                      |
| %CPU/R   | Current CPU usage as a percentage of what has been requested by the pod                 |
| %MEM/R   | Current main memory usage as a percentage of what has been requested by the pod         |
| %CPU/L   | Current CPU usage as a percentage of the pod's limit (cannot exceed this limit)         |
| %MEM/L   | Current main memory usage as a percentage of the pod's limit (cannot exceed this limit) |
| IP       | IP address of the pod                                                                   |
| NODE     | Name of the node the pod is running on                                                  |
| AGE      | Age of the pod (s = seconds, m = minutes, h = hours, d = days)                          |
