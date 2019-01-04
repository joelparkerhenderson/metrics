# 6 Container Performance KPIs You Should be Tracking to Ensure DevOps Success

See https://www.apmdigest.com/apmacademy/container-performance-kpi-devops-success-2

Contents:

* [](#)


## 1. Deployments per period

The ultimate test of speed is in the frequency of deployments. Depending on the stage of evolution your organization is in with regards to DevOps, you may have multiple releases per day or multiple months between each release.

If you already release daily, you should aim for more frequent releases per day. If you deploy every couple of weeks, look to bring that down to once a week.

Note that this KPI would be different for web apps and mobile apps. Typically, web apps are easy to release more frequently as they don't have gatekeepers between you and your app. Mobile apps, on the other hand, have to pass through the gates of the app stores on iOS and Android, and the huge variation in devices and OS versions has to be factored in.

That said, from wherever you are at today, releasing more frequently is the goal, and containers are your best bet to achieve this KPI.


## 2. Creation of new environments

Containers make it easy to spin up a new development or testing environment much faster than VMs. As developers and QA become more confident to create and destroy environments, they are free to build apps in a distributed manner. As they divide complex features and develop or test them in parts, it brings speed in how frequently the app can be deployed.

A key contributing factor to this KPI is the size of container images. With container images, the lighter the better. Lighter container images result in smaller containers, faster startup times, faster transfer across teams, and greater speed across the pipeline.


## 3. percentage of automated tests

Thanks to the concept of shift left, QA is now an active partner from the start of development. Because of this collaboration from the start, QA is in a better spot to do more automated testing than manual testing.

Containers bring predictability and consistency as code and artifacts are passed from Dev to QA. The same containers used to build the app are used in test environments. This enables QA to write and plan for automated tests on the code being written. Automated testing is proven to enable wider testing coverage, catch bugs earlier, improve speed of tests, and make them repeatable. Containers enable these very same objectives.


## 4. Mean time to recovery (MTTR)

Mean time to recovery (MTTR) is one of the oldest IT metrics, but it isn't outdated in a container system. With monolithic applications, an error in any part of the application can bring the entire app to a grinding halt. Containers mitigate this risk by enabling a distributed microservices architecture. Even if a single service fails, other services remain available. This is a big benefit of the transition to containers.

Service failures can occur for a variety of reasons — resource constraints, storage limitations, security breaches, or bugs in the application code. It's important to measure availability for each service in a containerized application, and look to improve it over time.

MTTR is strongly influenced by how well you can monitor your application, and how well-planned you've been in provisioning backups for various resources like EC2 instance backups, or storage volume backups. MTTR is a key KPI that affects quality, and containers can help bring MTTR down to levels you've never seen before.


## 5. Latency

Though latency is an individual metric that can be measured for every service, every container within a service, and every request handled by a container, you can still look at latency as an overall KPI that combines all these individual metrics.

Latency is a key contributor to a great user experience. Today's demanding end users don't want to be left waiting while an application completes a request, a media file buffers, or a page loads — They want their tasks to be executed immediately. Applications that deliver this experience have a clear edge over their rivals that are slower at every stage.

When optimizing for latency, databases play a key role. Ideally, you want to reduce the time requests spend traversing the network, or the time spent querying databases. This requires well-planned networking. The service mesh has emerged as the leading network type for containers. It facilitates east-west communication between containers at large scale.

Similarly, architecting your databases so that they're distributed, and querying them with a powerful search engine can bring great gains.


## 6. Resource utilitization

This KPI is all about efficiency. Once you've seen great improvement in this speed and quality of your software delivery, it's time to make the entire process more efficient. This means saving costs, or better usage of resources. In recent years, orchestration tools have been at the forefront driving efficiency in container operations.

Kubernetes has a great set of defaults to ensure you're using resources efficiently. It lets you set quotas at various levels of the container stack — service, pod, or container. Kubernetes automates the placement of pods (a group of containers) on nodes based on the resources a pod needs, and how many nodes are available. It constantly switches the location of pods as the workload changes. If you don't set limits for a container, it can utilize resources as available.

This may be good for burst performance, but in the case of a malfunctioning container, a single container may hog all resources and leave none for its neighbors. You can set limits for compute in the form of number of CPUs required, and for what duration of time. Similarly, you can set limits on how many MiB or GiB of memory are allocated to a container and for what duration of time. Kubernetes lets you also allot persistent storage for pods, and can dynamically provision storage volumes according to need.

With mature automation rules, Kubernetes is a dream come true for anyone managing containers. As you look to achieve resource utilization KPIs, Kubernetes can't be overlooked.
