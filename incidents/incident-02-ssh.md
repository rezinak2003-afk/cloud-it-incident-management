# Incident 02 — SSH Access Failure

## Impact
Unable to remotely connect to the Ubuntu EC2 instance through SSH.

## Investigation
1. Attempted SSH connection from Windows PowerShell.
2. Connection timed out on TCP port 22.
3. Checked the EC2 Security Group inbound rules.
4. Found that no inbound SSH rule was present.

## Root Cause
SSH/TCP port 22 was not allowed by the EC2 Security Group.

## Resolution
Restored the SSH/TCP port 22 inbound rule and restricted the source to My IP.

## Verification
Successfully reconnected to the Ubuntu EC2 instance using SSH.

## Jira
CIIML-2

## Status
Resolved
