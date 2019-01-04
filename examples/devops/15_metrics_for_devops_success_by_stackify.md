# 15 metrics for devops success by Stackify

See https://stackify.com/15-metrics-for-devops-success/

Contents: 

* [Deployment frequency](#deployment-frequency)
* [Deployment time](#deployment-time)
* [Lead time](#lead-time)
* [Customer tickets](#customer-tickets)
* [Automated tests pass %](#automated-tests-pass)
* [Defect escape rate](#defect-escape-rate)
* [Availability](#availability)
* [Service level agreements](#service-level-agreements)
* [Failed deployments](#failed-deployments)
* [Error rates](#error-rates)
* [Application usage & traffic](#application-usage-traffic)
* [Application performance](#application-performance)
* [Mean time to detection (MTTD)](#mean-time-to-detection-mttd)
* [Mean time to recovery (MTTR)](#mean-time-to-recovery-mttr)
* [Application metrics](#application-metrics)


## Deployment frequency

Tracking how often you do deployments is a good DevOps metric. Ultimately, the goal is to do more smaller deployments as often as possible. Reducing the size of deployments makes it easier to test and release.

You may want to count both production and non-production deployments separately. How often you deploy to QA or pre-production environments is also important. You need to deploy early and often in QA to ensure time for testing. Finding bugs in QA is important to keep your defect escape rate down.


## Deployment time

Tracking how long it takes to do an actual deployment is another good metric. One of our applications at Stackify is deployed with Azure worker roles and it takes about an hour to deploy. It is a nightmare. Tracking such things could help identify potential problems. It is much easier to deploy more often when the task of actually doing it is quick.


## Lead time

If the goal is shipping code quickly, this is a really key DevOps metric. I would define lead time as the amount of time that occurs between starting on a work item until it is deployed. This helps you know that if you started on a new work item today, how long would it take on average until it gets to production. This is also a good metric to help with BizDevOps.


## Customer tickets

The best and worst indicator of application problems is customer support tickets and feedback. The last thing you want is for your users to find bugs or have problems with your software. Because of this, they also make a good indicator of application quality and performance problems.


## Automated tests pass %

To increase velocity, it is highly recommended that your team makes extensive usage of unit and functional testing. Since DevOps relies heavily on automation, tracking how well your automated tests work is a good DevOps metrics. It is good to know how often code changes are causing your tests to break.


## Defect escape rate

Do you know how many software defects are being found in production versus QA? If you want to ship code fast, you need to have confidence that you can find software defects before they get to production. Your defect escape rate is a great DevOps metric to track how often those defects make it to production.


## Availability

The last thing you ever want is for your application to be down. Depending on your type of application and how you deploy it, you may have a little downtime as part of scheduled maintenance. I would suggest tracking that and all unplanned outages.


## Service level agreements

Most companies have some service level agreement (SLA) that they operate with. It is also important that you track your compliance with your SLAs. Even if there are no formal SLA, there probably are application requirements or expectations to be achieved.


## Failed deployments

We all hope this never happens, but how often do your deployments cause an outage or major issues for your users? Reversing a failed deployment is something we never want to do, but it is something you should always plan for. If you have issues with failed deployments, be sure to track this metric over time. This could also be seen as tracking mean time to failure (MTTF).


## Error rates

Tracking error rates within your application is super important. Not only are they an indicator of quality problems, but also ongoing performance and uptime related issues. Good exception handling best practices are critical for good software. Errors are a fact of life for most applications, and it is important that you keep a pulse on your error rates and look for spikes.


## Application usage & traffic

After a deployment, you want to see if the amount of transactions or users accessing your system looks normal. If you suddenly have no traffic or a giant spike in traffic, something could be wrong.

The last thing you ever want to see is no traffic at all. You could also see a spike in traffic if you are using microservices and one of your applications is causing a lot more traffic all of a sudden.


## Application performance

Before you even do a deployment, you should use a tool like Retrace to look for performance problems, hidden errors, and other issues. During and after the deployment, you should also look for any changes in overall application performance.

It might be common after a deployment to see major changes in the usage of specific SQL queries, web service calls, and other application dependencies. Tools like Retrace can provide valuable visualizations like this one below that helps make it easy to spot problems.


## Mean time to detection (MTTD)

When problems do happen, it is important that you identify them quickly. The last thing you want is to have a major partial or broad system outage and not know about it. Having robust application monitoring and good coverage in place will help you detect issues quickly. Once you detect them, you also have to fix them quickly!


## Mean time to recovery (MTTR)

This metric helps you track how long it takes to recover from failures. A key metric for the business is keeping failures to a minimum and being able to recover from them quickly. It is typically measured in hours and may refer to business hours, not clock hours.

Having good application monitoring tools in place to quickly identify issues and quickly deploy the fix is important to reducing your MTTR.


## Application metrics

Beyond the DevOps metrics listed above, there are dozens of other metrics you can track that are specific to your applications. Most of them are not necessarily relevant to DevOps in regards to deploying your application. However, they are very critical for monitoring the usage and performance of your applications in production.

For example, at Stackify, we use custom metrics to track how many log messages are received via our API per minute. This is a critical metric that helps us understand the volume of data flowing through our system. Depending on your application, you may have similar custom metrics that are critical to your application.
