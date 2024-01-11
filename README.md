# Test-Driven Development Challenge
The Java Spring API was developed using the Test-Driven Development (TDD) method, interpreting and adhering to the project’s integration tests. The project was structured with repository, service, and controller (web) layers. The implementation also includes exception handling configurations.

## Diagrama de Classes
``` mermaid
classDiagram
  class Event {
    + Long id
    + String name
    + LocalDate date
    + String url
    + City city
  }

  class City {
    + Long id
    + String name
    + Event[] events
  }

  City "1" *-- "*" Event
```
