# HTTP/2 test website

## Description

This is a local HTTP/2 test website which uses [Google Chrome's simplehttp2server](https://github.com/GoogleChrome/simplehttp2server) to run a local server.

## Good to know

* Make sure you don't have checked "Disable cache" in DEV Tools
* As of now, the `h2` protocol only works over a HTTPS connection
* To see the response protocol in DEV Tools, right click the columns in the Network tab and enable `Protocol`
* [`Link:` header tags is NOT how you do push](https://twitter.com/dassurma/status/748616497115836416)

## Installation (OS X)

* Download the corresponding binary from [their release page](https://github.com/GoogleChrome/simplehttp2server/releases)
* Open Terminal and navigate to the download folder
* Copy the binary from the download folder to the `/usr/local/bin` folder: `cp simplehttp2server_darwin_amd64 /usr/local/bin/simplehttp2server`
* Execute the command `chmod +x /usr/local/bin/simplehttp2server`
* Restart Terminal or open a new tab
* Clone this repository in the desired folder (e.g. `$HOME/Sites/http2`) `git clone https://github.com/dirkpennings/http2`
* Start your local server with `simplehttp2server` and navigate to [https://localhost:5000](https://localhost:5000)

### Useful links

* [HTTP/2 101 (Chrome Dev Summit 2015)](https://www.youtube.com/watch?v=r5oT_2ndjms&t=21m59s)

### Credits

Thanks go out to [Surma](https://github.com/surma) for explaining some details about simplehttp2server