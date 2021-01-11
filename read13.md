# What Is The LocalStorage ?

> *The read-only localStorage property allows you to access a Storage object for the Document’s origin; the stored data is saved across browser sessions. localStorage is similar to sessionStorage, except that while data stored in localStorage has no expiration time, data stored in sessionStorage gets cleared when the page session ends — that is, when the page is closed. (Data in a localStorage object created in a “private browsing” or “incognito” session is cleared when the last “private” tab is closed.)*



# The main features of localStorage are:

> Shared between all tabs and windows from the same origin.

> The data does not expire. It remains after the browser restart and even OS reboot.


# Cookies :
> were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But there are three potentially dealbreaking downsides:

- included with every HTTP request, thereby slowing down our web application by needlessly transmitting the same data over and over
- limited to 4KB of data — enough to slow down our application, but not enough to be terribly useful So, you need to a lot of storage space on the client that persists beyond a page refresh and isn’t transmitted to the server




***To use localStorage in your web applications, there are five methods to choose from:***

1-setItem(): Add key and value to localStorage.

2-getItem(): Retrieve a value by the key from localStorage.

3-removeItem(): Remove an item by key from localStorage.

4-clear(): Clear all localStorage.

5-key(): Passed a number to retrieve nth key of a localStorage.


*Example:*

*The following snippet accesses the current domain’s local Storage object and adds a data item to it using Storage.setItem().*

`localStorage.setItem('myCat', 'Tom');`

*The syntax for reading the localStorage item is as follows:*

`const cat = localStorage.getItem('myCat');`

*The syntax for removing the localStorage item is as follows:*

`localStorage.removeItem('myCat');`

*The syntax for removing all the localStorage items is as follows:*

`localStorage.clear();`





# Using HTML Storage..

> HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.
