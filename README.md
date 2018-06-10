# Cellular Networking Notepad

Notepad to collect research on React Native, cellular networking and developing apps for low resource settings. 

The business cases where wifi is not available and data is scarce are underserved. Organizations operating in these settings (working in refugee camps, for example) need to transfer data over whatever scarce network resources are available. 


### Android Networking Documentation:

[Android Connectivity Manager](https://developer.android.com/reference/android/net/ConnectivityManager)

Answers queries about the state of network connectivity. It also notifies applications when network connectivity changes.

[NetworkRequest Object](https://developer.android.com/reference/android/net/NetworkRequest)

Defines a request for a network, made through NetworkRequest.Builder and used to request a network via:

```java 
  ConnectivityManager.requestNetwork(NetworkRequest, PendingIntent)
``` 

or listen for changes via:

```java 
  ConnectivityManager.registerNetworkCallback(NetworkRequest, PendingIntent).
```

Example:

```java
  NetworkRequest.Builder req = new NetworkRequest.Builder();
  req.addTransportType(NetworkCapabilities.TRANSPORT_CELLULAR);
```

### Valuable Stack Overflow Questions:

[How to stay connected through mobile network after WIFI is connected on Android](https://stackoverflow.com/questions/29835240/how-to-stay-connected-through-mobile-network-after-wifi-is-connected-on-android/29837637#29837637)


### Integrating Native Modules into React Native 

* [Native Android Modules in React](https://facebook.github.io/react-native/docs/native-modules-android.html)
* [Basic React native file structure direction that Facebook hipster dickheads didnt put in React Native docs](https://www.reactnative.guide/16-custom-native-modules/16.1-android-native-module.html)
