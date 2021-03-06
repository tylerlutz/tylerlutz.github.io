---
layout: post
title:  "NodeJS"
date:   2016-02-24 13:00:00 -0500
categories: tutorials
---
This post was created to explain to you the concepts of NodeJS and tell you what exactly NodeJS is and what it can be used for. We will answer three basic questions; What is NodeJS, What makes NodeJS different?, and What is non blocking?. 
<br />
<br />
NodeJS is a server side language built on Google Chrome's V8 JavaScript Engine. NodeJS is a cross platform is a cross-platform runtime environment that can be ran on Linux, Mac OS X, and Windows. NodeJS is a simply server-side JavaScript that can be used for many different use-cases but the large advantage to Node is that Node can scale very well. Node is scalable due to the fact that it can handle concurrency very well, meaning that if 100 request hit the server at once but the task should only take 2 seconds, then each request should be completed in two seconds. This is different from other server-side languages which would take a request, wait 2 seconds, and then do the next request. 
<br />
<br />
Other than the scalability of Node, there are many other reasons that makes Node different from other programming languages. The big differences is that Node is built on JavaScript, Node is simply JavaScript for the server. This makes it a lot easier for the developer to write code because what they can write for the browser, can most likely be used on the server side and vise versa. This concept alone is what is making Node so popular, it is so much easier on the developer. But the scalability of Node and its efficiency is what makes it so much different from other languages. For example, a request is made to a web server to get data from a JSON file, other languages would be waiting for the response from the JSON file, while Node would be working on the next steps or an entirely different request while that file is fetched. This allows resources to be more efficient by working ahead or on a different request instead of idling while that single request is being processed.
<br />
<br />
The example below was taken from a stack overflow thread illustrating the difference between Blocking and Non-Blocking.
<img src="img/node_nonblocking.png" />
<br />
Node is a non-blocking language. It continues to work while another task is being completed in the background. As you can see in the example above, the blocking code alerts 1 then waits to alert 2 while the non-blocking code alerts 1, then starts to work on the fetch statement, but goes on to alert 3 while it is waiting for the fetch statement to be completed. Why is this important? Other languages that use the blocking concept are not using all of their resources efficiently i.e. the CPU and RAM. These resources go into idle while waiting for the task to complete. Non-blocking languages allow the program to continue and allows the CPU and Memory to work on other tasks while waiting for that fetch statement to conclude. This allows the program to better utilize the resources and becomes more efficient because there is less idle time in the program.

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
