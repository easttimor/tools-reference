# tools-reference

## Analyze
https://github.com/Netflix-Skunkworks/cloudtrail-anomaly
This project is a simple CloudTrail based anomaly detection for use in AWS. It keeps track of all API actions a principal calls (that are tracked by CloudTrail) for a N day period and alerts on new API calls after the N day period.

https://github.com/Netflix-Skunkworks/diffy
Diffy is a triage tool used during cloud-centric security incidents, to help digital forensics and incident response (DFIR) teams quickly identify suspicious hosts on which to focus their response.

https://github.com/FSecureLABS/awspx
awspx is a graph-based tool for visualizing effective access and resource relationships within AWS. It resolves policy information to determine what actions affect which resources, while taking into account how these actions may be combined to produce attack paths. Unlike tools like Bloodhound, awspx requires permissions to function — it is not expected to be useful in cases where these privileges have not been granted.

https://github.com/cloud-custodian/cloud-custodian
Cloud Custodian is a rules engine for managing public cloud accounts and resources. It allows users to define policies to enable a well managed cloud infrastructure, that's both secure and cost optimized. It consolidates many of the adhoc scripts organizations have into a lightweight and flexible tool, with unified metrics and reporting.

https://github.com/dowjones/hammer
Dow Jones Hammer is a multi-account cloud security tool for AWS. It identifies misconfigurations and insecure data exposures within most popular AWS resources, across all regions and accounts. It has near real-time reporting capabilities (e.g. JIRA, Slack) to provide quick feedback to engineers and can perform auto-remediation of some misconfigurations. This helps to protect products deployed on cloud by creating secure guardrails.

https://github.com/flosell/trailscraper

https://github.com/lyft/cartography

https://github.com/Netflix/security_monkey
Security Monkey monitors your AWS and GCP accounts for policy changes and alerts on insecure configurations.

https://github.com/turnerlabs/antiope
Antiope (PRONO An-Tie-Oh-Pee) is intended to be an open sourced framework for managing resources across hundreds of AWS Accounts. From a trusted Security Account, Antiope will leverage Cross Account Assume Roles to gather up resource data and store them in an inventory bucket. This bucket can then be index by ELK or your SEIM of choice to provide easy searching of resources across hundreds of AWS accounts.

## Exploit TTPs

https://github.com/FSecureLABS/leonidas
This is the repository containing Leonidas, a framework for executing attacker actions in the cloud. It provides a YAML-based format for defining cloud attacker tactics, techniques and procedures (TTPs) and their associated detection properties.

https://github.com/RhinoSecurityLabs/IPRotate_Burp_Extension

https://github.com/RhinoSecurityLabs/pacu

https://github.com/RhinoSecurityLabs/AWS-IAM-Privilege-Escalation
Scan AWS IAM to identify principals subject to the following methods:
https://rhinosecuritylabs.com/aws/aws-privilege-escalation-methods-mitigation/

## Play

https://github.com/RhinoSecurityLabs/cloudgoat

http://flaws.cloud/

http://flaws2.cloud/
