# StarWars Search Application

This Android application interfaces with the Star Wars API (SWAPI) to provide information about characters, planets, species, and films from the Star Wars universe. The app features a search page to look up characters (people) and a detail page to display detailed information about selected characters, including their associated planet, species, and films data.

In this branch you'll find:
*   User Interface built with **[Jetpack Compose](https://developer.android.com/jetpack/compose)** 
*   A single-activity architecture, using **[Navigation Compose]([https://developer.android.com/jetpack/compose/navigation](https://developer.android.com/jetpack/androidx/releases/hilt))**.
*   A presentation layer that contains a Compose screen (View) and a **ViewModel** per screen (or feature).
*   Using **[Flow](https://developer.android.com/kotlin/flow)** and **[coroutines](https://kotlinlang.org/docs/coroutines-overview.html)** for asynchronous operations.
*   Dependency injection using [Hilt](https://developer.android.com/training/dependency-injection/hilt-android).


## Screenshots

![Search Page](path/to/your/screenshot1.png)
![Detail Page](path/to/your/screenshot2.png)

## Architecture

This project is organized following the Clean Architecture principles, which divides the code into multiple layers:

### Presentation Layer

- **ViewModels**: Manage UI-related data and handle user interactions.
- **Compose UI**: Jetpack Compose is used to build the UI components.

### Domain Layer

- **Use Cases**: Encapsulate business logic and are invoked by the ViewModels.
- **Entities**: Represent the core data structures of the application.

### Data Layer

- **Repositories**: Abstract the data sources and provide data to the use cases.
- **Data Sources**: Include both remote (e.g., network) and local (e.g., database) data sources.

## Dependency Injection

The project uses Hilt for dependency injection.

### Installation

1. **Clone the repository**:
    ```bash
    https://github.com/aliyousefpoor/SFStarWarsSearch.git
    ```

2. **Open the project** in Android Studio.

3. **Build and run** the project on an emulator or physical device.

## Usage

### Search Page

- **Functionality**: Allows users to search for items using a search bar.
- **Components**: `SearchViewModel`, `SearchScreen`, and related UI components.

### Detail Page

- **Functionality**: Displays detailed information about a selected item.
- **Components**: `DetailViewModel`, `DetailScreen`, and related UI components.
