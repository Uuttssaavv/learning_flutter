The table below provides a quick reference to the equivalent UI components in Flutter, Android, and iOS, along with brief descriptions.

| **Functionality**              | **Flutter**            | **Android**                    | **iOS**                        |
|--------------------------------|------------------------|--------------------------------|--------------------------------|
| Dynamic list                   | `ListView.builder`     | `RecyclerView`                 | `UITableView`                  |
|                                | Creates a scrollable list of widgets        | Displays a list of items with efficient memory usage         | Displays a scrollable list of items  |
| Basic UI container             | `Container`            | `View`                         | `UIView`                       |
|                                | Versatile widget for styling and layout     | Base class for all UI components                     | Base class for all UI components                     |
| Vertical layout                | `Column`               | `LinearLayout` (vertical)      | `UIStackView` (vertical)       |
|                                | Arranges widgets vertically             | Arranges widgets vertically                                | Arranges views vertically                                |
| Horizontal layout              | `Row`                  | `LinearLayout` (horizontal)    | `UIStackView` (horizontal)     |
|                                | Arranges widgets horizontally           | Arranges widgets horizontally                                | Arranges views horizontally                                |
| Overlapping elements           | `Stack`                | `FrameLayout`                  | `UIView` with subviews         |
|                                | Places widgets on top of each other          | Places views on top of each other                          | Places subviews on top of each other                          |
| Basic app structure            | `Scaffold`             | `AppCompatActivity` + layouts  | `UIViewController` + layouts   |
|                                | Provides a basic layout structure       | Basic structure with app bar, drawer, etc.                   | Basic structure for app screens                        |
| Text input                     | `TextField`            | `EditText`                     | `UITextField`                  |
|                                | Input field for text   | Input field for text           | Input field for text           |
| Button                         | `Elevated Button`, `Text Button` | `Button`            | `UIButton`                     |
|                                | Creates a button with various styles         | Creates a clickable button                                | Creates a clickable button                                |
| Navigation                     | `Navigator`            | `FragmentManager` / `Activity` | `UINavigationController`       |
|                                | Manages stack of routes for navigation  | Manages navigation between screens                        | Manages navigation stack                                |
| Image display                  | `Image`                | `ImageView`                    | `UIImageView`                  |
|                                | Displays images        | Displays images                | Displays images                |
| Form grouping                  | `Form` + `FormField`   | `FormLayout` + inputs          | `UIViewController` + inputs    |
|                                | Groups multiple input widgets                | Groups multiple input elements                                | Groups multiple input elements                                |
---