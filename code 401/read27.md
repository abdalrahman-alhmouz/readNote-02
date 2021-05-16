### Task Is : 
* A Collection of Activities That Users Interact With When Performing A Certain Job. The Activities are Arranged in a stack-the back stack) -in The Order in Which Each Activity is opened.

* When apps are running simultaneously in a multi-windowed environment, supported in Android 7.0 (API level 24) and higher, the system manages tasks separately for each window; each window may have multiple tasks. The same holds true for Android apps running on Chromebooks: the system manages tasks, or groups of tasks, on a per-window basis.

The device Home screen is the starting place for most tasks. When the user touches an icon in the app launcher (or a shortcut on the Home screen), that app's task comes to the foreground. If no task exists for the app (the app has not been used recently), then a new task is created and the "main" activity for that app opens as the root activity in the stack.

When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. When an activity stops, the system retains the current state of its user interface. When the user presses the Back button, the current activity is popped from the top of the stack (the activity is destroyed) and the previous activity resumes (the previous state of its UI is restored). Activities in the stack are never rearranged, only pushed and popped from the stack—pushed onto the stack when started by the current activity and popped off when the user leaves it using the Back button. As such, the back stack operates as a "last in, first out" object structure. Figure 1 visualizes this behavior with a timeline showing the progress between activities along with the current back stack at each point in time.
 
 ![app](https://developer.android.com/images/fundamentals/diagram_backstack.png)
 
  
 ### launch modes :
 Launch modes allow you to define how a new instance of an activity is associated with the current task. You can define different launch modes in two ways:

1 - Using the manifest file
When you declare an activity in your manifest file, you can specify how the activity should associate with tasks when it starts.

2- Using Intent flags
When you call startActivity(), you can include a flag in the Intent that declares how (or whether) the new activity should associate with the current task.

 #### Save key-value data : 
  * If you have a relatively small collection of key-values that you'd like to save, you should use the SharedPreferences APIs. A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them. Each SharedPreferences file is managed by the framework and can be private or shared.

* Get a handle to shared preferences 
*   1 -getSharedPreferences() — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.
 2 - getPreferences() — Use this from an Activity if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.

