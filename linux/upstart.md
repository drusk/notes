# Don't automatically start a service

Useful for things like MongoDB, which you might not want to start
automatically on your development machine.

Services managed with Upstart are configured by a file such as
`/etc/init/mongod.conf`. To disable automatic startup:

```
echo "manual" > /etc/init/mongod.override
```

