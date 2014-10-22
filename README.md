# munin-kue

Munin plugin to monitor kue. Written in perl.

## about

At the moment, the plugins parses the json api. You must enable the web interface of kue for this plugin to work.

This is a work in progress, at a very early stage.

A plugin that reads information out of redis might be written some day.

Feel free to contribute.

## installation

On Debian :

 - put the plugin in `/usr/share/munin/plugins/`
 - create two symlinks to the plugin, named `kue_worktime` and `kue_common` in `/etc/munin/plugins/`.
 - see the [`options`](#options) section to configure the plugin to match your setup
 - restart munin-node

## options

name  | default value
----- | -------------
host  | 127.0.0.1
port  | 3000

If you need to change those values, you can override them by adding those lines to `/etc/munin/plugin-conf.d/munin-node` (on Debian) :
```
[kue_*]
env.host 192.168.0.1
env.port 5678
```
