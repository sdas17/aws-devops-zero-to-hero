# Day 1 — Cloud Computing: Agenda & Notes

## Agenda
- What is cloud?
- Public vs Private Cloud
- Why is public cloud so popular?
- Why AWS?
- Trends: Are people moving back to private cloud?
- Create an AWS account

---

## 1. What is cloud?
Cloud computing means delivering computing services—servers, storage, databases, networking, software, analytics, intelligence—over the internet ("the cloud"). Instead of owning physical hardware, organizations rent resources from cloud providers and pay for what they use.

Key characteristics:
- On-demand self-service
- Broad network access
- Resource pooling (multi-tenancy)
- Rapid elasticity / scalability
- Measured service (pay-as-you-go)

Short description for class: the cloud is basically using remote servers hosted on the internet to store, manage, and process data, rather than local servers or personal computers.


## 2. Public vs Private Cloud
- Public cloud: Services offered over the public internet and available to anyone who wants to purchase them. Examples: AWS, Azure, GCP.
  - Pros: low upfront cost, virtually unlimited scalability, managed services, broad global footprint.
  - Cons: shared infrastructure (multi-tenant), less direct control over hardware, potential data residency/compliance concerns.

- Private cloud: Cloud infrastructure operated solely for a single organization (on-premises or hosted). Can be managed by the organization or by a third-party.
  - Pros: more control, better isolation and security for sensitive workloads, easier compliance.
  - Cons: higher cost, requires expertise to manage, capacity planning required.

- Hybrid cloud: A mix of public and private—useful for workloads that need both on-premises control and cloud scalability.


## 3. Why is public cloud so popular?
- Cost model: pay-as-you-go removes large capital expenses.
- Speed & agility: teams can provision resources in minutes instead of weeks.
- Managed services: databases, ML, analytics, and other services reduce operational burden.
- Global presence: run workloads close to users worldwide.
- Strong ecosystem, community, and partner networks.


## 4. Why AWS?
- Market leader with the largest global footprint and broadest service catalog.
- Mature tooling and enterprise support.
- Large ecosystem of partners, certifications, and community resources.
- Many companies started with AWS early — lots of documentation and real-world patterns.


## 5. Trends: moving back to private cloud?
- Some organizations adopted hybrid or multi-cloud strategies to avoid vendor lock-in and address regulatory/compliance needs.
- Reasons to move workloads back on-prem or to private cloud include data residency, latency, cost optimization for steady-state workloads, and control/security.
- However, most net-new development tends to favor public cloud for agility and managed services.


## 6. Create an AWS account (class demo steps)
1. Go to https://aws.amazon.com and click "Create an AWS Account".
2. Provide email, choose account type (root vs IAM later), add contact information.
3. Add payment method (credit card required for verification).
4. Choose support plan (Basic is free).
5. Verify identity (phone/SMS).
6. Sign in to the AWS Management Console and create an IAM user for day-to-day tasks (do not use the root account).

Demo commands / tips:
- After creating an IAM user with AdministratorAccess, install and configure the AWS CLI:

```powershell
# Install (Windows, using MSI installer) - show link instead of automatic install
# Configure
aws configure
# enter Access Key ID, Secret Access Key, region (e.g., us-east-1), output (json)
```

- Verify CLI access:
```powershell
aws sts get-caller-identity
```


## Quick Summary
Public cloud provides fast, scalable, and cost-effective infrastructure and managed services. AWS is widely used because of its maturity and breadth of services. Private cloud still matters for specific compliance/security requirements and some stable workloads.


## Action items / TODOs
- [ ] Instructor: prepare a live demo of creating an IAM user and configuring AWS CLI
- [ ] Students: create AWS account before next session (or bring laptop to create together)
- [ ] Class: decide which regions we'll use for demos (recommend: us-east-1)


## References & further reading
- AWS official site: https://aws.amazon.com/
- NIST Cloud Computing Definition: https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf
- Articles on public vs private cloud and hybrid architectures


---
Notes created from the day's short agenda. Adjust or tell me where to save or how you'd like this shortened/expanded.
