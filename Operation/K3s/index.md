# K3s

[Home](../../README.md) > [Operation](../index.md)


### More Topic on K3s
- [Instalation](Instalation.md)
- [Longhorn](Longhorn.md)


<br>

## What is K3s?

<br>

<img src="https://k3s.io/img/k3s-logo-light.svg">

<br>

**K3s** is a lightweight, certified distribution of **Kubernetes** designed for edge computing, IoT (Internet of Things), and resource-constrained environments. It is a fully compliant Kubernetes distribution but optimized to run with lower resource usage, making it ideal for environments with limited hardware resources.

## Key Features of K3s

1. **Lightweight**  
   K3s is designed to be more lightweight than the standard Kubernetes distribution. It removes unnecessary features (like non-essential plugins) and uses a single binary that is much smaller than the typical Kubernetes binaries.

2. **Simplified Setup**  
   It simplifies the Kubernetes setup and deployment by using a reduced set of components, making it easy to install and manage. For example, K3s can be installed with a single command, making it more user-friendly.

3. **Low Resource Usage**  
   K3s is optimized for environments where resources (memory, CPU) are limited. This makes it suitable for edge devices, IoT systems, or environments where traditional Kubernetes may not be efficient enough.

4. **Compatibility**  
   K3s is fully compatible with **Kubernetes**, meaning that any applications, services, and tools that work with Kubernetes will work with K3s as well. It is fully certified by the Cloud Native Computing Foundation (CNCF).

5. **Uses SQLite by Default**  
   Instead of using etcd (which is the default for Kubernetes), K3s uses **SQLite** for its cluster database by default, reducing the complexity and resource consumption.

6. **Built-in Support for ARM**  
   K3s supports ARM-based devices, which is especially useful for running Kubernetes on smaller, embedded devices like Raspberry Pi or ARM-based servers.

7. **Low Overhead**  
   With reduced components and simplified architecture, K3s reduces the overhead of running Kubernetes on smaller systems. It uses fewer resources, making it suitable for environments like home labs, edge devices, or even for development purposes.

## Typical Use Cases

- **Edge Computing**  
  K3s is designed to run on edge devices, providing Kubernetes-based orchestration in remote locations or on hardware with limited resources.
  
- **IoT (Internet of Things)**  
  K3s is perfect for managing applications on IoT devices due to its light resource usage and small footprint.
  
- **Development and Testing**  
  K3s can be used for local development or CI/CD pipelines where Kubernetes is needed but full Kubernetes clusters would be too resource-intensive.

- **Home Labs**  
  Developers and enthusiasts use K3s to set up lightweight Kubernetes clusters at home, enabling them to test and deploy cloud-native applications in a small, resource-constrained environment.

## Components of K3s

- **K3s Server**  
  The main control plane node that runs the Kubernetes API server, controller manager, and scheduler.
  
- **K3s Agent**  
  The node that runs the kubelet and connects to the server to run containers.
  
- **Embedded Components**  
  K3s removes and integrates various components like Helm, CoreDNS, and Flannel to simplify Kubernetes deployment and operation.

## Summary

In summary, K3s is an optimized, lightweight version of Kubernetes that is perfect for running Kubernetes clusters in environments with limited resources, such as edge devices, IoT systems, and personal development environments.