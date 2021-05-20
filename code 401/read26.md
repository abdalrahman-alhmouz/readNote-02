## Android fundamentals

- Android SDK tools compile your code along with any data and resource files into an APK, an Andoid package which is an archive file with an .apk suffix. 
- Each Android app lives in its own security sandbox protected...
  -  Android operating system multi-user Linux system in which each app is a diff user
  - System assigns each app a unique Linux user ID, used only by the system and unknown to the app.
  - Each process has its own virtual machine so an apps code runs in isolation from other apps.
- Each app by default has access only to the compnents that it requires to do its work and no more.

### App components
- each component is an entry point through which the system or a user can enter your app. Some depend on others
- Four types
  - Activities
  - Services 
  - Broadcast receivers
  - Content providers

#### Activities
- entry point for interacting with the user, a single screen with a user interface. 
- can work together to form cohesive user experience but each one is independent of the others
- you implement an activity as a subclass of the `Actiity` class. 

#### Services
- entry point for keeping an app running in the background. 
- Doesn't provide a user interface.
- implemented as a subclass of `Service`

#### Braodcast receivers
- enables the system to deliver events to the app outside of a regular user flow
- example an app can schedule an alarm to post a notification to tell the user about an upcoming event. 
- they don't get a user interface but can create a status bas notification to alert the user.
- implemented as a subclass of `BroadcastReceiver` and ech broadcast is delivered as an `Intent` object.

#### Content providers
- shared set of app data that you can store in the file system, in a SQLite database, on the web or on any other persistent storage location that your app can access.
implemented as a subclass of `ContentProvider` and must implement a standard set of APIs that enable other apps to perform transactions.
- there's no `main()` function with Android apps

#### Activating components
- 3 of 4 component types, activities, services and broadcast receivers are activiated by an asynchronous message called an `Intent` 
- activities and services and intent defines the action to perform
- broadcast receivers the intent simply defines the announcement being broadcast.
- content providers are not activated by intents. Rather they are activated when targeted by a request from a `ContentResolver`

#### The manifest file
- `AndroidMaifest.xml` system must know that the component exists by reading the apps manifest file. Must declare all its components in this file which must be at the root of the app project directory.
- identifies any user permssions the app requires
- declares the min API Level required by the app
- declares hardware and software features used or required by the app
- declares API libraries the app needs to be linked against

#### Declaring components
- primary task of the maifest is to inform the system about the app's componenets
- `<application>` element, the `android:icon` attribute points to resources for an icon that identifies the app
- `<activity>` element, the `android:name` attribute apecifies the fully qualified class name of the `Activity   subclass
- `android:label` attribute specifies a string to use as the user-visible label for the activity

You must declare all app components using the following elements:

- `<activity>` elements for activities.
- `<service>` elements for services.
- `<receiver>` elements for broadcast receivers.
- `<provider>` elements for content providers.

#### Declaring component capabilities
- `Intent` to start activities, services and broadcast receivers

#### Declaring app requirements
- clearly define a profile for the eypes of devices your app supports by declaring device and software requirements in your manifest file.

#### App resources
- requires resources that are separate from the source code, ie. images, audio files, anything relating to the visual presentation of the app.
- makes it easy to update various characteristics without modifying code.
- SDK build tools define a unique integer ID which you can use to referenece the resources from your app code.
- qualifier is a short string that you include in the name of your resource directories in order to define the device config.
- diff layouts depending on screen orientation and size

![app](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQxVBsMyw9slexx43CCXPTA9NzEDakf_3aSeg&usqp=CAU)
