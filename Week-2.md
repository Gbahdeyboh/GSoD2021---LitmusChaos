# Week 1
Last week, I started to learn Kubernetes as a requirement for learning Litmus. It's been a really interesting journey and I've made a lot of progress since then.

Last week, I went through a few resources and started taking an introductory course to Kubernetes thought by Nana. This week, I was able to successfully complete the course, create, and deploy my first ever Kubernetes cluster. Yaaayy!. 

Asides from Nana's course, I was also able to continue going through the Kubernetes documentation while taking their Interactive Tutorials.


### What did I learn?
- Familiarized myself with kubectl commands.
- Learned CRUD deployment commands and Created my first Deployment.
- Learned about Kubernetes YAML configuration files, it's structure, format, and how to create them.
- Created my first deployment from a YAML configuration file.
- Learned about K8's YAML labels and selectors and how to match them.
- Learned to create ConfigMaps with k8's YAML files.
- Learned to create Secrets with with K8's YAML files. 
- Understood how services works, their types, and created my first ever Service.
- Learned how to create Load Balancers (External service).
- Created and deployed a Node-exprees and MongoDB application on a Kubernetes Cluster.
- Understood namespaces, their types, why it is needed, and how they work.
- Learned the basics of ingress
- Understood the basics of Pckage Management tool, Helm.
- Learned the basics of Volumes and persistent Storages.
- Went through the overview of Stateful and Stateless applications.

## What could I have done better?
- I spent too much time trying to Debug an issue rather than just Move on. I had an issue with Ingress and Ingress is currently not supported on arm64 Laptops(Macbook M1's). I didn't realize this on time.

## What were the challenges I faced?
I still need to scheme through Nana's course again, a lot of stuffs Mentioned in the last part of the course are not fully understood yet. I find myself having to sonstantly go back to recall even the most basic stuffs. I guess this is because I am still very new to Kubernetes.

## What's next?
- Create a sample project.
- Dockerize the sample project and push it to a Docker registry.
- Create A Kubernetes Cluster for this smaple project using the Docker Image you created. tent
- Host your Kubernetes Cluster on the cloud and make it publicly accessible.
- Create a Storage Volume and try to make it persistent.

