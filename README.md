
# GitOps Manifests Repository

## Overview
This repository contains Kubernetes manifests and Helm charts for deploying the Weather App.

## Related Repositories

- [Weather App EKS Terraform](https://github.com/eilaytal/weather-app-eks-terraform): Terraform configuration for deploying the Weather App on AWS EKS.
- [Jenkins Pipeline](https://github.com/eilaytal/jenkins_pipeline): Jenkins pipeline for automating CI/CD processes for the Weather App.
- [Weather App](https://github.com/eilaytal/weather-app): The main repository containing the Weather App source code.

## Directory Structure

### `weatherapp_chart/`
This directory contains Helm charts for deploying the Weather App.

#### Files:
- **Chart.yaml**: Helm chart metadata.
- **values.yaml**: Default configuration values for the Helm chart.
- **blue-configmap.yaml**: Configuration map for the blue environment.
- **green-configmap.yaml**: Configuration map for the green environment.
- **ingress.yaml**: Ingress configuration for accessing the Weather App.

### `templates/`
This directory contains Kubernetes manifest templates for deploying the Weather App.

#### Files:
- **weather-deployment.yaml**: Deployment configuration for the Weather App.
- **weather-service.yaml**: Service configuration for the Weather App.
- **.helmignore**: Specifies files to be ignored by Helm.

## Usage
1. Apply manifests using `kubectl` or Helm.
2. Monitor deployments in the Kubernetes cluster.

## Contributing
Feel free to contribute by submitting pull requests or raising issues in the repository.
