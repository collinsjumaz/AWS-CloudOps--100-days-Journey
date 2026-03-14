# Day 03 – March 14, 2026 – AWS Networking & Delivery Services

## Skills Learned:
- Reviewed Amazon VPC fundamentals: CIDR ranges, subnets, route tables, and gateways (IGW, VGW, VPC Peering, VPC Endpoints/PrivateLink).
- Understood the need to add gateways/endpoints to allow access to the internet, on-prem, or other VPCs.
- Covered AWS networking/delivery services for traffic optimization and availability (ELB, Route 53, Global Accelerator, CloudFront).
- Explored hybrid connectivity and service networking patterns (PrivateLink, VPN, Direct Connect, Transit Gateway, API Gateway, App Mesh, Cloud Map).

## Labs/Exercises Completed:
- N/A (concept review and note capture)

## Key Takeaways:
- A VPC starts fully private; you must intentionally add gateways or endpoints to connect out.
- ELB (ALB/NLB/GWLB/CLB) is essential for high availability and scaling traffic across targets.
- Route 53 routing policies and Global Accelerator can optimize global traffic flow.
- PrivateLink and VPN/Direct Connect keep traffic on private networks and support hybrid cloud connectivity.
- Transit Gateway is the go‑to for managing complex multi-VPC and hybrid connectivity.

## Notes:
- Next: Experiment with creating a VPC with both public and private subnets, and attach an IGW plus a NAT Gateway.
- Consider labbing a Transit Gateway design for multi-VPC architectures.
