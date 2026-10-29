# Lab Notes and Submission Details

## Goal
Create two VPCs and establish private connectivity through VPC peering while using a Bastion host for SSH access to private instances.

## CIDR plan
- VPC A: `10.10.0.0/16`
  - Public subnet: `10.10.1.0/24`
  - Private subnet: `10.10.2.0/24`
- VPC B: `10.20.0.0/16`
  - Private subnet: `10.20.1.0/24`

## Route tables
Refer to the route table matrix in the repository README and the route-table screenshots in `evidence/`.

## Security groups
See the README for the inbound rule intent and the `09a`, `09b`, and `09c` screenshots for the captured rules.

## Tests
The report records bidirectional ICMP tests, SSH through the Bastion, a controlled failure by removing an inbound ICMP rule, and successful recovery after restoring it.

## Important evidence limitation
The pre-peering baseline test was not captured. Do not describe the controlled security-group failure as a pre-peering baseline.

## Cleanup status
The lab resources were removed after the report and screenshots were saved. This repository documents the completed lab and does not represent a currently deployed environment.
