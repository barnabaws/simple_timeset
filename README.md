# simple_timeset
One line command to set correct time. Command sends GET HTTP request to online server, then strips the time from 'Date' header. 
Useful in systems without RTC hardware such as Raspberry PI. It does not provide such precision as NTP, but, it should be good enough for majority of applications. There is no special requirements regarding system (curl package) and network (HTTP/S query).

It's handy to add this line to '/etc/rc.local', so the time is set correctly just after boot.
