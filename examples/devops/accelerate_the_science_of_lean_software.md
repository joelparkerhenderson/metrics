# Accelerate: The science of lean software and devops

This page has the devops metrics recommendations from the book "Accelerate: The science of lean software and devops: building and scaling high performance technology organizations" by Nicole Forsgren, Jez Humble, Gene Kim.

Contents:

* [](#)


## Introduction

The book emphasizes continuous delivery of value to users. The authors call this “delivery performance”, and carefully evaluate many possible measures of delivery performance.

The authors recommend four measures as the best, because these measures are accessible, effective, understandible, and provide coverage of many other devops metrics.

Best measures of delivery performance:

* Delivery lead time

* Deployment frequency

* Time to restore service

* Change fail rate

The book carefully connects delivery performance measures with well-known industry devops metrics, and also with well-known lean manufacturing practices.


## Delivery lead time

Delivery lead time is the time it takes for work to be implemented, tested, and delivered. 

For comparison, total lead time is the time it takes to go from a customer making a request to the request being satisfied. The total lead time includes the delivery lead time.

Delivery lead time is easier to measure than total lead time, and also has a lower variability.

Shorter delivery lead time is better since it enables faster feedback on what we are building, and faster course correction.

Shorter delivery lead times are also important when there is a defect or outage, and we need to deliver a fix rapidly and with high confidence.


## Deployment frequency

Deployment frequency is how often the team deploys software to production.

For our purposes, this metric includes all our software (e.g. product releases, infrastructure changes, configuration updates) deployed to all our production environments (e.g. customer applications, sales demonstrations, high-availability backups).

Deployment frequency is our proxy for batch size. Reducing batch size is a central element of the Lean paradigm. However, in software, batch size is hard to measure, and hard to communicate across contexts, because there is no visible inventory. 

Reducing batch size reduces cycle times and variability in flow, accelerates feedback, reduces risk and overhead, improves efficiency, increases motivation and urgency, and reduces costs and schedule growth.


## Time to restore service

Time to restore service is how long it takes to fix a problem in production.

Modern software products and services are rapidly changing complex systems, and some failure is inevitable. We want to know: how quickly can service be restored?

Time to restore service is our proxy for reliability. For comparison, reliability can be measured as mean time between failures (MTBF). MTBF is the predicted elapsed time between inherent failures of a system, during normal system operation. 


## Change fail rate

When making changes to systems, what percentage of changes to production fail?

For our purposes, this metric includes all our software (e.g. product releases, infrastructure changes, configuration updates) deployed to all our production environments (e.g. customer applications, sales demonstrations, high-availability backups).

In the context of Lean, this is the same as percent complete and accurate for the product delivery process, and is a key quality metric.

