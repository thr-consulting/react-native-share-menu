# Android Installation

## Add Intent Filter

- In `android/app/src/main/AndroidManifest.xml` in the `<activity>` tag:

```xml
<activity
  ...
  android:documentLaunchMode="never">
  ...
  <intent-filter>
    <action android:name="android.intent.action.SEND" />
    <category android:name="android.intent.category.DEFAULT" />
    <data android:mimeType="text/plain" />
    <data android:mimeType="image/*" />
    <!-- Any other mime types you want to support -->
  </intent-filter>
</activity>
```
