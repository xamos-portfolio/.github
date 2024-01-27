# What is this?

Welcome to [IkenoXamos](https://github.com/IkenoXamos)'s Personal Portfolio Project. The goal of this project is to create a portfolio that can showcase personal projects that I have worked on and to demonstrate my skills.
Rather than creating a simple portfolio, I decided that the portfolio itself is a great opportunity to showcase the knowledge I have developed over the years.

As such, this project will involve the creation of a platform to host future personal/hobby projects. The first project will be to host the portfolio website itself, which will be a relatively simple static website showing what I've built and how they were created.

Feel free to browse the [repositories](https://github.com/orgs/xamos-portfolio/repositories?type=source) to see how it is being built.

If you have any suggestions for how I might improve the project or questions about any of the decisions I made, feel free to create an issue!

## Technologies Used

### Google Cloud Platform

Over the last several years I have discovered that I quite enjoy Kubernetes, so this will be the primary means by which I will host my projects. Specifically, I will be using Managed Kubernetes on GCP, [Google Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine).
It is a convenient choice for working with Kubernetes for hobby projects, as they have a nice [free tier offering](https://cloud.google.com/kubernetes-engine/pricing#cluster_management_fee_and_free_tier).

> The cluster management fee of $0.10 per cluster per hour (charged in 1 second increments) applies to all GKE clusters irrespective of the mode of operation, cluster size or topology.
>
> The GKE free tier provides $74.40 in monthly credits per billing account that are applied to zonal and Autopilot clusters. If you only use a single Zonal or Autopilot cluster, this credit will at least cover the complete cost of that cluster each month.

This allows me to use a Managed Kubernetes Service without paying large costs for the management fee. Azure offers the same free tier for Kubernetes as Google, but AWS does not. I decided to proceed with Google.

Once I chose Google for their Managed Kubernetes Service, it was an easy choice to continue to use GCP for the rest of the project.

### Terraform/OpenTofu

I also decided that it would be fun to follow Infrastructure as Code to build out all of the resources needed for the project using [Terraform](https://www.terraform.io/).
However, I recently discovered [OpenTofu](https://opentofu.org/), an open-source fork of Terraform. At the moment their features are about identical, but I decided it would be a fun experience to leverage an emerging community-fork of a well-known tool.
