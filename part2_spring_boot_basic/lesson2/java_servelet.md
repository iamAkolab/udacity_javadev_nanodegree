# Java Servlets

The Servlet class is the main connection between the apps you develop and the application server they run on. By extending Servlet, 
you can create endpoints that handle incoming requests in a way specific to your application needs, and you can map specific request 
URLs to specialized servlets by adding entries to a web.xml file. The app server uses this configuration to instantiate and manage 
your servlets. It interacts with each through three standard methods, init, service, and destroy:

* service is where requests are handled, and the server will call this method when a request is routed to the servlet it's called on.
* init is where initialization of the servlet is handled, and the server will call this method directly after instantiating the servlet.
* destroy is where servlet resource cleanup is handled, and is called directly before the server terminates the servlet instance.

![The Lifecycle of a Servlet in an Application Server](https://github.com/iamAkolab/udacity_javadev_nanodegree/blob/main/part2_spring_boot_basic/lesson2/screen-shot-2020-06-03-at-4.51.26-pm.png)

## A quick note on Java Application Files:
When you compile a Java program and package it to be run, the Java compiler creates what is called a Java ARchive, or JAR file. This file 
contains a compressed file hierarchy, with folders that represent Java packages that contain Java .class files, which are the compiled 
versions of .java source code files. It can also contain arbitrary resource files, either at the root level or deeply nested in the package 
hierarchy. These files often contain metadata related to the app or library contained in the JAR file, which can be read by any program that 
interacts with the JAR.

When you want to deploy an app to an app server, you have to package it as a Web application ARchive, or WAR file. A WAR file is almost identical 
to a JAR file, but includes configuration files specific to web applications. When we copy a WAR file into the deployment directory of an app server, 
the server unpackages it, looks for a web.xml file, and uses that file to find the classes and resources required by the application. This uses advanced 
Java features like reflection and class loading to programmatically load Java class definitions and instantiate them which is quite a nifty trick! It 
allows us to dynamically load, start, stop, and replace any number of applications in a web server at any time.

## Key Terms
* Endpoints: An endpoint is the address at which a client can reach a specific part of a server's functionality. Usually, this is a URL path, the /words/and/slashes that follow the domain of a URL, like .com or .org.
* Servlet: A class defined as a part of the Java: Enterprise Edition specification. Provides an implementable interface for web server request processing, defining a service method that the server invokes on an instantiated servlet to handle a ServletRequest and ServletResponse object for an incoming request. The servlet also defines lifecycle methods for the server to invoke when initializing or destroying a servlet.
* JAR: A Java Archive file, which stores compiled .class files in a folder hierarchy that matches the code's package structure. Includes an optional manifest file.
* WAR: A variation on the JAR for web applications, which optionally includes web resources like HTML files and configuration files like web.xml for servlet registration/mapping.
