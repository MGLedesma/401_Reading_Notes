# Compute Abstraction on AWS

Resource: [Compute Abstractions on AWS: A Visual Story](https://aws.amazon.com/blogs/architecture/compute-abstractions-on-aws-a-visual-story/)

## The different abstraction levels

- Computing can take place at different layers of abstraction
- AWS provides a multitude of services that compute at different abstraction layers
- The layers can be defined like so:
- Virtual Machine/Instance Abstraction
- The very first abstraction on AWS, introduced in 2006 (EC2)
- User retains responsibility of guest OS, applicationsd, middleware, and their lifecycles
- Exists at the edge between user and provider
- Container Abstraction
- Containers virtualize an OS to allow separated applications with different/incompatible software dependencies to run
- Modern container-solutions typically implemented in two logical pieces:
- Control Plane: exposes API and interfaces to define, deploy, and lifecycle containers, AKA container orchestration layer.
- Data Plane: responsible for providing hardware capacity, connects to a network.
- Amazon released ECS as a solution to free customers from having to manage control planes.
- Function Abstraction
- Allows a customer to run a single function, rather than an entire OS instance to run code (AWS Lambda)
- Bare Metal Abstraction
- Amazon EC2 bare metal, essentially gives users direct access to hardware
- Full Container Abstraction
- An option presented by AWS Fargate to turn the Data Plane into a managed service

