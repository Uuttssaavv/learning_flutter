## Overview
In Flutter, widgets are the building blocks of the user interface. There are two primary types of widgets: Stateless and Stateful. 

Understanding the difference between these two types is fundamental for any Flutter developer.

</br>

### Stateful vs Stateless Widgets in Flutter
</br>

| **Aspect**                   | **Stateless Widgets**                                       | **Stateful Widgets**                                      |
|------------------------------|-------------------------------------------------------------|-----------------------------------------------------------|
| **Definition**               | Widgets that do not change over time.                       | Widgets that can change their state during the app's lifecycle. |
| **State Management**         | No internal state management.                              | Manages state internally and can update the UI dynamically. |
| **Lifecycle Methods**        | No lifecycle methods, just a `build` method.                | Has multiple lifecycle methods (e.g., `initState`, `setState`, `dispose`). |
| **Performance**              | Generally more efficient as they do not need to manage state. | Slightly less efficient due to state management overhead. |
| **Use Cases**                | Static content, UI elements that do not change.             | Interactive content, UI elements that change based on user actions or data updates. |
| **Rebuilds**                 | Rebuilt only when parent widget rebuilds.                   | Can trigger rebuilds via `setState`. |
| **State Retention**          | State is not retained and rebuilt each time.                | State can be retained and modified over the lifecycle. |
| **Parent-Child Relationship**| Parent controls configuration and rebuilds.                 | Child can manage its own state independently. |
| **Widget Tree**              | Purely declarative, no side effects.                        | Can have side effects through state changes and `setState` calls. |
| **Examples in Flutter Library** | `Text`, `Icon`, `Container`.                              | `Checkbox`, `Slider`, `Form`. |
---