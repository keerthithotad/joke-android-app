# joke-android-app
 We’ll create a STARTED service We’re going to create a new project that contains an activity called MainActivity, and a started service called DelayedMessageService. Whenever MainActivity calls DelayedMessageService, it will wait for 10 seconds and then display a piece of text.
 
 # Display the message in Android’s log.
 
 We’ll start by displaying the message in Android’s log so that we can check
that the service works OK. We can look at the log in Android Studio.
 
 1 Display the message in a notification.
We’ll get DelayedMessageService to use Android’s built-in
notification service to display the message in a notification. 
# What happens when you run the app
Here’s what the code does when we run the app:
Let’s take the app for a test drive so we can see it working.
DelayedMessageService
Some text. I know
how to handle that.
1...2...3...4...5...
MainActivity starts DelayedMessageService by calling startService()
and passing it an intent.
The intent contains the message MainActivity wants
DelayedMessageService to display, in this case “Timing!”.
When DelayedMessageService receives the intent, its onHandleIntent()
method runs.
DelayedMessageService waits for 10 seconds
DelayedMessageService logs the message.
When DelayedMessageService has finished running, it’s destroyed.
Test drive the app
When you run the app, MainActivity is displayed. 
