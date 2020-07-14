# One Liners

This is simply a random assortment of useful one line commands that I use grequently.

## Mounting Shared Folders for VMWare

```bash
sudo vmhgfs-fuse .host:/ /mnt/ -o subtype=vmhgfs-fuse,allow_other
``` 

## Spoofing a Webserver with Socat
Have a xss vulnerability and need a place to make requests to? Sure you could set up a python webserver, but if you simply need to catch requests and display them then socat is a better solution.

```bash
sudo socat TCP-LISTEN:80,reuseaddr,fork -
```

