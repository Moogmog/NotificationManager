# NotificationManager
NotificationManager for Android Java

## How to use?
1. Set Group name
   <pre><code>NotificationManager.setGroupName("This is my Group.");</code></pre>

2. Create Notificaton Channel
   <pre><code>NotificationManager.createChannel(getApplicationContext(), "Channel Name", "Channal Description");</code></pre>
   
3. Make Notification
   ``` java
   NotificationManager.showNormalNotification(getApplicationContext(), 1, "Title", "Normal Notification");</code></pre>

   Or
   
   <pre><code>String[] box = new String[6];
   box[0] = "One";
   box[1] = "Two";
   box[2] = "Three";
   box[3] = "Four";
   box[4] = "Five";
   box[5] = "Six";
   NotificationManager.showInboxStyleNotification(getApplicationContext(), 2, "Title", "InBoxStyle Notification", box);
   ```
   
<hr/>

## All Methods
``` java
@void setGroupName(String name)
@void showNormalNotification(Context context, int id, String title, String content)
@void showInboxStyleNotification(Context context, int id, String title, String content, String[] boxText)
@void deleteNotification(Context context, int id)
@int getSmallIcon()
```
