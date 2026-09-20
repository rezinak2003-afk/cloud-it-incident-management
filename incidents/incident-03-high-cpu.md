# Incident 03 — High CPU Usage

## Impact
High CPU utilization affected available system resources.

## Investigation
1. Monitored running processes using `ps`.
2. Identified PID 3387 running the `yes` process.
3. Found the process consuming approximately 99.9% CPU.

## Root Cause
The `yes` process was continuously consuming CPU resources.

## Resolution
Terminated the abnormal process using `kill`.

## Verification
Confirmed that PID 3387 was no longer running.

## Jira
CIIML-3

## Status
Resolved
