# MULTITHREADING
To develop a multithreading application that uses shareable resources. Any entity willing to access shareable resource must be a stream. The application must implement functionality defined by the individual task.
## PORT
Ships enter port for offloading and/or loading containers and are moored to the dockings. Each docking can have only one ship moored. Containers are offloaded from the ship to the port warehouse and/or from the warehouse to the ship. Number of containers cannot exceed the capacity of a warehouse or ship. Each ship must be handled.
### Требования
+ Программа должна использовать возможности синхронизации, поставляемые
библиотеками java.util.concurrent и java.util.concurrent.locks.
+ Не использовать synchronized, volatile, BlockingQueue и другие ограниченно
потокобезопасные коллекции.
+ Классы и другие сущности приложения должны быть грамотно структурированы по пакетам
и иметь отражающую их функциональность название.
+ Использовать шаблон State для описания состояний объекта, если только этих состояний
больше двух.
+ Для создания потоков использовать по возможности Callable
+ Вместо Thread.sleep использовать только возможности перечисления TimeUnit.
+ Данные инициализации объектов считывать из файла.
+ В приложении должен присутствовать потокобезопасный Singleton.
+ Для записи логов использовать Log4J2.
+ Разрешается для вывода работы потоков использовать метод main
