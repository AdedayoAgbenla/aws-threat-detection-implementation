<h1>Continuous Monitoring &amp; Threat Detection Implementation</h1>
<h3>AWS Enterprise Environment</h3>

<h2>Overview</h2>
<p>
  This repository documents the implementation of continuous monitoring and threat detection controls across an AWS environment
  for a cloud-based organization. The goal was to detect suspicious activity early, improve investigation capabilities, and
  strengthen incident response through centralized logging and alerting.
</p>

<hr/>

<h2>Key Responsibilities</h2>
<ul>
  <li>Enabled Amazon GuardDuty for threat detection across CloudTrail, VPC Flow Logs, and DNS logs</li>
  <li>Configured SNS notifications for security findings and validated alert delivery using sample GuardDuty findings</li>
  <li>Implemented an EventBridge-triggered Lambda workflow to auto-remediate low-severity GuardDuty findings (with least-privilege considerations)</li>
  <li>Deployed AWS CloudTrail and integrated it with CloudWatch Logs for near real-time monitoring of API activity</li>
  <li>Built CloudWatch metric filters and alarms for high-risk events (Root usage, IAM policy changes, unauthorized API calls, Console login without MFA, CloudTrail changes)</li>
  <li>Enabled AWS Security Hub and integrated data sources (GuardDuty, AWS Config, Inspector, Macie) to aggregate security findings</li>
  <li>Validated detection and remediation through controlled misconfigurations (e.g., public S3 access, missing S3 access logging, insecure default security group rules)</li>
  <li>Enabled VPC Flow Logs to CloudWatch, verified ACCEPT/REJECT traffic, and created alarms for rejected traffic and log delivery failures</li>
</ul>

<hr/>

<h2>Tools &amp; Technologies</h2>
<ul>
  <li>Amazon GuardDuty</li>
  <li>AWS CloudTrail</li>
  <li>AWS Security Hub</li>
  <li>Amazon VPC Flow Logs</li>
  <li>Amazon CloudWatch (Logs, Metric Filters, Alarms)</li>
  <li>Amazon SNS</li>
  <li>AWS Lambda</li>
  <li>Amazon EventBridge</li>
  <li>AWS Config</li>
  <li>Amazon Inspector</li>
  <li>Amazon Macie</li>
</ul>

<hr/>

<h2>Impact</h2>
<ul>
  <li>Improved visibility of API activity and network traffic across the AWS environment</li>
  <li>Enabled faster detection and alerting for suspicious IAM and root account activity</li>
  <li>Centralized security findings to support investigation and response workflows</li>
  <li>Reduced response time for low-severity threats through automated remediation</li>
  <li>Strengthened security posture through continuous monitoring and validated controls</li>
</ul>

<hr/>

<h2>Author</h2>
<p>
  <strong>Adedayo</strong><br/>
  AWS Cloud Architect | Cloud Security Specialist
</p>

<hr/>

<h2>Disclaimer</h2>
<p>
  All documentation is anonymized and does not contain confidential or proprietary information.
</p>
