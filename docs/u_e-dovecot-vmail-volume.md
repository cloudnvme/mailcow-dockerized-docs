If you want to use another folder for the vmail-volume, you can create an `docker-compose.override.yml` file and add:
```
version: '2.1'
volumes:
  vmail-vol-1:
    driver_opts:
      type: none
      device: /data/mailcow/vmail
      o: bind
```
