# connect
Microsoft Visual Studio 2017 compilable version of connect (used in the
connect-proxy debian package) as taken from [here](https://bitbucket.org/gotoh/connect/wiki/Home).

Open the solution, build the single file, copy Release/connect.exe to
somewhere on your path (I use git-bash's ~/bin/).

```bash
$ connect
connect --- simple relaying command via proxy.
Version 1.105
usage: C:\Program Files\Git\usr\bin\connect.exe [-dnhst45] [-p local-port]
          [-H [user[:pass]@]proxy-server[:port]] [-S [user[:pass]@]socks-server[:port]]
          [-T [user[:pass]@]proxy-server[:port]]
          [-c telnet-proxy-command]
          host port
```

Also added the common function to be able to pass password on command line:

```bash
$ connect -H user:pass@host:port someserver.com 12345
```
