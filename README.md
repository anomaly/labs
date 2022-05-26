# Anomaly Labs
Working designs, documentation and references for all ideas at Anomaly labs. The general philosophy behind each one of these projects is to increase communication between developers and designers and reduce the need for synchronous communication.

Anomaly desires to pursue multiple products, streamlining the development process will be a vital to the success of the projects.

# Infrastructure

Our approach roughly is to use:
- Docker and Docker Hub to manage to publish images of our containers
- Terraform to provision the components we require e.g Kubernetes Cluster, Managed database, networking rules, DNS. Use Terraform Cloud for managing the state of the infrastructure.
- Helm to deploy Charts in cluster itself e.g Redis, Postgres (until Linode has a managed solution), and our application.
- Use Kubernetes to scale replicas up and down as we need them (this should be automated into the future).

Previously the team's approach was to keep application and deployment sources in the same repository. A central theme of these repositories is to decouple the application from deployment, providing the most amount of flexibility.

## Terraform reference implementation for Linode

The project aims to establish a standardised reference for using Terraform to provision and tear down infrastructure. 

The implementation will focus primarily on using Linode's infrastructure with the possibility of expanding to Amazon Web Services and Google Cloud Platform if the need arises.

Our key outcomes for this project are:
- Document our understanding of Terraform with key steps to bootstrap a project
- Document Linode related specifics around Terraform
- Create a Template project that developers can use to speed up their setup

[Visit project](projects/terraform-linode)
 
## Helm reference usage

The project aims to establish an understanding of deploying applications with Helm and best practices around secrets management.

Our aim will be to deploy various components like Redis, Postgres, and our application. As Linode brings up managed services we will move components out of the cluster.

## Containerised application deployment

Anomaly uses [Docker](https://docker.com) to develop and deploy all it's web applications. Deployment of the these applications has varied between client projects. This lab exercise aims to strongly define and provide a reference implementation that:

- Outlines a git based lifecycle of a deployment i.e test, quality assurance, and production
- Clearly define the architecture while being cost effective
- How envrionment variables are made available to various parts of the application
- Role of Github or a deployment facility
- Mechanism of storing and reteriving infrastructure level secrets

[Visit project](projects/docker-k8s)

## Identity management for applications

TBA

# Workflow

## CI/CD pipeline

[Visit project](projects/ci-cd)

# Web development

Developing for the web is a central part of Anomaly's offerings. The following projects explore and document core technologies and methods to ensure that our approach stays modern:

## Server side architecture

[Visit project](projects/arch-server)

## Web client side architecture

[ReactJS](https://reactjs.org) is our current Javascript development framework of choice. This plays to our strengths of being able to leverage it for building Single Page Applications (SPA) and use the same skill set to build static web sites using frameworks like [GatsbyJS](https://www.gatsbyjs.com) or [NextJS](https://nextjs.org).

The key outcomes of this project are:
- Establishing frameworks that are used along side React for network requests, API consumption, etc
- Outline the use of CSS frameworks like Tailwind CSS
- Fully inclusive interfaces with a strong focus on accessibility and internationalization
- Outline delivery of the application on object stores and content distribution networks
- Asset optimisation for single page applications

[Visit project](projects/arch-client)


# Mobile 

## iOS project layout

[Visit project](projects/arch-ios)

## Other

## Reading list



# License
Content of this repository are licensed under the Apache 2.0 license.