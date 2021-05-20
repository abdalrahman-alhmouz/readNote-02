## Android Tasks and the Back Stack
- task is a stack of activities
- Back button activity finished and popped off the stack
- apps running simultaneously in a multi windowed environment the system manages tasks separately for each window.
- Home screen is the starting place for most tasks. 
- when current activity starts another the new activity is pushed on the top of the stack and takes focus. previous remains but is stopped. 
- back stack operates as a LIFO object structure
- Task is a cohesive unit that can move to the "background" when users begin a new task or go to the Home screen via the Home button.
- A task can then return to the "foreground" so users can puck up where they left off.
- Activities can be instantiated multiple times even from other tasks
- Defining launch modes with manifest file or Intent flags
- 4 launchMode attributes
  - "standard": default, can be instantiated multiple times, can belong to fidderent taks and one taks can have multiple instances
  - "singleTop": instance os the activity already exists at the top of the current task the system routes the intent to that instance through a call to its `onNewIntent()` method
  - "singleTask": creates new task and instantiates the activity at the root of the new task. If already exists in a separate task the system routes the intent to the existing instance through a call to its `onNewIntent()`
  - "singleInstance": same as "singleTask" except the system doesn't launch any other activities into the task holding the instance

  - Using Intent flags
    - `FLAG_ACTIVITY_NEW_TASK`: start activity in a new task. If a task is already running for the activity you are not starting that task is brought to the foreground with its last state restored and the activity receives the new intent in `onNewIntent()`
    - `FLAG_ACTIVITY_SINGLE_TOP`: If the activity being started is the current activity (at the top of the back stack), then the existing instance receives a call to `onNewIntent()`, instead of creating a new instance of the activity.

- Clearing the back stack
  - If the user leaves a task for a long time, the system clears the task of all activities except the root activity. When the user returns to the task again, only the root activity is restored

## Android SharedPreferences
- `getSharedPreferences()` — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.
- `getPreferences()` — Use this from an Activity if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.
- When naming your shared preference files, you should use a name that's uniquely identifiable to your app. An easy way to do this is prefix the file name with your application ID. For example: `"com.example.myapp.PREFERENCE_FILE_KEY"`
- To write to a shared preferences file, create a `SharedPreferences`.Editor by calling `edit()` on your `SharedPreferences`.
- To retrieve values from a shared preferences file, call methods such as `getInt()` and `getString()`, providing the key for the value you want, and optionally a default value to return if the key isn't present. 
