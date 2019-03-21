## Regex Filters for Pi-hole
This is a custom `regex.list` file for use with Pi-hole v4+ (FTLDNS).

All commands will need to be entered via Terminal (PuTTY or your SSH client of choice) after logging in.

### Install
1. `sudo vim /etc/pihole/regex.list` and paste in [regex.list](./regex.list)
2. `sudo service pihole-FTL restart`

### Testing the regex filter
See if you can access https://ad.pi-hole.net/

Then check the query log in the Pi-hole admin console for your blocked domain. It should show as **Pi-holed (wildcard)**.

![alt test](https://image.ibb.co/j5kWTz/Blocked.png)
