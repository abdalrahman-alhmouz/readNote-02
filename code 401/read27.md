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

