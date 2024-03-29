# The Spring Framework
![The Spring Framework](https://video.udacity-data.com/topher/2020/June/5ed93f8f_l2-10-big-picture/l2-10-big-picture.png)

The figure above shows that Spring takes the component class files and dependency configuration from the developer and instantiates a system of Java objects with references to each other.

Of all the tools we'll be using in this course, Spring is the most important because it defines our entire style of application development. Spring is a framework for Inversion of Control, which means that to use it, we have to package our code into individual component classes, telling Spring which components need each other to function. Spring takes the component classes we define and the dependencies we define between them and instantiates a system of matching Java objects with references to each other. This frees us from having to write so-called "glue code" to instantiate, connect, and manage components manually, and allows us to instead focus on writing so-called business logic, or code that concerns itself exclusively on the conceptual model of the application.

## Key Terms
* Inversion of Control (IoC): A design pattern in which the developer creates independent application components and uses a framework to connect them, rather than writing the integration code themselves
* Business Logic: Code that relates exclusively to an application's conceptual model and featureset. Contrast with utility code like database access, HTTP request parsing, etc.
* Persistent Components: Java Objects that Spring maintains over time; they're persistent because they're created and maintained for as long as the application needs them to be.
* Dependency Injection: A mechanism by which IoC may be implemented. Components are configured with dependencies on other components, which are injected at runtime. Injection is quite literal - a component's dependencies are usually expressed as annotated fields on the component class, and Spring will populate those fields with the dependencies at runtime.
