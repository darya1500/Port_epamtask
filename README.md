# MULTITHREADING
To develop a multithreading application that uses shareable resources. Any entity willing to access shareable resource must be a stream. The application must implement functionality defined by the individual task.
## PORT
[Ships](https://github.com/darya1500/epam_task/blob/master/src/main/java/by/epam/learn/daryatarasevich/port/entity/Ship) enter [port](https://github.com/darya1500/epam_task/blob/master/src/main/java/by/epam/learn/daryatarasevich/port/entity/Port) for offloading and/or loading containers and are moored to the dockings. Each docking can have only one ship moored. Containers are offloaded from the ship to the port warehouse and/or from the warehouse to the ship. Number of containers cannot exceed the capacity of a warehouse or ship. Each ship must be handled.
### Requirements
+ Program should use synchronization capabilities provided by the java.util.concurrent and java.util.concurrent.locks libraries.
+ Do not use synchronized, volatile, BlockingQueue and other partially threadsafe collections.
+ Classes and other entities of application must be correctly structured in packages and named reflecting their functionality.
+ Use the [State](https://github.com/darya1500/epam_task/tree/master/src/main/java/by/epam/learn/daryatarasevich/port/state) template to describe states of an object, only if there are more than two states.
+ Whenever possible, use [Callable](https://github.com/darya1500/epam_task/blob/master/src/main/java/by/epam/learn/daryatarasevich/port/entity/Ship) to create threads.
+ Instead of Thread.sleep, use only the capabilities of the TimeUnit enumeration.
+ [Read objects initialization data from files](https://github.com/darya1500/epam_task/tree/master/src/main/java/by/epam/learn/daryatarasevich/port/reader).
+ The application must include a thread safe [Singleton](https://github.com/darya1500/epam_task/blob/master/src/main/java/by/epam/learn/daryatarasevich/port/entity/Port).
+ To record logs use Log4J2.
+ It is allowed to use the[ main](https://github.com/darya1500/epam_task/tree/master/src/main/java/by/epam/learn/daryatarasevich/port/main) method to display the work of threads.
