# Isango
### MyBB Simple Social Login / Registration Plugin Using OAuth2
---

## Compatibility
- MyBB 1.8.x
- PHP 7.1+

## Implemented Features
- Users can login / register through several social gateways in a click
- Currently supported: Discord, Facebook, Github, Google, LinkedIn, Microsoft, Yandex. New services will be added to the plugin over time; however (advanced) users can easily implement other services by creating configuration `.ini` of the expected service in required pattern (no programming needed). Once a configuration file is created and placed inside `inc/plugins/isango` folder only re-anabling the plugin will activate the new service with the plugin.
- Administrators can choose the usergroup from ACP Plugin Settings under which the new users will be registered and placed, defaults to `Registered` (gid 2).
- Users can add the authentication connections from user control panel which will help them logging in using the already registered services.

## Planned features so far
- Optional ability to allow new users to input desired username while registering with Isango. Currently the plugin attempts to decide a suitable username based on available data received from the used service.
- Ability to send automated welcome private message to the newly registered user intimating the random password used to register the account.
- Adding more services to the plugin

## Installation
- Exactly same like any other plugins. Users need to upload the files inside `upload` folder of the package maintaining the already made structure using any FTP / WebDav and install / activate the plugin from ACP.
- Users need to create App for the website at the service provider's developer site to obtain App ID / Secret which are required to input through MyBB ACP Plugin settings. For detail guidelines on creating App for individual service providers please refer [Wiki](https://github.com/mybbgroup/isango/wiki).

## External Dependency:
No external OAuth library has been used in this plugin. It has been implemented complying minimum possible OAuth2 requirements.
