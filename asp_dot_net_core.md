# Dependency Injection in Dot net core
  -A dependency is any object that another object requires. 
  1. Transient
    Transient lifetime services are created each time they're requested from the service container. This lifetime works best for         lightweight, stateless services.

  2. Scoped
     Scoped lifetime services are created once per client request (connection).
     When using a scoped service in a middleware, inject the service into the Invoke or InvokeAsync method. Don't inject via constructor        injection because it forces the service to behave like a singleton.
     
  3. Singleton lifetime services are created the first time they're requested (or when ConfigureServices is run and an instance is    specified with the service registration). Every subsequent request uses the same instance. If the app requires singleton behavior, allowing the service container to manage the service's lifetime is recommended. Don't implement the singleton design pattern and provide user code to manage the object's lifetime in the class.
