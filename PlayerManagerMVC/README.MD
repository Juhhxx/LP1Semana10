```mermaid
---
title: PlayerManagerMVC
---
    classDiagram
        class CompareByName
        class Controller
        class UglyView
        class IView
        class IView
        <<interface>> IView
        class IComparable
        <<interface>> IComparable
        class IComparer
        <<interface>> IComparer
        class PlayerOrder
        <<Enumeration>> PlayerOrder
        
        CompareByName ..|> IComparer
        Player ..|> IComparable
        UglyView ..|> IView
        Controller --o Player
        UglyView --o Player
        CompareByName --> Controller
        CompareByName ..> Player
        UglyView ..> Controller
        PlayerOrder --> Controller
```