# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week

## Diagrama de Classes

```mermaid
classDiagram
  class User {
    - name: string
    - account: Account
    - features: Feature[]
    - card: Card
    - news: News[]
  }

  class Account {
    - number: string
    - agency: string
    - balance: double
    - limit: double
  }

  class Feature {
    - icon: string
    - description: string
  }

  class Card {
    - number: string
    - limit: double
  }

  class News {
    - icon: string
    - description: string
  }

  User -- Account: has
  User -- Feature: has
  User -- Card: has
  User -- News: has
```