# cordova-plugin-allow-notifications

Android 13 (API level 33) and higher supports a runtime permission for sending non-exempt (including Foreground Services (FGS)) notifications from an app: POST_NOTIFICATIONS. This change helps users focus on the notifications that are most important to them.

To request the new notification permission from your app, update your app to target Android 13 and complete a similar process compared to requesting other runtime permissions, as shown in the following sections.

The permission that you need to declare in your app's manifest file appears in the following code snippet:

<uses-permission android:name="android.permission.POST_NOTIFICATIONS"/>

More info on https://developer.android.com/develop/ui/views/notifications/notification-permission
