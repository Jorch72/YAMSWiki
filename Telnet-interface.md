**NB:** The telnet interface will be disabled by default, to enable go to Settings > Network Settings and tick the box for Telnet.  You will need to restart YAMS for this to be applied.

The telnet interface allows you to control all servers directly through your favourite terminal client, which can provide a faster method of issuing commands and long sequences of commands as there is no delay waiting for the web interface to poll.

To use, start up your telnet client of choice (`start > run > telnet` or [Putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/)) and enter your server's IP or DNS name, with the port as set in network settings (default 56553).  You will be greeted with a password prompt:

![Telnet welcome screen](http://yams.in/assets/images/docs/telnet-welcome.png)

Enter your password, being careful to make sure you are not watched as it is displayed in clear text, and press enter.  You should now see a list of servers and available commands:

![Telnet welcome screen](http://yams.in/assets/images/docs/telnet-opened.png)

Select the server you wish to operate on by typing e.g. `server 1`.  YAMS will now stream any output to your terminal, test it by issuing the `help` command.