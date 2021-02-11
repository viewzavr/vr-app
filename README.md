# vr-app-template
A template for running your new Viewzavr app / package. It uses [Viewzavr system A](https://github.com/viewzavr/viewzavr-system-a).

# Usage

Use this repo as a `template`, and place your code into `app.js` file.

# Running

## Option 1 - proxy based, experimental
You may use [viewzavr-hosted player](http://viewlang.ru/viewzavr-apps/viewzavr-system-a/player/) and you may try it's proxiing ability to load github resources.
Example:
http://viewlang.ru/viewzavr-apps/viewzavr-system-a/player/?src=https://github.com/viewzavr/vr-app-template/blob/main/app.js

You do not need your server for this option. You may delete provided html files freely.

This option has a drawback - time to time the proxy hangs.

## Option 2 - cloud based
You may use [viewzavr-hosted player](http://viewlang.ru/viewzavr-apps/viewzavr-system-a/player/) and you may use https://www.jsdelivr.com to load your app. For example, current app may be loaded in a such way:
* http://viewlang.ru/viewzavr-apps/viewzavr-system-a/player/?src=https://cdn.jsdelivr.net/gh/viewzavr/vr-app-template@main/app.js

You do not need your server for this option. You may delete provided html files freely.

This option has a drawback - jsdelivr.com caches files, so you have to change `@main` tag in url to most recent commits.

## Option 3 - own server for app.js
To run your app, use viewzavr-hosted player:
* http://viewlang.ru/viewzavr-apps/viewzavr-system-a/player/?src=path-to-your-app.js

This option allows easier app.js update. You have to configure CORS headers on your server.

## Option 4 - own server for html and app.js
Use `index-viewzavr-remote.html` as a template. This file uses viewzavr codes hosted on viewzavr server.

This option gives you control over html. You do not need to configure CORS.

## Option 5 - 100% own
Use `index-viewzavr-own.html` as a template. Before using it, add viewzavr as a submodule to your project:
```
git submodule add git@github.com/viewzavr/viewzavr-system-a
```

This option gives you full control over everything, but requires you to update viewzavr system time to time.

## license

2021+ (c) Pavel Vasev. This template is available with MIT license. Your app license is up to you.
