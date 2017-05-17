---
layout: post
title:  "Adventures in Serverless"
date:   2017-05-17 20:22:54 +0100
categories: serverless AWS
---

You might have hears about the wonderful service from AWS called [Lambda][aws-lambda] which basically alows you to write code and run it in the cloud
without worrying about provisioning of web servers - hence the name for the approach/architecture: serverless.

This is an incredibly powerful tool that allows you to orchestrate complex architecture by splitting it to small manageable chunks.

The way it works is that Lambda are triggered by events which can be a lot of things: HTTP request from API Gateway, a file uploaded to S3 bucket or just run as a cron job.

I was looking for an idea for a side project that I could use to learn how to utilise AWS and Lambdas for all sorts of scenarios, and I have come up with something:
feature flags API. Idea is to start of with a basic CRUD that can return a JSON in following format:

{% highlight javascript %}
{
    "featureNameA": true,
    "featureNameA": false,
    ...etc
}
{% endhighlight %}

And some endpoint that one could use to edit/delete those feature flags. So the requirements at this stage where:
- CRUD feature flags API with minimum data
- AWS Lambda + other services is necessary

Hence was the start of the [Serverless Feature Flags](serverless-feature-flags). One of the things I have decided to do was to use [Serverless framework][severless-framework] which
gives you an easy way to define triggers/resources for your Lambdas and help you deployment and tear down process.

Tune in next time where I will tell a story of how I got from 0 to basic API working and how I then optimised the code.


[aws-lambda]: http://docs.aws.amazon.com/lambda/latest/dg/welcome.html
[serverless-feature-flags]: http://docs.aws.amazon.com/lambda/latest/dg/welcome.html
[serverless-framework]: https://serverless.com/

