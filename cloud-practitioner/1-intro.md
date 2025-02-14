
# Intro To Cloud On AWS

## 1. Hierarchy in AWS

_The way AWS is laid out..._

### Availability Zones, Regions, Local Zones, Edge

* A region is a collection of AZ's
* An AZ is within a region
* Some regions have ~3 AZ's, some have more
* LZ-s - extensions of an AWS Region
* Edge locations (CloudFront CDN uses these)

// TODO: 👷‍♀ Is an edge within an AZ or just a region?

### 3 Reasons For Choosing a Region

1. Latency to the user — You need to be located closer to the user.
1. Data laws — You have legal requirements that means you need to be in a given region.

// TODO: 👷‍♀ What's the third reason!?

---

## 2. Cloud Concepts

### Cloud Computing Models

* IAAS (VPC,EC2,EBS)
* PAAS (RDS,EMR,ElasticSearch)
* SAAS (web-based email, Office 354, Salesforce)
* FAAS (Amazon Simple Storage Service - S3, AWS Lambda, DynamDB, SNS) - build and run applications without thinking about servers

### 3 Types of Cloud

* Public: AWS, Azure, GCP
* Hybrid: Mixture of public and private
* Private Cloud: Your datacenter

---

## 3. Business case for AWS

### 6 Advantages Of Cloud

* Trade capital expense for variable expense
* Economies of scale
* Stop guessing about capacity (on demand)
* Increase speed and agility
* Stop spending money running data centers
* Global in minutes

### 4 Key Values for Building a Migration Business Case

* Cost Saving - free up budget for investment elswhere
* Staff Productivity - Teams can work on higher value activities
* Operational Resilience - Increased reliability, availability and security
* Busine Agility - Increased innovation and reduced time to market

---

## 4. Best practices

### Migration best practices

* Get stakeholders and senior leaders aligned
* Set top-down quantifiable goals (focused, not organic)
* Trust the process - Assess -> Mobilize -> migrate & Modernize
* Chose the right migration pattern (7Rs)
  * Retire
  * Retain
  * Relocate (eg. VMWare, Hyper-V)
  * Rehost (lift & shift)
  * Repurchase
  * Re-platform
  * Refactor

---

### Cloud Architecture Design Principles

* design for failure (multi-AZ, multi-region)
* elasticity (autoscaling)
* elastic load balancer -> enables fault tolerance
* Loose Coupling (SQS)
* AWS well-architected framework design principles
  * Stop guessing capacity needs
  * Test systems at production scale
  * automat to make architectural experimentation easier
  * allow for evolutionary architectures
  * drive architectures using data
  * improve through game days

(effort increases from top to bottom)

> Example of this design:
 > Elastic Beanstalk
> automtically handles capacity provisioning, load balancing, scaling and application health monitoring

Deployment options

* All at once
* Rolling (a batch at a time)
* Immutable (two environments temporarily)
* Blue/Green (two environments)
