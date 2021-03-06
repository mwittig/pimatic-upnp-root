# pimatic-upnp-root

[![npm version](https://badge.fury.io/js/pimatic-upnp-root.svg)](http://badge.fury.io/js/pimatic-upnp-root)

Pimatic UPnP Root-Device to advertise the Pimatic web interface on the Local Network. For example, this may be useful 
 for Windows users as the Pimatic device will show in the network view. Double-clicking the device will open
 the web interface using the default web browser.
 
![Network View](https://raw.githubusercontent.com/mwittig/pimatic-upnp-root/master/screenshots/screenshot-2.png)

## Configuration

You can load the plugin by editing your `config.json` to include the following in the `plugins` section. The property `
 presentationURL` specifies the URL of the pimatic web interface. If not set, a fallback will bet set. The property 
'friendlyName' set the friendly name of the device. It is set to "Pimatic Smart Home" by default. The property 
 'port' refers to the listener port of the UPnP peer to let other devices query the UPnP device description. The port is
 set to 8008 by default. Note, on first startup the plugin creates an unique identifier which will be stored as part
 of the configuration. A 'uuid' property will be added to the configuration file.

    { 
       "plugin": "upnp-root",
       "presentationURL": "http://raspberrypi.fritz.box",
       "friendlyName": "Pimatic Smart Home",
       "port": 8008
    }

## History

See [GitHub Releases](https://github.com/mwittig/pimatic-upnp-root/releases).

## License

Copyright (c) 2018, Marcus Wittig and contributors

All rights reserved.

[GPL-2.0](https://github.com/mwittig/pimatic-upnp-root/blob/master/LICENSE).