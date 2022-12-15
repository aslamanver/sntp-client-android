### SNTPClient for Android
Simple SNTP Client class for retrieving network time on Android (SNTPClient)

<img width="250" src="https://i.imgur.com/y9AODqW.png" />

#### Copy-Paste
Copy the `SNTPClient.java` into your project, there you go. It's ready.

#### Usage

1. Retrieve the time of a specific time zone.

```java
SNTPClient.getDate(TimeZone.getTimeZone("Asia/Colombo"), new SNTPClient.Listener() {

    @Override
    public void onTimeResponse(String rawDate, Date date, Exception ex) {

    }
});
```
<hr>

2. Current time zone can be passed to retrive current time of the device zone.
```java
Calendar.getInstance().getTimeZone();
```

#### About more

* The output time is formatted according to <a href="https://en.wikipedia.org/wiki/ISO_8601">ISO 8601</a> format.
> yyyy-MM-dd'T'HH:mm:ssZ

* Time server host is Google
> time.google.com
