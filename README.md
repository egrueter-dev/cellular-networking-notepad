# Cellular Networking Notepad

Notepad to collect research on React Native, cellular networking and developing apps for low resource settings.


### Android Networking Documentation:
[Android Connectivity Manager](https://developer.android.com/reference/android/net/ConnectivityManager)

Answers queries about the state of network connectivity. It also notifies applications when network connectivity changes.

[NetworkRequest Object](https://developer.android.com/reference/android/net/NetworkRequest)

Defines a request for a network, made through NetworkRequest.Builder and used to request a network via ConnectivityManager.requestNetwork(NetworkRequest, PendingIntent) or listen for changes via ConnectivityManager.registerNetworkCallback(NetworkRequest, PendingIntent).

Example:

```java
  NetworkRequest.Builder req = new NetworkRequest.Builder();
  req.addTransportType(NetworkCapabilities.TRANSPORT_CELLULAR);
```


### Valuable Stack Overflow Questions:

[How to stay connected through mobile network after WIFI is connected on Android](https://stackoverflow.com/questions/29835240/how-to-stay-connected-through-mobile-network-after-wifi-is-connected-on-android/29837637#29837637)


