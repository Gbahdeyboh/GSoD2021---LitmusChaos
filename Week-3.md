# Week 3
[Last week](https://github.com/Gbahdeyboh/GSoD2021---LitmusChaos/blob/master/Week-2.md), I completed Nana's course on Kubernetes and was able to understand a host of different stuffs. 

This week, I did a revision of the course, Docker and worked on a really Interesting project. I spent most of the week trying to revise stuffs and figure out how to comeplete the project I worked on.
It was a really simple project, but it is my first ever Kubernetes project and I'm really excited about it.

I was able to build a very basic web API service using NodeJS and MongoDB, this basic application was then containerized with Docker. The Docker image was pushed to Dockerhub.

This image was then deployed on a Kubernetes. My K8s cluster had two pods; the app pod and the mongoDB pod.
The app pod pulls the docker image I built from dockerhub, and uses a LoadBalancer Service to expose this pod.
The mongo pod pulls the mongo image, and exposes it over a ClusterIP Service. But this had a bit of problem, each time the pod dies, I loose all of the previously stored data. 
This made me see the need to implement a Persistent Volume Claim. I added PVC suport to the mongo Deployment and was able to persist stored data even after the pod dies. 

You can read more about the app I built, what it does, and also take a look at it's code [here](https://github.com/Gbahdeyboh/kubernetes-practice).

### Which of the things learned was applied while working on this project??
- Deployments.
- Services.
- ConfigMaps.
- Secrets.
- Containerization.
- Persistent Volume Claims.

## What could I have done better?
It's funny that I can't think of one right now, but when something comes to my mind, I will definitely edit this to reflect that.

## What were the challenges I faced?
Bugs everywhere😢.
Some of the stuffs I did where copied and pasted and sadly it took me some time to realize that I had wrongly understood how environment variables are passed froetm a deployment down to a container. 
I was able to get help from the `Kubernetes-novice slack` channel. I struggled with several stuffs too, but this was the one that took me the most time to understand.

## What's next?
- Undertsand what Chaos Engineering is, and why it is needed/important.
- Learn Litmus 🥳🥳🥳🥳.
- Attempt to build my own Chaos Engineering workflows with Litmus.
- Get more familiar with the Litmus tutorials structure and the tools I would be needing to contribute to it e.g codelab.

