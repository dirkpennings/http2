# HTTP/2 test website

## Description

This is a local HTTP/2 test website which uses [Google Chrome's simplehttp2server](https://github.com/GoogleChrome/simplehttp2server) to run a local server.

## Good to know

* Make sure you don't have checked "Disable cache" in DEV Tools
* As of now, the `h2` protocol only works over a HTTPS connection
* To see the response protocol in DEV Tools, right click the columns in the Network tab and enable `Protocol`
* [`Link:` header tags is NOT how you do push](https://twitter.com/dassurma/status/748616497115836416)
* [Chrome Canary](https://www.google.nl/chrome/browser/canary.html) shows a "Push" initiator when receiving pushed assets ![Chrome Canary push initiator](https://cdn-images-1.medium.com/max/800/0*a3NOiXytpFA8UrwW.)

## Installation (OS X)

* Download the corresponding binary from [their release page](https://github.com/GoogleChrome/simplehttp2server/releases)
* Open Terminal and navigate to the download folder
* Copy the binary from the download folder to the `/usr/local/bin` folder: `cp simplehttp2server_darwin_amd64 /usr/local/bin/simplehttp2server`
* Execute the command `chmod +x /usr/local/bin/simplehttp2server`
* Restart Terminal or open a new tab
* Clone this repository in the desired folder (e.g. `$HOME/Sites`) `git clone https://github.com/dirkpennings/http2`
* Navigate to the newly created folder `cd http2`
* Start your local server with `simplehttp2server` and navigate to [https://localhost:5000](https://localhost:5000) with your browser

## Installation (Windows)

* Download the corresponding binary from [their release page](https://github.com/GoogleChrome/simplehttp2server/releases)
* Rename the executable `simplehttp2server_windows_amd64.exe` to `simplehttp2server.exe`
* Move the executable to `C:\Windows\System32` (because this folder already exists in the PATH variable)
* Open the command prompt and clone this repository in the desired folder (e.g. `C:\temp`) `git clone https://github.com/dirkpennings/http2`
* Navigate to the newly created folder `cd http2`
* Start your local server with `simplehttp2server` (accept any Windows Security alerts) and navigate to [https://localhost:5000](https://localhost:5000) with your browser

### Useful links

* [HTTP/2 101 (Chrome Dev Summit 2015)](https://www.youtube.com/watch?v=r5oT_2ndjms&t=21m59s)
* [Issue 5: HTTP/2 Push](https://medium.com/totally-tooling-tears/issue-5-http-2-push-9c6eba8d6d7c#.fev9r5zo3)

### Credits

Thanks go out to [Surma](https://github.com/surma) for explaining some details about simplehttp2server