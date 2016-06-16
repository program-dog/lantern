Here is a server version running on linux without desktop. So there is no this error[#3447](https://github.com/getlantern/lantern/issues/3447) : 

```
error while loading shared libraries: libappindicator3.so.1: cannot open shared object file: No such file or directory
```
Here are the binary files:

[lantern_linux_386_server](https://github.com/program-dog/lantern/blob/server/lantern-server/lantern_linux_386_server)<br>
[lantern_linux_amd64_server](https://github.com/program-dog/lantern/blob/server/lantern-server/lantern_linux_amd64_server)

To run, maybe you should do this:

```bash
chmod a+x lantern_linux_386_server
chmod a+x lantern_linux_amd64_server
```
and then,

```
./lantern_linux_386_server  --addr 127.0.0.1:8787  2>lantern_error.log 
./lantern_linux_amd64_server  --addr 127.0.0.1:8787 2>lantern_error.log 
```
