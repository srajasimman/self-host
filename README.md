![image](https://github.com/user-attachments/assets/030ec4cc-0a5a-43b2-b4e3-a210b76fb48f)

# Self-Hosting Boilerplate with Docker Compose
This repository provides a boilerplate for self-hosting various applications and services using Docker Compose. It includes a predefined `docker-compose.yml` file that simplifies the deployment of your services.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Services Included](#services-included)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

To get started with self-hosting your applications, follow these instructions.

### Prerequisites

- Docker installed on your machine. [Get Docker](https://docs.docker.com/get-docker/)
- Docker Compose installed. [Install Docker Compose](https://docs.docker.com/compose/install/)

## Usage

1. Clone this repository:

    ```sh
    git clone https://github.com/srajasimman/self-host.git
    cd self-host
    ```

2. Review and modify the `docker-compose.yml` file to suit your needs.

3. Start the services:

    ```sh
    docker-compose up -d
    ```

4. Check the status of your services:

    ```sh
    docker-compose ps
    ```

## Services Included

This boilerplate includes the following services:

### Reverse Proxy and Load Balancer

- **Traefik**: A dynamic reverse proxy and load balancer for managing routing of your applications.

### Homepage

- **Homepage**: A simple, customizable homepage for your self-hosted services.

### Development

-- **Gitea**: An all-in-one software development service

### CI/CD

- **Jenkins**: An automation server for building, testing, and deploying your code.

### Storage

- **MinIO**: A high-performance object storage server compatible with Amazon S3.
- **Registry**: A private Docker registry for storing and distributing your Docker images.

### Security and Analysis

- **Trivy**: A vulnerability scanner for Docker images, suitable for use in CI pipelines.
- **SonarQube**: A platform for continuous inspection of code quality to perform automatic reviews with static analysis of code.

### Databases

- **PostgreSQL**: A powerful, open-source object-relational database system.

### Monitoring and Alerts

- **Uptime Kuma**: A self-hosted monitoring tool like "Uptime Robot" to keep track of your services' availability.
- **Uptime Kuma API**: An API service for Uptime Kuma to facilitate integrations.
- **Prometheus**: A systems monitoring and alerting toolkit.
- **Alertmanager**: Handles alerts sent by client applications such as Prometheus and manages silencing, inhibition, and routing.
- **Grafana**: An analytics and monitoring platform to visualize data from various sources.
- **cAdvisor**: Provides container users an understanding of the resource usage and performance characteristics of their running containers.
- **Node Exporter**: An exporter for hardware and OS metrics exposed by *nix kernels for Prometheus monitoring.
- **Blackbox Exporter**: A probe-based exporter that allows blackbox probing of endpoints over HTTP, HTTPS, DNS, TCP, ICMP, and gRPC.

### Email Testing

- **MailHog**: An email testing tool for developers to view and debug email interactions.

## Configuration

You can configure each service by modifying the respective section in the `docker-compose.yml` file. Here are some common configurations:

- **Ports**: Ensure that the ports defined in the `docker-compose.yml` file do not conflict with other services running on your host machine.
- **Volumes**: Map your host directories to container directories as needed to persist data.
- **Environment Variables**: Set environment variables for each service to customize their behavior.

## Contributing

We welcome contributions! If you have suggestions for improvements or want to add more services, please create a pull request or open an issue.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Happy self-hosting!
