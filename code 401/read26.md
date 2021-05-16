### Application Fundamentals :
Android applications are composed of one or more application components (activities, services, content providers, and broadcast receivers) Each component performs a different role in the overall application behavior, and each one can be activated individually (even by other applications)
* Android apps can be written using Kotlin, Java, and C++ languages. The Android SDK tools compile your code along with any data and resource files into an APK, an Android package, which is an archive file with an .apk suffix. One APK file contains all the contents of an Android app and is the file that Android-powered devices use to install the app.


#### App components :

![app](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQxVBsMyw9slexx43CCXPTA9NzEDakf_3aSeg&usqp=CAU)
* compoenents are building block of android application.
there are four types of components.
- Activities
 - Services
 - Broadcast receivers
 - Content providers
 - Activities
 * activities are interface with entry point that interact with user.
activity can be like read list od data., it can also be doing some other task like for example creating data.
together they form the application.

entry point for keeping an app running in the background.
service does not provide a user interface, which means it might run something in the background while user doing something else.
service might fetch data over the network
Broadcast receivers
component that enables the system to deliver events to the app outside of a regular user flow.
broadcast receivers are another well-defined entry into the app.
Content providers
it manage a shared set of app data that you can store in the file system.
 ### Activating components :
activities, services, and broadcast receivers are activated by an asynchronous message called an intent.
Intents bind components to each other at runtime.
Intent object create a message to activate a component or a specific type of component.
activity and service define the action to do.
content providers are not activated by intents.
they are activated when targeted by a request from a ContentResolver.
 ### The manifest file
 - android system know if component file exit from manfiest file when system read it.
app must declare all its components in this file.
things manifest does in addition to declaring the app's components:
Identifies user permissions the app require.
Declares the minimum API Level required by the app.
Declares hardware and software features used or required by the app such as camera.
Declares API libraries the app needs to be linked against.
