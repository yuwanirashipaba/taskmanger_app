# TaskAppNew

A simple **task manager / notes** Android app built with **Kotlin**, **Room**, and **MVVM**.

## Features

- **Create / edit tasks**
- **List tasks** in a RecyclerView
- **Local persistence** with Room (SQLite)

## Tech stack

- **Language**: Kotlin
- **Architecture**: MVVM (ViewModel + LiveData)
- **Database**: Room (`TaskDatabase`, `TasksDao`)
- **Async**: Kotlin Coroutines
- **UI**: XML layouts + RecyclerView

## Project info

- **Application ID / namespace**: `com.example.taskappnew`
- **Min SDK**: 24
- **Target / Compile SDK**: 34
- **Module**: `:app`

## Getting started

### Prerequisites

- Android Studio (recommended)
- JDK 17 (typical for Android Gradle Plugin 8.x)

### Open in Android Studio

1. Open Android Studio
2. **File → Open…** and select this repository folder
3. Let Gradle sync finish

### Build (command line)

```bash
./gradlew :app:assembleDebug
```

### Run tests

Unit tests:

```bash
./gradlew test
```

Instrumented tests (requires an emulator/device):

```bash
./gradlew connectedAndroidTest
```

## Code map

- `app/src/main/java/com/example/taskappnew/MainActivity.kt`: main task list screen
- `app/src/main/java/com/example/taskappnew/AddEditTaskActivity.kt`: add/edit screen
- `app/src/main/java/com/example/taskappnew/Task.kt`: Room entity model
- `app/src/main/java/com/example/taskappnew/TasksDao.kt`: Room DAO
- `app/src/main/java/com/example/taskappnew/TaskDatabase.kt`: Room database
- `app/src/main/java/com/example/taskappnew/TaskRepository.kt`: data layer
- `app/src/main/java/com/example/taskappnew/TaskViewModel.kt`: UI state + operations

