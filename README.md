# Udemy Docker Mastery

This repository is a comprehensive guide for the **Docker Mastery** course, offering resources, examples, and references to help you master Docker, Swarm, and Kubernetes. The course is designed and instructed by **Bret Fisher**, a Docker Captain, and covers key concepts and practices essential for modern containerized development and operations.


Course: [Docker Mastery: with Kubernetes + Swarm from a Docker Captain](https://www.udemy.com/course/docker-mastery/?srsltid=AfmBOor5iCrk2nKE69Dp1p0YtiABIislVUpoBD0MhLxnDB-wMqQPEYXw&couponCode=LETSLEARNNOW)

Instructor: Bret Fisher

## Course Overview
This course covers the following topics:

- Fundamentals of Docker, containers, and orchestration
- Setting up Docker on different operating systems (Windows, macOS, Linux)
- Building, tagging, and pushing Docker container images
- Managing persistent data with volumes and bind mounts
- Simplifying multi-container workflows using Docker Compose
- Using Docker Swarm and Kubernetes for orchestration and deployment


## Table of Contents

### Section 1: Course Introduction and Docker Introduction

In this opening section, we'll lay the groundwork for your learning journey by introducing Docker and its importance in today's tech ecosystem. You’ll understand how Docker fits into modern development practices and why mastering it is crucial. Along the way, you'll gain access to key resources, join a vibrant community of over 21,000 students, and get answers to frequently asked questions. We’ll also cover the latest Docker updates to keep you on the cutting edge of this essential skill.

### Section 2: The Best Way to Setup Docker for Your OS

In this section, we'll walk you through the process of setting up Docker on different operating systems to ensure a smooth start to your course. You’ll learn about the various Docker editions and which one is best suited for your needs. We’ll cover fast and efficient installation methods for Docker on Windows, Mac, and Linux, providing you with helpful tips for both desktop and server setups. You’ll also get introduced to VS Code, a powerful tool for DevOps, Docker, and YAML editing, and explore the latest updates to Docker versions and products to keep you up to date with new developments.

### Section 3: Creating and Using Containers

In this section, we’ll dive into the core concepts of working with Docker containers. You’ll learn how containers function and how to monitor their processes via the command-line interface (CLI). We’ll show you how to access the shell inside containers, allowing you to interact with them directly. Through practical examples, you’ll become familiar with commands like docker container run -it to start containers interactively and docker container exec -it to execute commands within running containers.

We’ll also explore Docker Networks, covering both private and public communication between containers. You’ll understand how Docker’s default network settings work and how it provides the flexibility of a “batteries included, but removable” approach. To solidify your understanding, we’ll walk through an exercise on running containers with port mapping, followed by an in-depth look at how Docker handles traffic flows and firewall settings to manage packets in and out of containers.

### Section 4: Container Images

In this section, we’ll explore everything you need to know about Docker images. You’ll start by understanding what an image is and what it isn’t, followed by an introduction to Docker Hub, where you’ll find a vast repository of pre-built images. We’ll delve into the concept of image layers, demonstrating how Docker uses these layers to optimize storage and performance. You’ll also learn how to visualize and manage these layers, and create custom images tailored to your needs.

Next, we’ll guide you through essential commands like docker history and docker image inspect to gain deeper insights into the structure and history of images. You’ll also get a clear understanding of image tagging and how to push your images to Docker Hub. Finally, we’ll cover how to build your own images from scratch, including the basics of Dockerfiles, running Docker builds, and extending official images to create more complex containers.

### Section 5: Container Lifetime & Persistent Data: Volumes, Volumes, Volumes

In this section, we’ll dive into the concept of container lifecycle management and persistent data handling in Docker. You’ll learn how containers are ephemeral by nature and how Docker provides tools to manage persistent data beyond the container's life. We’ll start with an introduction to data volumes, explaining their importance for storing and retaining data even when containers are stopped or removed.

You’ll then explore named volumes, which offer a user-friendly way to assign volumes to containers, followed by the `docker volume create` command to create volumes manually. We’ll also cover shell differences for path expansion and dive into bind mounting as a method of linking files from your host system to containers, giving you even greater control over your data.

To solidify your understanding, we’ll walk you through assignments like upgrading databases using named volumes and editing code running in containers with bind mounts. Lastly, we'll discuss managing sensitive data such as database passwords within containers, ensuring that your application is secure and efficient.

### Section 6: Making It Easier with Docker Compose: The Multi-Container Tool

In this section, we’ll explore how Docker Compose simplifies working with multiple containers. You’ll begin by understanding the `docker-compose.yml` file, which allows you to define and manage multi-container applications with ease. We’ll cover how to use Docker Compose to handle persistent data, including data volumes and named volumes, and how these tools work together to ensure data is preserved even when containers are recreated.

You’ll learn about creating volumes with `docker volume create`, as well as shell differences for path expansion and bind mounting to link files from your host to containers. We’ll also guide you through assignments such as upgrading databases with named volumes and editing code running inside containers with bind mounts.

As you advance, we’ll show you how to build Compose files for multi-container services and extend them to handle image building within Compose configurations. You’ll also tackle assignments focused on run-time image building and testing multi-container setups, preparing you to fully leverage Docker Compose in real-world applications.

### Section 7: Swarm Intro and Creating a 3-Node Swarm Cluster

In this section, we’ll introduce Docker Swarm and its orchestration capabilities, helping you understand how to manage containerized applications at scale. We’ll start by exploring Swarm Mode, which offers built-in orchestration for Docker clusters, and discuss the new challenges containers present when running across multiple nodes.

You’ll then create your first service and scale it locally to see how Swarm handles service management. We’ll also dive into the `docker swarm init` command to explain what happens when you initialize a Swarm and how it sets up the cluster. We’ll cover UI changes related to service creation and updates, as well as a known Docker Machine bug that may affect your Swarm setup.

Finally, we’ll guide you through the process of creating a 3-node Swarm cluster, giving you the hands-on experience needed to manage and scale Dockerized applications across multiple nodes.

### Section 8: Swarm Basic Features and How to Use Them in Your Workflow

In this section, we’ll explore the basic features of Docker Swarm and how to integrate them into your workflow. We’ll start by scaling out with overlay networking, which allows for multi-host networking and the expansion of your virtual network. You’ll learn how the routing mesh in Swarm works, acting as a global traffic router to direct requests to the appropriate service.

Next, we’ll guide you through an assignment where you’ll create a multi-service, multi-node web application, putting your skills to the test. We’ll also cover Swarm stacks and how to leverage Docker Compose to define and deploy production-grade services in Swarm.

Security is key, so we’ll dive into secrets storage in Swarm, explaining how to protect your environment variables and use secrets within Swarm services and stacks. To help you gain hands-on experience, we’ll walk you through an assignment on creating a stack with secrets and deploying it securely.

### Section 9: Swarm App Lifecycle

In this section, we’ll look at the complete application lifecycle within Swarm, from development to deployment. You’ll learn how to use secrets with local Docker Compose for local “simulated” secrets before moving on to managing the full application lifecycle with Compose, making it easy to build and deploy applications seamlessly.

We’ll cover how to perform service updates, ensuring you can make changes to your services without downtime, and dive into Swarm app lifecycle best practices. You’ll also explore healthchecks in Dockerfiles and how they contribute to maintaining the health of your Swarm-based applications.

### Section 10: Container Registries: Image Storage and Distribution

In this section, we’ll explore container registries and how Docker images are stored and distributed. You’ll gain a deeper understanding of Docker Hub, its auto-build features, and how to use Docker registry in various environments. We’ll also guide you through running a private Docker registry locally, securing it with TLS and authentication.

You’ll learn how to integrate Docker registries with Swarm for image distribution in a multi-node setup, and explore the use of third-party image registries for added flexibility.

### Section 11: Docker in Production

In this section, we’ll dive into the challenges and best practices for running Docker and Swarm in production environments. You’ll learn about Dockerfile optimization, anti-patterns to avoid, and how to ensure your containers are production-ready. We’ll cover architecture decisions like choosing between container-on-VM or container-on-bare-metal and discuss the importance of selecting the right OS and base distribution for your containers.

You’ll also learn about Docker Swarm architectures, from single-node setups to large-scale Swarm clusters with 100+ nodes, and the considerations for scaling your applications effectively.

### Section 12: The What and Why of Kubernetes

In this section, we’ll introduce you to Kubernetes, a leading container orchestration platform. You’ll learn what Kubernetes is, why it might be the right solution for your needs, and how it compares to Docker Swarm. We’ll go over the advantages and disadvantages of both orchestrators, helping you decide which is the best fit for your containerized applications.

### Section 13: Kubernetes Install and Your First Pods

In this section, we’ll guide you through the installation of Kubernetes and setting up your first Pods. You’ll start by understanding Kubernetes architecture and terminology, with a focus on the system components that make up a cluster. From there, we’ll help you set up Kubernetes locally using different tools like Docker Desktop, Minikube, and MicroK8s, providing you with tips for a smooth installation.

You’ll dive into Kubernetes container abstractions such as Pods and controllers, and learn how to use `kubectl` to manage them. You’ll create your first Pod with `kubectl run` and explore the changes introduced in Kubernetes 1.18. We’ll also cover scaling ReplicaSets and inspecting Kubernetes objects to monitor and manage your applications effectively.

### Section 14: Exposing Kubernetes Ports

In this section, we’ll explore how to expose your Kubernetes services to the outside world. You’ll start by understanding the four primary service types: ClusterIP, NodePort, LoadBalancer, and ExternalName. We’ll walk you through creating a `ClusterIP` service to expose your deployments and how to inspect the service for proper configuration.

You’ll also learn how to create `NodePort` and `LoadBalancer` services to make your applications accessible externally. We’ll touch on the basics of Kubernetes DNS, including how CoreDNS works to manage service discovery and resolve service names.

### Section 15: Kubernetes Management Techniques

This section focuses on various management techniques for Kubernetes. You’ll begin by exploring how to use `kubectl` generators to run, expose, and create resources quickly. We’ll cover the evolution of the `kubectl run` command and its future role in Kubernetes.

You’ll also dive into the difference between imperative and declarative approaches in Kubernetes, understanding how both styles fit into software development. Lastly, we’ll look at three different management approaches for Kubernetes, helping you choose the right strategy for your workflows.

### Section 16: Moving to Declarative Kubernetes YAML

In this section, you’ll learn about the declarative approach to managing Kubernetes resources using YAML files. We’ll explore `kubectl apply` as the preferred method for deploying configurations in a DevOps environment and walk you through the process of using manifests to define and control resources.

You’ll discover how to build your own YAML files from scratch and leverage commands to assist in this process. We’ll also cover dry runs and diffs to test your configurations before deployment, ensuring that your changes are correct. You’ll also learn about labels and label selectors, which help organize and manage Kubernetes objects efficiently.

### Section 17: Your Next Steps and The Future of Kubernetes

In this final section, we’ll look at your next steps in mastering Kubernetes and where the technology is headed. We’ll start by covering storage in Kubernetes, including how volumes provide persistent storage for your applications. We’ll then explore Ingress, which allows you to manage HTTP traffic routing at Layer 7, and dive into custom resources and the operator pattern to extend Kubernetes functionality.

You’ll also learn about higher-level abstractions for deployments and how to template YAML configurations for more complex applications. We’ll introduce the Kubernetes Dashboard, a web GUI for cluster management, and explain how namespaces and contexts help manage multiple Kubernetes clusters. Finally, we’ll take a look at the future of Kubernetes and the trends to watch as it continues to evolve.

### Section 18: Docker Security Good Defaults and Tools

This section focuses on the best practices and tools for securing your Docker environment. You’ll begin by learning the top 10 security steps to follow for Docker. We’ll explore Docker Cgroups and Namespaces, which help secure your containers by leveraging Linux utilities. Then, we’ll dive into Docker Engine’s out-of-the-box security features and show you how Docker's default settings reduce your risk profile.

You’ll also discover Docker Bench, a security scanning tool for assessing the host configuration, and learn how to avoid running containers as root by using the `USER` directive in Dockerfiles. We’ll introduce Docker User Namespaces, an added layer of security, and walk you through enabling user namespaces. Additionally, we’ll explore code repo and image scanning for CVEs (Common Vulnerabilities and Exposures) to protect against potential threats.

Further, you’ll learn about advanced security features like Sysdig Falco, content trust, and custom security profiles using Seccomp and AppArmor. We’ll also cover Docker Rootless Mode, which allows you to run the Docker daemon without root access, and discuss security considerations for Windows containers. Finally, we’ll look at distroless images and evaluate whether they provide extra security, as well as dive into Docker secrets management for protecting container data.

### Section 19: Docker 19.03 Release New Features

In this section, we’ll explore the exciting new features introduced in Docker 19.03. You’ll start with BuildKit, the new build subsystem, and the enhanced `docker buildx` CLI, which simplifies building multi-platform images. We’ll also look at Docker Context, which helps manage Docker connections to multiple environments, including SSH connections.

You’ll learn about Docker App and its ability to package Compose YAML files for more efficient application deployment. Additionally, we’ll cover the introduction of Docker’s Rootless Mode in the Docker Engine, which offers a more secure way to run containers without requiring root privileges. We’ll also touch on Docker Desktop Enterprise and the features it brings to the table, including support for enterprise clusters.

### Section 20: DevOps and Docker Clips

This section takes a DevOps perspective on using Docker, with a series of practical scenarios. We’ll start by discussing the security of Alpine base images and whether they offer better protection compared to other base images. We’ll cover how to handle non-root users in containers and manage file permissions effectively.

Next, we’ll explore containerizing an Apache web server, examining whether it’s better to run multiple sites in one container or use separate containers for each site. We’ll also discuss potential network conflicts when Docker IP subnets overlap with outside networks and explore the use of Docker for Raspberry Pi development.

We’ll dive into Windows 10 containers and their process isolation features, and also cover best practices for using Docker with Postgres. You’ll learn how to use Supervisor to run multiple applications in a container and when to use Docker Compose vs. Swarm for managing single-server environments.

You’ll also discover how to configure Docker environment variables and entrypoints, containerize Java and JBoss with one `.war` file per container, and implement TLS in both development and production environments. Additionally, we’ll cover the topic of using multiple Docker images from a single Git repository, utilizing Docker with ARM devices like Raspberry Pi or AWS A1 instances, and managing role-based access control (RBAC) in Docker and Swarm.

Finally, we’ll discuss the differences between `ENTRYPOINT` and `CMD` in Dockerfiles, how to use external storage in Docker, whether you can turn a VM into a container, and how to manage startup order in multi-container applications.

### Section 21: DockerFile and Compose File Reviews

In this section, we’ll review real-world Dockerfiles and Compose files. You’ll get insights into improving your Dockerfiles by reviewing examples such as a PHP Dockerfile, PHP with Apache and Alpine, and PHP with FPM. We’ll also examine an Elasticsearch Compose stack file to give you practical guidance on creating optimal Docker setups.

### Section 22: Extras, Common Questions, and Resources

This final section offers extra resources to enhance your Docker skills. We’ll provide templates for good defaults in Docker for Node.js and PHP, helping you get started quickly with best practices. You’ll also learn about the Docker Certified Associate (DCA) certification and how it can benefit your career.

In addition, we’ll offer bonus content, including access to all my content update notifications on Patreon, and give you the chance to sign up for my newsletter. You’ll also find exclusive coupons for Docker Mastery, Kubernetes Mastery, Docker for Node.js, Swarm Mastery, and more. We’ll finish by discussing what’s next in your Docker journey.

## Additional Information
- **`docs` directory**: This repository contains a `docs` folder with a document that includes a secure password to access additional content.
- **`resources` directory**: This repository includes a `resources` folder with course materials, also protected by a secure password.
