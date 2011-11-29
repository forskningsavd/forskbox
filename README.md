## Use pre-built box

You can download a pre-built box manually, verify that the md5 sum corresponds to this document and add it to Vagrant (`vagrant box add 'forskbox' 'forskbox.box'`). Another alternative is to just run `vagrant up` in a project which already includes the url to the box.

## Build your own box

* Install [VeeWee](https://github.com/jedi4ever/veewee).
* Build: `vagrant basebox build 'forskbox'`
* Validate box: `vagrant basebox validate 'forskbox'`
* Export .box file: `vagrant basebox export 'forskbox'`
* *(Optional)* Upload to `http://files.forskningsavd.se/boxes/forskbox.box` and update the md5 sums in this document.
* Install it to your Vagrant setup: `vagrant box add 'forskbox' 'forskbox.box'`
* *(Optional)* You can now delete the temporary files to save space: `rm forskbox.box; rm -rf iso/`

## Current boxes and md5 sums

    http://files.forskningsavd.se/boxes/
        forskbox.box: b8781b5a60d4a03b853cdc8d33a0fc05
