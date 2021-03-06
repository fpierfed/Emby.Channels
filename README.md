Emby.Channels
====================

This repository contains many of the channels managed by the Emby community.

Each of the projects has a build event that copies it's output to the programdata/plugins folder. 

By default this assumes you have the server repository side by side in a folder called 'Emby'. If this is not the case, or if you've installed the server than you'll need to update the build events manually in order to test code changes.


## Differences With Upstream Emby.CHannels

Documentation and build scripts.


## How to build (Mono)

Copy MediaBrowser.Common.dll, MediaBrowser.Model.dll and MediaBrowser.Controller.dll in the relevant places inside the packages directory (see the README.md files therein).

Then, in the Emby.Channel directory, issue
> xbuild /t:build /p:Configuration="Release" /p:Platform="Any CPU" MediaBrowser.Channels.sln


## More Information ##

[How to Build a Server Plugin](https://github.com/MediaBrowser/MediaBrowser/wiki/How-to-build-a-Server-Plugin)
