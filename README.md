# Live Server
**_[If you found any bug or if you have any suggestion, feel free to report or suggest me. If you like the extension, don't forgot to rate it.]_**

[![VSCode Marketplace Badge](https://vsmarketplacebadge.apphb.com/version/ritwickdey.LiveServer.svg)](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) [![Total Install Count Badge](https://vsmarketplacebadge.apphb.com/installs/ritwickdey.LiveServer.svg)](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) [![Avarage Rating Badge](https://vsmarketplacebadge.apphb.com/rating-short/ritwickdey.LiveServer.svg)](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ritwickdey/vscode-live-server/)
<br>
Launch a development local server directly from VSCode to your browser and watch live preview of HTML<br>
![App Preview](./images/Screenshot/AnimatedPreview.gif)


## Usage/Shortcuts

**_[In case if you don't have any `.html` file in your workspace then you have to follow method no 3 & 4 to start Live Server. I don't know why you want so?! :p But feature is still there.]_**

1. Open a HTML File/Project and directly Click to `Go Live` from StatusBar to turn off/on the server. 
![Go Live Control Preview](./images/Screenshot/statusbar2.jpg)

2. Open a HTML file and Right click on the editor and choose the options.
![Edit Menu Option Preview](./images/Screenshot/editormenu2.jpg)

3. Hit `(alt+L, O)` to Open the Server and `(alt+L, C)` to close the server. 

4. Press `F1` or `ctrl+shift+P` and type `Live Server: Open Live Server ` to start a server or type `Live Server: Close Live Server` to stop a server.

## Features
* A Quick Development Live Server.
* Live Reload on change of HTML files.
* Run the live server from status bar.
* Quick Statusbar control.
* Customizable Port Number.
* Customizable Server Root.
* Customizable default browser.
* Support for Chrome Debugging Attachment (_[More Info](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)_). [[Quick Gif Demo](./images/Screenshot/ChromeDebugging.gif)].
* Support for any browser (Eg: Chrome Canary, Firefox Nightly) using advance Command Line.

## Settings
* **`liveServer.settings.port` :** Customize Port Number of your Live Server.  If you want random port number, set it as `0`.
    *  _Default value is `5500`._

* **`liveServer.settings.root` :** To change root of server in between workspace folder structure,  use `/` and absolute path from workspace.
    * _Example: `/sub_folder1/sub_folder2`_. Now `sub_folder2` will be root of the server.
    *  _Default value is "`/`".(The Workspace Root)_.

* **`liveServer.settings.CustomBrowser` :** To change your system's default browser. (_chrome_ or _firefox_ or _Microsoft-Edge_).
    * _Default value is `Null`. (It will open your system's default browser.)_

* **`liveServer.settings.ChromeDebuggingAttachment` :** To Enable Chrome Debugging Attachment to Live Server. [[Quick Gif Demo](./images/Screenshot/ChromeDebugging.gif)].
    * _**NOTE**: You must have to install [ `Debugger for Chrome.`](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)_
    * _If the value is `true`, Start Live Server and select 'Attach to Chrome' from Debug Window to start debugging. [`Debugger for Chrome`](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome) Extension will inject debugging feature into running instance of browser window._
    *  _Default value is `false`._
* **`liveServer.settings.AdvanceCustomBrowserCmdLine` :**  To set your any favorite browser (Eg: Chrome Canary, Firefox Nightly) using advance Command Line. 
    * _This setting will override `CustomBrowser` and `ChromeDebuggingAttachment` settings._
    * _Examples:_
        * _chrome --incognito_
        * _chromecan --remote-debugging-port=9222_
        * _chrome --headless_
        * _chrome --incognito --remote-debugging-port=9222_

## Installation
Open VSCode Editor and Press `ctrl+P`, type `ext install LiveServer`.

## What's new ?

#### Version 1.6.0 (19.07.2017)

* [[#5](https://github.com/ritwickdey/vscode-live-server/issues/5)] New Settings - `liveServer.settings.AdvanceCustomBrowserCmdLine` - Now set your any favorite browser (Eg: Chrome Canary, Firefox Nightly) for Live Server using advance Command Line. (_[More Info.](https://github.com/ritwickdey/vscode-live-server#settings)_) [Thanks [Obinna A. Kalu](https://github.com/obkalu)].

*  Support for Microsoft-Edge through `liveServer.settings.CustomBrowser` settings.

#### Version 1.5.0 (17.07.2017)
* [[Quick Gif Demo](./images/Screenshot/ChromeDebugging.gif)] New Feature Added - Support for Chrome Debugging Attachment. (You have to enable the feature through `liveServer.settings.ChromeDebuggingAttachment` settings. _[More Info.](https://github.com/ritwickdey/vscode-live-server#settings)_).  [Thanks [Obinna A. Kalu](https://github.com/obkalu) [[#5](https://github.com/ritwickdey/vscode-live-server/issues/5)] ].

#### Version 1.4.3 (10.07.2017)
* Status-bar Icon added. Minor Fix update on Status bar control. 

## Changelog
To check full changelog click here [changelog](CHANGELOG.md).

## LICENSE

This extension is licensed under the [MIT License](LICENSE)