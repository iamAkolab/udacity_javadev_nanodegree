# The Java Application Server

A Java Application Server is a pluggable architecture that can host many deployed applications at once. It provides utilities like multi-threading, 
request filtering, and resource sharing to each application. Those applications must expose endpoints that handle the requests routed to them by the server.

![Java Application Server](https://github.com/iamAkolab/udacity_javadev_nanodegree/blob/main/part2_spring_boot_basic/lesson2/l1-16-the-java-application-server.jpg)

## Key Terms
* HTTP: Hypertext Transfer Protocol. A binary protocol that originally defined the mechanics of requesting and sending HTML over the internet.
* Web Server: A program that listens for and responds to HTTP requests over the internet
* Application Server: A program that hosts other applications, forwarding incoming requests to the appropriate application according to a filter. Provides shared access to resources and multi-threading.
* Pluggable Architecture: A pluggable architecture refers to any piece of software that allows parts of it to be added, replaced, and removed. Usually, this is achieved through a common interface for every "pluggable" component. Sometimes the architecture can even replace components at runtime, as is the case with Servlets in an Application Server.
* Threads/Threading: These terms come from concurrent programming - a thread is essentially one track of computation, and multi-threading is running multiple threads in parallel. This gets a little complicated because your CPU has a limited number of physical cores that can process instructions in parallel, while the number of threads you can have can be many more than your computer has cores, but that's a topic for another time!

## Things to remmber
* Apps are Managed and Run by Java Application Servers
* They can access Resorces provided by the Server
* There May be Many Other Apps on the Same Server
