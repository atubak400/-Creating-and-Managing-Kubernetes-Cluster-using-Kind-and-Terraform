# Creating and Managing Kubernetes Cluster using Kind and Terraform

![](./img/)

This project is all about making a Kubernetes cluster using Kind and Terraform. With Kind, a tool that helps set up Kubernetes clusters using Docker, we create a local space for development and testing. Then, we use Terraform, a handy tool for coding infrastructure, to define and handle the Kubernetes bits in the cluster. This combo of Kind and Terraform makes it easy to set up, configure, and manage Kubernetes clusters. It's a smooth way for both developers and admins to handle the nitty-gritty of creating and organizing Kubernetes setups. Join us in exploring how Kind and Terraform team up to simplify the whole process!

Install Kind and download Docker Desktop

Run brew install kind on your terminal

Launch and sign in to your Docker Desktop

Create kind-config.yaml file

code kind-config.yaml

Created a local Kubernetes cluster named "terraform-kubernetes-demo" using a custom configuration file:
kind create cluster --config kind-config.yaml --name terraform-kubernetes-demo

Verified the list of Kind clusters:
kind get clusters

Checked the cluster information using kubectl:
kubectl cluster-info --context kind-terraform-kubernetes-demo

Listed the files in the current directory:
ls

Create the Terraform configuration file in Visual Studio Code:
code kubernetes.tf

Viewed the Kubernetes configuration for the Kind cluster:
kubectl config view --minify --flatten --context=kind-terraform-kubernetes-demo

Created a Terraform variables file (terraform.tfvars):
code terraform.tfvars

Listed the files in the current directory again:
ls

Formatted the Terraform configuration:
terraform fmt

Initialized the Terraform configuration:
terraform init


I have set up a local Kubernetes cluster using Kind, configured it with Terraform, and initialized Terraform for managing Kubernetes resources# -Creating-and-Managing-Kubernetes-Cluster-using-Kind-and-Terraform
