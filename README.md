
# quickstart-ec2-ipsec-mesh
## Opportunistic Amazon EC2 IPsec Mesh on the AWS Cloud

This Quick Start deploys an opportunistic Internet Protocol Security (IPsec) mesh that sets up dynamic IPsec tunnels between Amazon Elastic Compute Cloud (Amazon EC2) instances in your AWS Web Services (AWS) account. 

IPsec is a protocol for in-transit data protection between hosts. The manual configuration of site-to-site IPsec between multiple hosts can be an error-prone and intensive task, and the effort to keep the mesh parameters in sync can be significant. Using opportunistic IPsec, you can set up an IPsec mesh for a large number of hosts by using a simple and uniform configuration that does not need to change when you add or remove hosts.

The Quick Start sets up an environment that automates the configuration of opportunistic IPsec when EC2 instances are launched. It also generates instance certificates with weekly re-enrollment, sets up IPsec monitoring metrics in Amazon CloudWatch, and configures alarms and notifications through CloudWatch and Amazon Simple Notification Service (Amazon SNS).

The Quick Start is automated by an AWS CloudFormation template that sets up the opportunistic IPsec mesh environment in about 5 minutes. The implementation uses [Libreswan](https://libreswan.org/), an open-source implementation of IPsec encryption and Internet Key Exchange (IKE) version 2.

![Quick Start architecture for opportunistic IPsec mesh on AWS](https://d0.awsstatic.com/partner-network/QuickStart/datasheets/ipsec-mesh-on-aws-architecture.png)

For architectural details, best practices, step-by-step instructions, and customization options, see the 
[deployment guide](https://fwd.aws/8JmD7).

To post feedback, submit feature ideas, or report bugs, use the **Issues** section of this GitHub repo.
If you'd like to submit code for this Quick Start, please review the [AWS Quick Start Contributor's Kit](https://aws-quickstart.github.io/). 
