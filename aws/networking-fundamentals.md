# Networking Fundamentals

Every AWS account comes with a RFC1918 specified IP range, which is private and is guranteed to not conflict with anything on the internet.
Some of these are

- 10.0.0.0/8
- 172.16.0.0/12
- 192.168.0.0/16

AWS recommends `/16` as it can have upto `65,536` addresses.

## Security Group

- operates at instance level
- supports allow rules only
- is steful - return traffic is automatically allowed regardless of any rules
- all rules evaluated before deciding whether to allow traffic
- applies only to instances explicitey associated with security group

## Network ACL

- operates at subnet level
- supports allow and deny rules
- is stateless - return traffic must be explicitely allowed by rules
- rules evaluated in order when deciding whether to allow traffic
- automatically applies to all instances launched into associated subnet 