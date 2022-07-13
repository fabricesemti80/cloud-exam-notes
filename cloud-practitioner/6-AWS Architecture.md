# Architecture principles

## Highly Available and fault tolerant

 Elastic Beanstalk

- automtically handles capacity provisioning, load balancing, scaling and application health monitoring

Principles

- VPC spawns multiple AZ-s
- EC2 instances in AutoScaling groups --> enables elasticity
- uses Elastic Load Balancer --> fault tolerance

Deployment options

- All at once
- Rolling (a batch at a time)
- Immutable (two environments temporarily)
- Blue/Green (two environments)
