# deb2tgz
Shell script that converts Debian packages to Slackware packages.

It added support to other formats to the shell script deb2tgz that exists in https://code.google.com/archive/p/deb2tgz/

## Support to zst format - issue 1
As suggested by @sevens [sevens repo](https://github.com/sevens/deb2tgz) in commits [sevens@9a99096](https://github.com/sevens/deb2tgz/commit/9a990965577c286a268ac982172cc502564c155f) and [sevens@9829fbf](https://github.com/sevens/deb2tgz/commit/9829fbf1309439b96dfa9f93a79c486491daabbf) code based on his suggestions were added. 

Check [issue 1](https://github.com/vborrego/deb2tgz/issues/1)

Test issue 1
 * Download http://security.ubuntu.com/ubuntu/pool/main/l/less/less_590-1ubuntu0.22.04.1_amd64.deb
 * run ```./deb2tgz less_590-1ubuntu0.22.04.1_amd64.deb ```
 * Check txz contents
```sh
tar tvJf less_590-1ubuntu0.22.04.1_amd64.txz 
```

Test deb file with xz in it
 * Download http://mirrors.kernel.org/ubuntu/pool/main/l/less/less_487-0.1_amd64.deb
 * run ```./deb2tgz less_487-0.1_amd64.deb ```
 * Check txz contents
```sh
tar tvJf less_487-0.1_amd64.txz 
```
