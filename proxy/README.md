## Proxy

Proxy pattern provides a surrogate or placeholder for another object to control access to it.
The pattern has structural purpose and applies to objects. 

### When to use

* whenever there is a need for a more versatile or sophisticated reference to an object than a simple pointer

## UML

```mermaid
 classDiagram
      direction LR
      class Client
      class Subject
      <<abstract>> Subject
      class RealSubject
      class Proxy
      
      Client-->Subject
      
      Subject <|-- Proxy
      Subject <|-- RealSubject
      
      Proxy-->"realSubject" RealSubject
      
      Subject : operation()*
      Proxy : operation()
      RealSubject : operation()
```
## TO LEARN MORE

https://reactiveprogramming.io/blog/es/patrones-de-diseno/proxy
