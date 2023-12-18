---
title: MVC vs MVVM
date: 2023-12-18 08:48:29
tags: MVC, MVVM
---
This article explain the difference between mvc and mvvm.
<!-- more -->
## MVC (Model-View-Controller)
MVC is a widely used design pattern, especially in web applications. It divides the application into three interconnected components:
- **Model**: Represents the data and business logic of the application. Manages the data, logic, and rules of the application.
- **View**: Represents the UI components. Displays data from the model to the user and sends user commands to the controller.
- **Controller**: Acts as an interface between Model and View. Processes user input, makes changes in the Model.

### Example:
- **Model**: Server-side database table `Users` and related business logic.
- **View**: HTML + CSS page displaying user data.
- **Controller**: Server-side script handling HTTP requests, interacting with Model, passing data to View.

## MVVM (Model-View-ViewModel)

MVVM is primarily used in graphical user interfaces and introduces the ViewModel.

- **Model**: Similar to MVC, it represents the data and the business logic.
- **View**: Similar to MVC, represents the UI. The View is active; it updates itself if the ViewModel changes.
- **ViewModel**: Serves as a middleman between the Model and the View. Transforms Model information into View-friendly data, implements properties, and commands for binding.

### Example:
In a WPF application:
- **Model**: Classes like `User` with properties (Name, Email).
- **View**: XAML pages defining the UI.
- **ViewModel**: C# class transforming Model data into View-friendly data, implements data binding.

## Differences:

1. **Data Binding**: MVVM relies on data binding, while MVC often requires manual updating of the View.
2. **Testability**: MVVM enhances testability of UI logic, as ViewModel doesn't need a View reference.
3. **Use Case**: MVC is used for web applications, MVVM for desktop/mobile applications.
4. **Complexity**: MVVM can be more complex due to data-binding but leads to cleaner separation of GUI and business logic.
