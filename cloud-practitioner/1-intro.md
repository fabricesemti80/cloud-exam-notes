
# Intro To Cloud On AWS

## 1. Hierarchy in AWS

_The way AWS is laid out..._

### Availability Zones, Regions, Edge

* A region is a collection of AZ's
* An AZ is within a region
* Some regions have ~3 AZ's, some have more
* Edge locations

// TODO: 👷‍♀ Is an edge within an AZ or just a region?

#### 3 Reasons For Choosing a Region

1. Latency to the user — You need to be located closer to the user.
1. Data laws — You have legal requirements that means you need to be in a given region.

// TODO: 👷‍♀ What's the third reason!?

---
## Cloud Concepts

### 3 Types of Cloud Computing

* IAAS
* PAAS
* SAAS

### 3 Types of Cloud

* Public: AWS, Azure, GCP
* Hybrid: Mixture of public and private
* Private Cloud: Your datacenter

---

## Business case for AWS

### 6 Advantages Of Cloud

* Trade capital expense for variable expense
* Economies of scale
* Stop guessing about capacity (on demand)
* Increase speed and agility
* Stop spending money running data centers
* Global in minutes

#### 4 Key Values for Building a Migration Business Case

* Cost Saving - free up budget for investment elswhere
* Staff Productivity - Teams can work on higher value activities
* Operational Resilience - Increased reliability, availability and security
* Busine Agility - Increased innovation and reduced time to market

---

## Migration best practices

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

## Cloud Architecture Design Principles

* design for failure (multi-AZ, multi-region)
* elasticity (autoscaling)
* Loose Coupling (SQS)
* AWS well-architected framework design principles
  * Stop guessing capacity needs
  * Test systems at production scale
  * automat to make architectural experimentation easier
  * allow for evolutionary architectures
  * drive architectures using data
  * improva through game days

(effort increases from top to bottom)
