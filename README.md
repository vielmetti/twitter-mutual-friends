"Twitter mutual friends" was a set of tools (or perhaps simply documentation for API calls) 
that showed how to match up two users friends and see what the stream is of their overlapping feeds.

You should now use http://mike.verdone.ca/twitter/ and http://github.com/sixohsix/twitter to get this done,
and this project is closed. 

> Python Twitter Tools (PTT) includes a Twitter API, command-line tool, and IRC bot. It is developed by Mike Verdone and the Python Twitter Tools developer team.

```
#!/bin/sh
( twitter-follow -o -r $1
  twitter-follow -o -r $2 ) |
sort | uniq -d
```
