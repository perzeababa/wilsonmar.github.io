---
layout: post
filename: api-ecosystem
title: "API Development Ecosystem"
excerpt: "It does your job. And helps others to do your job."
tags: [API, ecosystem, swagger, generation]
image:
# pic-blue-city-abu-dhabi-skyscrapers-1900x500
  feature: https://cloud.githubusercontent.com/assets/300046/15269473/c8311bfa-19bc-11e6-890c-06abc511ef39.jpg
  credit: Tian Xinqi
  creditlink: http://www.tianxinqi.com/news/Above80swgpuwnk
comments: true
shorturl: https://goo.gl/wojj1R
---
<i>{{ page.excerpt }}</i>

<hr />

{% include _toc.html %}

This tutorial is about the elements of an ecosystem for 
<strong>development</strong> of Application Programming Interfaces (APIs).

<amp-youtube data-videoid="HjTjXpfdf60" layout="responsive" width="480" height="270">
</amp-youtube>
In this 3 minute video, click "CC" to toggle Closed Captioning text below.

<strong>API services</strong> obtain revenue based on access by 
<strong>client apps</strong> written by other 
<strong>developers</strong>.

But first those developers need to find (<strong>discover</strong>) that the API exists,
perhaps from <strong>galleries of available APIs</strong>
such as <a target="_blank" href="https://apis.guru/">apis.guru</a>.

It's helpful to have a comparison of results from static
<strong>quality scans</strong> evaulating machine-readable
<strong>interface specs</strong> of the API.

There are several competing API specification formats (such as RAML, WADL, and Swagger).
But [Swagger](/swagger/) seems to be the most popular at this time.

<strong>Discussion</strong> and evaluation of APIs can be more focused
when they revolve around community agreement of a specific set of
<strong>rules</strong> driving quality scans.

<strong>Documentation</strong> about the API helps not only
for the API to be discovered from the public galleries,
but also for developers to more quickly appreciate the intricacies of that API.

What's even better than reading documentation 
is to interact live with a sample <strong>demonstration</strong> app
so developers and potential users can really grasp the value of the services exposed.

Then developers would be more enticed to get <strong>API keys</strong>
client apps need to provide when accessing API services.

It helps to have enough <strong>sample data</strong> so
sample <strong>test automation scripts</strong> have the test coverage needed
to give assurance that all features really work, and work quickly, even under load. 

Many developers now also like having a <strong>mock server</strong> running locally
so they can work anywhere with a stable end-point, even while off the network.
Many have found this shortens development cycles by reducing the need to wait for others to
achieve stability in dependent modules.

All this is what makes up a "full" API ecosystem.

<amp-img width="650" height="286" alt="api-ecosystem-v05-a-650x286-69"
src="https://cloud.githubusercontent.com/assets/300046/16362494/68d05a36-3b6d-11e6-8af3-5df961e1d778.jpg">
</amp-img>

<hr />

It takes <strong>effort</strong> 
to create docs, demo, test, and mock server code.

That is why many have begun writing automated generation of such code.

But ideally, the <strong>logic</strong> used to generate this code 
would be based on both the interface specifications and 
<strong>wisdom</strong> culled from analysis of the 
<strong>metadata</strong> gleaned from patterns in data over time
and analysis of history previously only used for <strong>billing</strong>.

More sophisticated variation of <strong>data values</strong> in generated code
is now the frontier.
Such data include values and statistics from both historical points in time 
and projections plus predictions of values expected in the future.

With apps of enterprise scope and complexity,
<strong>manual</strong> coding of the client and server code-base by human developers
can seem repetitive and be error-prone, therefore taking more time and 
be more expensive than what could be.

So instead of manually defining interface specs,
they can now be generated from the 
<strong>code base</strong> 
by marking up server code with 
comments
recognizeble by a <strong>parser such as Doxegen</strong>.

All this cuts <strong>time to market</strong> because changes to server code
can now be quickly reflected in the 
docs, the client demo code, mock server code, test code, and benchmark run results.


<a name="Diagram"></a>

<amp-img width="650" height="305" alt="api-ecosystem-v05-650x305-64.jpg"
src="https://cloud.githubusercontent.com/assets/300046/16363159/2761d3c4-3b7f-11e6-9dd9-31f8b6b46d70.jpg">
</amp-img>


## More on API Microservices #

This is one of a series:

{% include api_links.html %}