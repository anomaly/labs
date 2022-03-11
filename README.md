# Anomaly Labs
Working designs, documentation and references for all ideas at Anomaly labs.

## Infrastructure

<details>
<summary>Terraform reference implementation for Linode</summary>

The project aims to establish a standardised reference for using Terraform to provision and tear down infrastructure. 

The implementation will focus primarily on using Linode's infrastructure with the possibility of expanding to Amazon Web Services and Google Cloud Platform if the need arises.

Our key outcomes for this project are:
- Document our understanding of Terraform with key steps to bootstrap a project
- Document Linode related specifics around Terraform
- Create a Template project that developers can use to speed up their setup

[Visit project](projects/terraform-linode)

</details>

<details>
<summary>Containerised application deployment</summary>

Anomaly uses [Docker](https://docker.com) to develop and deploy all it's web applications. Deployment of the these applications has varied between client projects. This lab exercise aims to strongly define and provide a reference implementation that:

- Outlines a git based lifecycle of a deployment i.e test, quality assurance, and production
- Clearly define the architecture while being cost effective
- How envrionment variables are made available to various parts of the application
- Role of Github or a deployment facility
- Mechanism of storing and reteriving infrastructure level secrets

[Visit project](projects/docker-k8s)

</details>

<details>
<summary>Identity management for applications</summary>
</details>

## Workflow

<details>
<summary>CI/CD pipeline</summary>

[Visit project](projects/ci-cd)

</details>

# Web development

Developing for the web is a central part of Anomaly's offerings. The following projects explore and document core technologies and methods to ensure that our approach stays modern:

<details>
<summary>Server side architecture</summary>

[Visit project](projects/arch-server)

</details>

<details>
<summary>Web client side architecture</summary>

[ReactJS](https://reactjs.org) is our current Javascript development framework of choice. This plays to our strengths of being able to leverage it for building Single Page Applications (SPA) and use the same skill set to build static web sites using frameworks like [GatsbyJS](https://www.gatsbyjs.com) or [NextJS](https://nextjs.org).

The key outcomes of this project are:
- Establishing frameworks that are used along side React for network requests, API consumption, etc
- Outline the use of CSS frameworks like Tailwind CSS
- Fully inclusive interfaces with a strong focus on accessibility and internationalization
- Outline delivery of the application on object stores and content distribution networks
- Asset optimisation for single page applications

[Visit project](projects/arch-client)

</details>

## Mobile 

<details>
<summary>iOS project layout</summary>

[Visit project](projects/arch-ios)

</details>

## Other

<details>
<summary>Reading list</summary>
</details>



# License
Content of this repository are licensed under the Apache 2.0 license.