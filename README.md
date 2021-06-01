# Cloud Security Tools Reference
A collection of useful offensive and defensive open source software.

Table of Contents
=================
| Category      | [Amazon Web Services](#amazon-web-services)      | [Microsoft Azure](#microsoft-azure) | [Google Cloud Platform](#google-cloud-platform) |
| ----------- | ----------- | ----------- | ----------- |
| Analyze and Defend |[Analyze and Defend](#analyze-and-defend)|||
| |[Static Analysis](#static-analysis)|||
| |[Cloud Security Posture Management](#cloud-security-posture-management)|||
| |[Resource Tracking and Relationships](#resource-tracking-and-relationships)|||
| |[Identity and Access](#identity-and-access)|||
| ||||
| Identify and Exploit|[Recon / Enumeration](#recon-and-enumeration)|||
| |[Exploit TTPs](#exploit-ttps)|||
| ||||
| Learn |[Collections](#aws-collections)|||
| |[CTFs and Labs](#aws-ctfs-and-labs)|||


# Amazon Web Services
## Analyze and Defend

### CloudTrail API Activity
| Tool      | Link      | Description |
| ----------- | ----------- | ----------- |
| Cloudtrail Anomaly | https://github.com/Netflix-Skunkworks/cloudtrail-anomaly | "This project is a simple CloudTrail based anomaly detection for use in AWS. It keeps track of all API actions a principal calls (that are tracked by CloudTrail) for a N day period and alerts on new API calls after the N day period."| 
| Trailscraper | https://github.com/flosell/trailscraper | "A command-line tool to get valuable information out of AWS CloudTrail and a general purpose toolbox for working with IAM policies" | 

### Static Analysis
| Tool      | Link      | Description |
| -----------| ----------- | ----------- |
| KICS | https://github.com/Checkmarx/kics      | "Find security vulnerabilities, compliance issues, and infrastructure misconfigurations early in the development cycle of your infrastructure-as-code with KICS by Checkmarx." |
| CloudSploit Cloudformation | https://cloudsploit.com/cloudformation   | "Scan your Cloudformation templates for over 95 security risks in seconds for free." |
| Checkov | https://github.com/bridgecrewio/checkov | "Checkov is a static code analysis tool for infrastructure-as-code. It scans cloud infrastructure provisioned using Terraform, Cloudformation or Kubernetes and detects security and compliance misconfigurations." |
| parliament | https://github.com/duo-labs/parliament | "parliament is an AWS IAM linting library" |
| tfsec | https://github.com/liamg/tfsec | "tfsec uses static analysis of your terraform templates to spot potential security issues." |
| tflint | https://github.com/terraform-linters/tflint | "a framework and each feature is provided by plugins, the key features are as follows: Find possible errors (like illegal instance types) for Major Cloud providers (AWS/Azure/GCP). Warn about deprecated syntax, unused declarations. Enforce best practices, naming conventions." |
| terrafirma | https://github.com/wayfair/terrafirma | "Terraform static analysis tool designed for detecting security misconfigurations." |
| AirIAM | https://airiam.io/documentation.html | "AirIAM is a tool to identify and automate Least privilege IAM principles in AWS using Terraform."|
| CloudFormation Guard | https://github.com/aws-cloudformation/cloudformation-guard | "an open-source general-purpose policy-as-code evaluation tool" |

### Cloud Security Posture Management
| Tool      | Link      | Description |
| -----------| ----------- | ----------- |
| Prowler | https://github.com/toniblyx/prowler | "Prowler is a command line tool for AWS Security Best Practices Assessment, Auditing, Hardening and Forensics Readiness Tool."|
| ScoutSuite | https://github.com/nccgroup/ScoutSuite | "Scout Suite is an open source multi-cloud security-auditing tool, which enables security posture assessment of cloud environments. Using the APIs exposed by cloud providers, Scout Suite gathers configuration data for manual inspection and highlights risk areas. Rather than going through dozens of pages on the web consoles, Scout Suite presents a clear view of the attack surface automatically."|
| CS Suite | https://github.com/SecurityFTW/cs-suite | "CS Suite is a one stop tool for auditing the security posture of the AWS infrastructure and does system audits as well. CS Suite leverages current open source tools capabilities and has other missing checks added into one tool to rule them all."|
| Cloud Custodian | https://github.com/cloud-custodian/cloud-custodian | "Cloud Custodian is a rules engine for managing public cloud accounts and resources. It allows users to define policies to enable a well managed cloud infrastructure, that's both secure and cost optimized. It consolidates many of the adhoc scripts organizations have into a lightweight and flexible tool, with unified metrics and reporting."|
| Hammer | https://github.com/dowjones/hammer | "Dow Jones Hammer is a multi-account cloud security tool for AWS. It identifies misconfigurations and insecure data exposures within most popular AWS resources, across all regions and accounts. It has near real-time reporting capabilities (e.g. JIRA, Slack) to provide quick feedback to engineers and can perform auto-remediation of some misconfigurations. This helps to protect products deployed on cloud by creating secure guardrails."|
| Security Monkey | https://github.com/Netflix/security_monkey | "Security Monkey monitors your AWS and GCP accounts for policy changes and alerts on insecure configurations."|
| Diffy | https://github.com/Netflix-Skunkworks/diffy | "Diffy is a triage tool used during cloud-centric security incidents, to help digital forensics and incident response (DFIR) teams quickly identify suspicious hosts on which to focus their response." |

### Resource Tracking and Relationships
| Tool      | Link      | Description |
| ----------- | ----------- | ----------- |
| Smogcloud | https://github.com/BishopFox/smogcloud | Find exposed AWS cloud assets that you did not know you had. A comprehensive asset inventory is step one to any capable security program. |
| awspx | https://github.com/FSecureLABS/awspx | "awspx is a graph-based tool for visualizing effective access and resource relationships within AWS. It resolves policy information to determine what actions affect which resources, while taking into account how these actions may be combined to produce attack paths. Unlike tools like Bloodhound, awspx requires permissions to function — it is not expected to be useful in cases where these privileges have not been granted."|
| antiope | https://github.com/turnerlabs/antiope | "Antiope (PRONO An-Tie-Oh-Pee) is intended to be an open sourced framework for managing resources across hundreds of AWS Accounts. From a trusted Security Account, Antiope will leverage Cross Account Assume Roles to gather up resource data and store them in an inventory bucket. This bucket can then be index by ELK or your SEIM of choice to provide easy searching of resources across hundreds of AWS accounts."|
| cartography | https://github.com/lyft/cartography | "Cartography is a Python tool that consolidates infrastructure assets and the relationships between them in an intuitive graph view powered by a Neo4j database."|
| clouddiscovery | https://github.com/Cloud-Architects/cloudiscovery | Analyze AWS resources including reports and graph visualization.|
| Cloudlist | https://github.com/projectdiscovery/cloudlist | "Cloudlist is a tool for listing Assets from multiple Cloud Providers."|

### Identity and Access
| Name | Link      | Description |
| ----------- | ----------- | ----------- |
| Cloudsplaining | https://github.com/salesforce/cloudsplaining | Cloudsplaining is an AWS IAM Security Assessment tool that identifies violations of least privilege and generates a risk-prioritized HTML report.|
| SkyArk | https://github.com/cyberark/SkyArk/ | "SkyArk currently focuses on mitigating the new threat of Cloud Shadow Admins, and helps organizations to discover, assess and protect cloud privileged entities."|
| iamlive | https://github.com/iann0036/iamlive | Generate an IAM policy from AWS calls using client-side monitoring (CSM) or embedded proxy |
| Policy Sentry | https://github.com/salesforce/policy_sentry | "IAM Least Privilege Policy Generator."|

## Identify and Exploit

### Recon and Enumeration
| Tool | Link      | Description |
| ----------- | ----------- | ----------- |
| cloud_enum | https://github.com/initstring/cloud_enum | "Multi-cloud OSINT tool. Enumerate public resources in AWS, Azure, and Google Cloud."|
| Weird AAL | https://github.com/carnal0wnage/weirdAAL | Permissions enumeration and useful functions.|
| PMapper | https://github.com/nccgroup/PMapper | "Principal Mapper (PMapper) is a script and library for identifying risks in the configuration of AWS Identity and Access Management (IAM) for an AWS account or an AWS organization. It models the different IAM Users and Roles in an account as a directed graph, which enables checks for privilege escalation and for alternate paths an attacker could take to gain access to a resource or action in AWS."|
| s3 account search | https://github.com/WeAreCloudar/s3-account-search | "This tool lets you find the account id an S3 bucket belongs too."
| S3Scanner | https://github.com/sa7mon/S3Scanner | "A tool to find open S3 buckets and dump their contents"|
| AWSBucketDump | https://github.com/jordanpotti/AWSBucketDump | "AWSBucketDump is a tool to quickly enumerate AWS S3 buckets to look for loot. It's similar to a subdomain bruteforcer but is made specifically for S3 buckets and also has some extra features that allow you to grep for delicious files as well as download interesting files if you're not afraid to quickly fill up your hard drive."|
| Cloud Service Enum | https://github.com/NotSoSecure/cloud-service-enum/ | Permissions enumeration.|
| Enumerate IAM | https://github.com/andresriancho/enumerate-iam | Permissions enumeration.|
| aws public ips | https://github.com/arkadiyt/aws_public_ips | fetch all public IP addresses (both IPv4/IPv6) associated with an AWS account. |


### Exploit TTPs
| Tool | Link      | Description |
| ----------- | ----------- | ----------- |
| Pacu | https://github.com/RhinoSecurityLabs/pacu | "Pacu is an open source AWS exploitation framework, designed for offensive security testing against cloud environments." |
| dsnap | https://github.com/RhinoSecurityLabs/dsnap | Utility for downloading EBS snapshots using the EBS Direct API's."|
| burp - iprotate | https://github.com/RhinoSecurityLabs/IPRotate_Burp_Extension | "Extension for Burp Suite which uses AWS API Gateway to change your IP on every request." |
| endgame | https://github.com/DavidDikker/endgame | "one-liner commands to backdoor an AWS account's resources with a rogue AWS account - or share the resources with the entire internet" |
| barq | https://github.com/Voulnet/barq | "barq is a post-exploitation framework that allows you to easily perform attacks on a running AWS infrastructure. It allows you to attack running EC2 instances without having the original instance SSH keypairs. It also allows you to perform enumeration and extraction of stored Secrets and Parameters in AWS." |
| leonidas | https://github.com/FSecureLABS/leonidas | This is the repository containing Leonidas, a framework for executing attacker actions in the cloud. It provides a YAML-based format for defining cloud attacker tactics, techniques and procedures (TTPs) and their associated detection properties. |
| nimbostratus | https://github.com/andresriancho/nimbostratus | "Tools for fingerprinting and exploiting Amazon cloud infrastructures." |
| CloudCopy | https://github.com/Static-Flow/CloudCopy | "implements a cloud version of the Shadow Copy attack against domain controllers running in AWS" |
| redboto | https://github.com/elitest/redboto/ | "collection of scripts that use the Amazon SDK for Python boto3 to perform red team operations against the AWS API." |

## Learn

### AWS Collections
| Link      | Description |
| ----------- | ----------- |
| https://cloudsecdocs.com/ by Marco Lancini (@lancinimarco) | "a website collecting technical notes, how-tos, and cheatsheets related to cloud-native technologies (not only security-focused)" | 
| https://www.practicalcloudsecurity.com/  | by Chris Farris (@jcfarris) "a website designed to help busy security practitioners navigate the intricacies of AWS’s Service Offerings" | 
| https://gist.github.com/kmcquade/33860a617e651104d243c324ddf7992a  | "AWS API calls that return credentials" | 
| https://rhinosecuritylabs.com/aws/aws-privilege-escalation-methods-mitigation/ |  | 
| https://gist.github.com/kmcquade/33860a617e651104d243c324ddf7992a | "AWS API calls that return credentials"|

### AWS CTFs and Labs

| Name      | Link      | Description |
| ----------- | ----------- | ----------- |
| CloudGoat | https://github.com/RhinoSecurityLabs/cloudgoat | "CloudGoat is Rhino Security Labs' "Vulnerable by Design" AWS deployment tool."| 
| SadCloud | https://github.com/nccgroup/sadcloud | "tool for spinning up insecure AWS infrastructure with Terraform." |
| Nimbostratus | https://github.com/andresriancho/nimbostratus-target | "This code deploys an Amazon AWS infrastructure which has various vulnerabilities and weak configuration settings which can be exploited using nimbostratus."| 
| Flaws | http://flaws.cloud/ | "Through a series of levels you'll learn about common mistakes and gotchas when using Amazon Web Services (AWS)" by Scott Piper (@0xdabbad00)| | 
| Flaws2 | http://flaws2.cloud/ |  "this game/tutorial teaches you AWS (Amazon Web Services) security concepts." by Scott Piper (@0xdabbad00)|

### Other great tools aggregators

https://github.com/toniblyx/my-arsenal-of-aws-security-tools

https://cloudberry.engineering/tool/

https://github.com/qazbnm456/awesome-web-security

https://github.com/yeyintminthuhtut/Awesome-Red-Teaming

# Microsoft Azure

| Category | Tools | Link | Description |
| ----------- | ----------- | ----------- | ----------- |
| Recon/Enum | ScoutSuite | https://github.com/nccgroup/ScoutSuite | "Scout Suite is an open source multi-cloud security-auditing tool, which enables security posture assessment of cloud environments. Using the APIs exposed by cloud providers, Scout Suite gathers configuration data for manual inspection and highlights risk areas. Rather than going through dozens of pages on the web consoles, Scout Suite presents a clear view of the attack surface automatically."|
| Recon/Enum | cloud_enum | https://github.com/initstring/cloud_enum | "Multi-cloud OSINT tool. Enumerate public resources in AWS, Azure, and Google Cloud."|
| Recon/Enum | MSOLSpray | https://github.com/dafthack/MSOLSpray | "A password spraying tool for Microsoft Online accounts (Azure/O365)."| 
| Recon/Enum | BlobHunter| https://github.com/cyberark/BlobHunter | "An opensource tool for scanning Azure blob storage accounts for publicly opened blobs."|
| Hunt | Sparrow | https://github.com/cisagov/Sparrow | "Sparrow helps network defenders detect possible compromised accounts and applications in Azure/Microsoft O365 environments." |
| Hunt | AzureAD Investigator | https://github.com/fireeye/Mandiant-Azure-AD-Investigator | "detecting artifacts that may be indicators of UNC2452 and other threat actor activity."|
| CSPM | SkyArk | https://github.com/cyberark/SkyArk/ | "SkyArk currently focuses on mitigating the new threat of Cloud Shadow Admins, and helps organizations to discover, assess and protect cloud privileged entities."|
| CSPM | CrowdStrike Reporting Tool | https://github.com/CrowdStrike/CRT | "This tool queries the following configurations in the Azure AD/O365 tenant which can shed light on hard to find permissions and configuration settings in order to assist organizations in securing these environments."|
| Exploit | MicroBurst | https://github.com/NetSPI/MicroBurst | "MicroBurst includes functions and scripts that support Azure Services discovery, weak configuration auditing, and post exploitation actions such as credential dumping." |
| CTF/Lab | CONVEX | https://github.com/azure/convex | "Cloud Open-source Network Vulnerability Exploitation eXperience (CONVEX) spins up Capture The Flag environments in your Azure tenant for participants to play through."|

# Google Cloud Platform
> I'm just getting started here. Stay tuned.

| Category | Tools | Link | Description |
| ----------- | ----------- | ----------- | ----------- |
| CTB/Lab | Thunder CTF | https://thunder-ctf.cloud/ | "Thunder CTF allows players to practice attacking vulnerable cloud projects on Google Cloud Platform (GCP)." |
