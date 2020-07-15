# AWS Tools Reference
Useful offensive and defensive OSS

## Info
https://gist.github.com/kmcquade/33860a617e651104d243c324ddf7992a
@kmcquade3
"AWS API calls that return credentials"

https://rhinosecuritylabs.com/aws/aws-privilege-escalation-methods-mitigation/

## Analyze and Defend

https://github.com/Netflix-Skunkworks/cloudtrail-anomaly
"This project is a simple CloudTrail based anomaly detection for use in AWS. It keeps track of all API actions a principal calls (that are tracked by CloudTrail) for a N day period and alerts on new API calls after the N day period."

https://github.com/Netflix-Skunkworks/diffy
"Diffy is a triage tool used during cloud-centric security incidents, to help digital forensics and incident response (DFIR) teams quickly identify suspicious hosts on which to focus their response."

https://github.com/FSecureLABS/awspx
"awspx is a graph-based tool for visualizing effective access and resource relationships within AWS. It resolves policy information to determine what actions affect which resources, while taking into account how these actions may be combined to produce attack paths. Unlike tools like Bloodhound, awspx requires permissions to function — it is not expected to be useful in cases where these privileges have not been granted."

https://github.com/cloud-custodian/cloud-custodian
"Cloud Custodian is a rules engine for managing public cloud accounts and resources. It allows users to define policies to enable a well managed cloud infrastructure, that's both secure and cost optimized. It consolidates many of the adhoc scripts organizations have into a lightweight and flexible tool, with unified metrics and reporting."

https://github.com/dowjones/hammer
"Dow Jones Hammer is a multi-account cloud security tool for AWS. It identifies misconfigurations and insecure data exposures within most popular AWS resources, across all regions and accounts. It has near real-time reporting capabilities (e.g. JIRA, Slack) to provide quick feedback to engineers and can perform auto-remediation of some misconfigurations. This helps to protect products deployed on cloud by creating secure guardrails."

https://github.com/flosell/trailscraper
"A command-line tool to get valuable information out of AWS CloudTrail and a general purpose toolbox for working with IAM policies"

https://github.com/lyft/cartography
"Cartography is a Python tool that consolidates infrastructure assets and the relationships between them in an intuitive graph view powered by a Neo4j database."

https://github.com/Netflix/security_monkey
"Security Monkey monitors your AWS and GCP accounts for policy changes and alerts on insecure configurations."

https://github.com/turnerlabs/antiope
"Antiope (PRONO An-Tie-Oh-Pee) is intended to be an open sourced framework for managing resources across hundreds of AWS Accounts. From a trusted Security Account, Antiope will leverage Cross Account Assume Roles to gather up resource data and store them in an inventory bucket. This bucket can then be index by ELK or your SEIM of choice to provide easy searching of resources across hundreds of AWS accounts."

https://github.com/NotSoSecure/cloud-service-enum/
Permissions enumeration.

https://github.com/sa7mon/S3Scanner
"A tool to find open S3 buckets and dump their contents"

https://github.com/nccgroup/ScoutSuite
"Scout Suite is an open source multi-cloud security-auditing tool, which enables security posture assessment of cloud environments. Using the APIs exposed by cloud providers, Scout Suite gathers configuration data for manual inspection and highlights risk areas. Rather than going through dozens of pages on the web consoles, Scout Suite presents a clear view of the attack surface automatically."

https://github.com/salesforce/cloudsplaining
Cloudsplaining is an AWS IAM Security Assessment tool that identifies violations of least privilege and generates a risk-prioritized HTML report.

## Exploit TTPs

https://github.com/RhinoSecurityLabs/pacu
"Pacu is an open source AWS exploitation framework, designed for offensive security testing against cloud environments."

https://github.com/Voulnet/barq 
"barq is a post-exploitation framework that allows you to easily perform attacks on a running AWS infrastructure. It allows you to attack running EC2 instances without having the original instance SSH keypairs. It also allows you to perform enumeration and extraction of stored Secrets and Parameters in AWS."

https://github.com/FSecureLABS/leonidas
This is the repository containing Leonidas, a framework for executing attacker actions in the cloud. It provides a YAML-based format for defining cloud attacker tactics, techniques and procedures (TTPs) and their associated detection properties.

https://github.com/RhinoSecurityLabs/IPRotate_Burp_Extension
"Extension for Burp Suite which uses AWS API Gateway to change your IP on every request."

https://github.com/RhinoSecurityLabs/AWS-IAM-Privilege-Escalation
Scan AWS IAM to identify principals subject to the following methods:
* https://rhinosecuritylabs.com/aws/aws-privilege-escalation-methods-mitigation/

https://github.com/andresriancho/nimbostratus
"Tools for fingerprinting and exploiting Amazon cloud infrastructures."

https://github.com/jordanpotti/AWSBucketDump
"AWSBucketDump is a tool to quickly enumerate AWS S3 buckets to look for loot. It's similar to a subdomain bruteforcer but is made specifically for S3 buckets and also has some extra features that allow you to grep for delicious files as well as download interesting files if you're not afraid to quickly fill up your hard drive."

## Code Quality

https://github.com/duo-labs/parliament
"parliament is an AWS IAM linting library"

https://github.com/liamg/tfsec
"tfsec uses static analysis of your terraform templates to spot potential security issues."

https://github.com/bridgecrewio/checkov
"Checkov is a static code analysis tool for infrastructure-as-code. It scans cloud infrastructure provisioned using Terraform, Cloudformation or Kubernetes and detects security and compliance misconfigurations."

## Learn

https://www.practicalcloudsecurity.com/ by Chris Farris (@jcfarris)
"a website designed to help busy security practitioners navigate the intricacies of AWS’s Service Offerings"

https://github.com/RhinoSecurityLabs/cloudgoat
"CloudGoat is Rhino Security Labs' "Vulnerable by Design" AWS deployment tool."

https://github.com/andresriancho/nimbostratus-target
"This code deploys an Amazon AWS infrastructure which has various vulnerabilities and weak configuration settings which can be exploited using nimbostratus."

http://flaws.cloud/ by Scott Piper (@0xdabbad00)

http://flaws2.cloud/ by Scott Piper (@0xdabbad00)
