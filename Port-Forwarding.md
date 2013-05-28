YAMS features the ability to handle port forwarding for you, meaning ports are opened only when needed and closed again when not for extra security.

Port forwarding is enabled by default, but requires the following:
  * A UPnP capable router.
  * UPnP "Enhanced Security" (or similar) disabled.

## Diagnosing problems

UPnP is a flaky standard at the best of times, and many routers ship with UPnP switched off.

`Unable foward port 80 for Public website: Exception - Object reference not set to an instance of an object.`

If you see an error message in the [[global log]] like the above, YAMS has been unable to find a UPnP router to talk to, make sure you have UPnP enabled in your router config (just Google your router model and UPnP).
