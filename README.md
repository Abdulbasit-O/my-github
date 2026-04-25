# The Serverless Automator — AWS Lambda

An automated cloud cost-saving system built on AWS Lambda.
The goal is to stop paying for development servers that nobody is using after work hours.

## What I'm Building
Two Lambda functions that run in sequence every evening:

**5:00 PM — Backup**
- Detects running EC2 Development instances
- Backs up critical data to S3 before anything stops

**6:00 PM — Shutdown**
- Stops all running Development instances
- Sends a Slack notification confirming what was shut down

## Why This Matters
Forgotten development servers are one of the most common sources of unnecessary cloud spend. This automates the discipline that most teams rely on humans to remember and makes sure nothing is lost before the lights go off.

## Stack
AWS Lambda · Python (Boto3) · CloudWatch Events · S3 · Slack API · IAM

## The Checklist
- [ ] Write backup Lambda to snapshot/save Dev instance data to S3
- [ ] Write shutdown Lambda to stop Dev instances and notify Slack
- [ ] Configure CloudWatch Events — backup at 5 PM, shutdown at 6 PM
- [ ] Set up IAM roles with least-privilege permissions for both functions
- [ ] Test full sequence end to end and document findings

## Status
🔨 In progress