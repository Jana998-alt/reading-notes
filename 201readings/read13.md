# Read: 13 - Local Storage

local storage has been a challenge for web sites since their beginning. Unlike desktop applications, the storage available for websites was a few kilobytes, that extended to some tens of kilobytes with some solutions. 
There have been many attempts to solve this problem from many big companies. With some plugins or browser’s solutions. 
Presenting HTML5, was a big leap for this problem. According to: http://diveinto.html5doctor.com/storage.html , HTML5 storage is a way for web pages to store named key/value pairs locally, within the client web browser. 
It is supported by the latest version of ALL browsers. But for older versions, you need to check if it is supported or not, using this code: 

``` 
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
``` 

## using HTML5 storage
Remember it is a set of key-value pairs, meaning that to get the value you can use the key. 
You should know that very thing is used as a string, but can always be transformed to other data types through functions. 

```
interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};
``` 
