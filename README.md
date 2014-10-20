# munin-kue

Munin plugin to monitor kue. Written in perl.

## about

At the moment, the plugins parses the json api. You must enable the web interface of kue for this plugin to work.

This is a work in progress, at a very early stage.

A plugin that reads information out of redis might be written some day.

Feel free to contribute.

## options

name  | default value
----- | -------------
host  | 127.0.0.1
port  | 3000
