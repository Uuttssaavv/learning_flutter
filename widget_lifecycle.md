

### Flutter Widget Lifecycle Guidance
--- 
</br>

----
| **Lifecycle Method**       | **Description**                                                  | **Usecase** | **Example** |
|----------------------------|------------------------------------------------------------------|-------------------|-------------|
| `createState`              | Called when a stateful widget is created. Initializes the state object. | Return a new instance of the State class associated with this widget. | Return a new instance of `_MyWidgetState` for a `MyWidget` stateful widget. |
| `initState`                | Called once when the state object is created. Used for one-time initialization. | Set up initial state, start animations, or fetch initial data. Call `super.initState()`. | Start an animation or initiate a network request. |
| `didChangeDependencies`    | Called when the widget’s dependencies change.                     | Handle changes to inherited widgets or other dependencies. | Update state when an inherited theme changes. |
| `build`                    | Called whenever the widget needs to be rendered.                  | Construct the widget tree. Keep it pure and avoid side effects. | Return the widget tree for the current state. |
| `didUpdateWidget`          | Called whenever the widget configuration changes.                 | Handle updates to properties and state that depend on widget parameters. | Reset a timer if the duration property of the widget changes. |
| `setState`                 | Triggers a rebuild of the widget when the state changes.          | Use to update the UI in response to state changes. Minimize the amount of state changes to optimize performance. | Update the UI when a user interacts with a button. |
| `deactivate`               | Called when the state object is removed from the tree temporarily. | Clean up resources that can be recreated easily or might change when the widget reattaches. | Pause an animation when the widget is removed from the tree. |
| `dispose`                  | Called when the state object is permanently removed. Used for cleanup. | Dispose of resources such as controllers, animation objects, and listeners. Always call `super.dispose()`. | Dispose of a `TextEditingController` or stop a subscription to a stream. |
