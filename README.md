# Docker Registry
A stateless, highly scalable server side application that stores and lets you distribute Docker images

## Resources
* [Homepage](https://docs.docker.com/registry/)
* [Documentation](https://docs.docker.com/registry/)

## kustomization
This kustomization will create the following Kubernetes Resources:
* A [Namespace](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/) named *docker-registry* in which the whole application resides.
* A [Deployment](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/) + [Service](https://kubernetes.io/docs/concepts/services-networking/service/) named *docker-registry*.
* An empty [ConfigMap](https://kubernetes.io/docs/concepts/configuration/configmap/) + [Secret](https://kubernetes.io/docs/concepts/configuration/secret/) *docker-registry* for configuration.

## Configuration
The application can be configured through the generated ConfigMap and Secret as they get injected as environment variables.
