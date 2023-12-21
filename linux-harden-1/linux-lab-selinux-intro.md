## SELinux basic introduction

- Go to root shell
- Install httpd (webserver)
- Start webserver process
- Check context types, they allow different access, look at -Z argument
- Check context on processes too
- Check on network socket too
- Set the httpd server to listen on 8088 and restart
- Look at SELinux enforcement
- Set SELinux to permissive mode
- Try to restart your web server
- Look at audit log
- Revert the enforcement mode, restart the webserver, check journalctl
- Check /var/log/message for SELinux alert
- Look at the sealert
- Authorize port 8088 binding and restart daemon
- Install setools
