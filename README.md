AWS Migration Case Study. 
Security Pillar Recommendations
-
This project presents a cloud migration proof‑of‑concept for Bean & Bytes, focusing on secure,
scalable, and highly available AWS architecture. It includes a multi‑AZ VPC design, identity controls,
monitoring, and Security Pillar improvements based on the AWS Well‑Architected Framework.

Overview
-
The solution demonstrates how Bean & Bytes can migrate to AWS using a layered security model 
and best practices for protecting data, systems, and workloads. The architecture includes 
public and private subnets, EC2 instances in an Auto Scaling group, RDS primary/secondary 
databases, S3 static hosting, and IAM‑based access control.

Architecture Highlights
-
Multi‑AZ VPC with public and private subnets;
EC2 instances behind an Elastic Load Balancer;
Auto Scaling group for high availability;
RDS primary and secondary for failover;
NAT gateways for secure outbound traffic;
Internet gateway for controlled public access;
Route 53 for DNS;
S3 static website hosting;
CloudWatch monitoring and alarms;
IAM roles and policies for admin and user access;
Network ACLs and Security Groups for layered protection;

Key Security Considerations
-
Multi‑layered protection across network, compute, and database layers;
Network ACLs controlling subnet‑level traffic;
Security Groups restricting instance‑level access;
IAM policies enforcing least privilege;
Separation of public and private subnets;

Security Pillar Recommendations
-
Implement a Strong Identity Foundation;
Use IAM roles instead of long‑term credentials;
Enforce MFA for administrators;
Apply least‑privilege access across all roles;

Maintain Traceability
-
Enable AWS CloudTrail for full API logging;
Use CloudWatch for metrics, alarms, and operational visibility;

Prepare for Security Events
-
Create an incident management and investigation policy;
Run incident response simulations;
Ensure logging and monitoring support rapid detection and recovery;

Conclusion
-
The Bean & Bytes cloud solution already incorporates strong security measures such as private subnets, 
IAM policies, and multi‑layered network protection. By strengthening identity controls, improving 
monitoring, and preparing for security events, the company can maintain a secure, resilient, and 
compliant cloud environment as it scales.

Reference
-
AWS Well‑Architected Framework – Security Pillar
https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/welcome.html 
