![YAMS global log](http://yams.in/assets/images/docs/global-log.png)

The Global log records any event or notification that is not related to a specific server such as:
  * Update notifications
  * Application runs
  * Networking information ([[port forwarding]] and [[firewall]] opening)
  * Backups

Whilst the information in this log is important, most of it shouldn't impact on your server's normal operation.  All log lines have the following format:

    [<DATE> <TIME>] (<SOURCE>) <MESSAGE>

**SOURCE** helps you classify the messages and troubleshoot any issue may have.  E.g. if no-one from outside can connect check for messages tagged `networking`

Messages are colour coded as follows:

  * **Grey** - Informational
  * **Yellow** - Non-critical warning
  * **Red** - Error

`updater` messages are usually transient and related to the provider's websites being unavailable or changing their links and will usually be fixed on their own or by the [[automatic update]] grabbing a new URL for the application.