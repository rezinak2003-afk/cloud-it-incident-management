# Cloud IT Incident Management Lab

A hands-on IT infrastructure and incident troubleshooting lab built using AWS EC2, Ubuntu Linux, networking concepts, and Jira.

## Project Overview

This project simulates common IT support incidents on an Ubuntu Linux server hosted on AWS EC2.

The objective was to practice a structured L1 troubleshooting workflow:

**Incident → Investigation → Root Cause → Resolution → Verification → Documentation**

## Architecture

```text
Windows Laptop
      |
      | SSH
      v
   Internet
      |
      v
   AWS VPC
      |
      v
Security Group
      |
      v
 Ubuntu EC2
      |
      +---- Nginx Web Server
      |
      +---- Linux Processes
      |
      +---- SSH
      |
      v
     Jira
```
