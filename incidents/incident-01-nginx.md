# Incident 01 — Website Unavailable

## Impact
Website hosted on the Ubuntu EC2 instance was unavailable.

## Investigation
1. Tested the web service using `curl localhost`.
2. Connection to port 80 failed.
3. Checked the Nginx service status.
4. Nginx was found inactive/dead.

## Root Cause
The Nginx web service had been stopped.

## Resolution
Started the Nginx service using `systemctl`.

## Verification
`curl localhost` successfully returned the Nginx welcome page.

## Jira
CIIML-1

## Status
Resolved
