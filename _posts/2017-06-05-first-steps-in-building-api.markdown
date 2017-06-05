---
layout: post
title:  "First steps into building our API with Lambdas"
date:   2017-06-05 21:40:00 +0100
categories: serverless AWS
---

When deciding what stack to use and and which services to go for, I decided to go for very basic things that would server my needs.
As I wanted to build API using JavaScript and Lambdas, I needed to pick a storage layer for where I would keep my data.

The choice was clear and simple: DynamoDB....

Played around with AWS-SDK from npm, to see what sort of calls/parameters I need, etc:
http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/DynamoDB.html

Support for promises in aws sdk: https://aws.amazon.com/blogs/developer/support-for-promises-in-the-sdk/

Set up DynamoDB in serverless YAML
{% highlight javascript %}
{
    code example 1: YAML
}
{% endhighlight %}


Writing first endpoint

etc.

Set up DynamoDB in serverless YAML
{% highlight javascript %}
{
    first piece of code
}
{% endhighlight %}


[aws-lambda]: http://docs.aws.amazon.com/lambda/latest/dg/welcome.html
[serverless-feature-flags]: github.com/VladDubrovskis/serverless-feature-flags
[serverless-framework]: https://serverless.com/

