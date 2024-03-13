# Kubernetes YAML Configuration Templates

This repository contains Kubernetes YAML configuration templates for deploying an NGINX server and a CRUD Node.js application, along with associated ConfigMaps and Secrets.

## Prerequisites

Before using these YAML configuration files, ensure you have the following prerequisites installed and configured:

- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/): The Kubernetes command-line tool for managing Kubernetes clusters.
- Access to a Kubernetes cluster: Ensure you have access to a Kubernetes cluster where you intend to deploy these resources.

## Directory Structure

The repository is organized as follows:

- `nginx/`: Contains YAML files for deploying an NGINX server.
- `crud-node/`: Contains YAML files for deploying a CRUD Node.js application.

## Usage

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/your-username/kubernetes-yaml-templates.git
    ```

2. Navigate to the directory containing the YAML files relevant to your deployment.

3. Modify the configuration files as needed to match your application's requirements. You may need to update image names, environment variables, resource requests, etc.

4. Apply the configuration to your Kubernetes cluster using `kubectl apply -f filename.yaml`. For example:

    ```bash
    kubectl apply -f nginx/deployment.yaml
    ```

    ```bash
    kubectl apply -f crud-node/deployment.yaml
    ```

5. Verify that the resources have been created successfully:

    ```bash
    kubectl get pods
    ```

## Contributing

Contributions are welcome! If you have improvements or additional Kubernetes YAML configuration templates to share, feel free to submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
