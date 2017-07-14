# Examples

<a href="https://travis-ci.org/iris-contrib/examples"><img src="https://img.shields.io/travis/iris-contrib/examples.svg?style=flat-square" alt="Build Status"></a>
<a href="https://github.com/iris-contrib/examples/blob/master/LICENSE"><img src="https://img.shields.io/badge/%20license-MIT%20%20License%20-E91E63.svg?style=flat-square" alt="License"></a>
<a href="https://github.com/kataras/iris/blob/master/HISTORY.md"><img src="https://img.shields.io/badge/version-8.x%20-blue.svg?style=flat-square" alt="CHANGELOG/HISTORY"></a>

This repository provides easy to understand code snippets on how to get started with web development with the Go programming language using the [Iris](https://github.com/kataras/iris) web framework.

It doesn't contains "best ways" neither explains all its features. It's just a simple, practical cookbook for young Gophers!

## Table of contents

* [Overview](overview)
    * [Hello world!](hello-world/main.go)
    * [Glimpse](overview/main.go)
    * [Tutorial: Online Visitors](tutorial/online-visitors/main.go)
    * [Tutorial: URL Shortener using BoltDB](tutorial/url-shortener/main.go)
* [HTTP Listening](http-listening)
    * [Common, with address](http-listening/listen-addr/main.go)
    * [UNIX socket file](http-listening/listen-unix/main.go)
    * [TLS](http-listening/listen-tls/main.go)
    * [Letsencrypt (Automatic Certifications)](http-listening/listen-letsencrypt/main.go)
    * [Custom net.Listener](http-listening/custom-listener/main.go)
    * [SO_REUSEPORT for unix systems](http-listening/custom-listener/unix-reuseport/main.go)
    * [Omit server errors](http-listening/listen-addr/omit-server-errors)
    * [Custom HTTP Server](http-listening/custom-httpserver/iris-way/main.go)
    * [Custom HTTP Server (STD)](http-listening/custom-httpserver/std-way/main.go)
    * [Multi HTTP Servers](http-listening/custom-httpserver/multi/main.go)
    * [Graceful Shutdown](http-listening/graceful-shutdown/default-notifier/main.go)
* [Configuration](configuration)
    * [Functional](configuration/functional/main.go)
    * [From Configuration Struct](configuration/from-configuration-struct/main.go)
    * [Import from YAML file](configuration/from-yaml-file/main.go)
    * [Import from TOML file](configuration/from-toml-file/main.go)
* [Routing](routing)
    * [Overview](routing/overview/main.go)
    * [Basic](routing/basic/main.go)
    * [Custom HTTP Errors](routing/http-errors/main.go)
    * [Dynamic Path](routing/dynamic-path/main.go)
    * [Reverse routing](routing/reverse/main.go)
    * [Custom wrapper](routing/custom-wrapper/main.go)
    * [Route State](routing/route-state/main.go) 
* [Custom Context](routing/custom-context)
    * [Method Overriding](routing/custom-context/method-overriding/main.go)
    * [New Implementation](routing/custom-context/new-implementation/main.go)  
* [Convert http.Handler](convert-handlers)
    * [From func(http.ResponseWriter, *http.Request, http.HandlerFunc)](convert-handlers/negroni-like/main.go)
    * [From http.Handler or http.HandlerFunc](convert-handlers/nethttp/main.go)
* [Subdomains](subdomains)
    * [Single](subdomains/single/main.go)
    * [Multi](subdomains/multi/main.go)
    * [Wildcard](subdomains/wildcard/main.go)
    * [WWW](subdomains/www/main.go)      
* [View](view)
    * [Overview](view/overview/main.go)
    * [Hi](view/template_html_0/main.go)
    * [A simple Layout](view/template_html_1/main.go)
    * [Layouts: `yield` and `render` tmpl funcs](view/template_html_2/main.go)
    * [The `urlpath` tmpl func](view/template_html_3/main.go)
    * [The `url` tmpl func](view/template_html_4/main.go)
    * [Inject Data Between Handlers](view/context-view-data/main.go)
    * [Embedding Templates Into App Executable File](view/embedding-templates-into-app/main.go)
* [Authentication](authentication)
    * [Basic Authentication](authentication/basicauth/main.go)
    * [OAUth2](authentication/oauth2/main.go)
    * [JWT](https://github.com/iris-contrib/middleware/blob/master/jwt/_example/main.go)
* [File Server](file-server)
    * [Favicon](file-server/favicon/main.go)
    * [Basic](file-server/basic/main.go)
    * [Embedding Files Into App Executable File](file-server/embedding-files-into-app/main.go)
    * [Send/Force-Download Files](file-server/send-files/main.go)
* [Single Page Applications](file-server/single-page/application)
    * [Single Page Application](file-server/single-page-application/basic/main.go)
    * [Embedded Single Page Application](file-server/single-page-application/embedded-single-page-application/main.go) 
* [How to Read from *http.Request`](http_reqest)
    * [Bind JSON](http_request/read-json/main.go)
    * [Bind Form](http_request/read-form/main.go)
    * [Upload/Read Files](http_request/upload-files/main.go)
* [How to Write to http.ResponseWriter](http_responsewriter)
    * [Text, Markdown, HTML, JSON, JSONP, XML, Binary](http_responsewriter/write-rest/main.go)
    * [Stream Writer](http_responsewriter/stream-writer/main.go)
    * [Transactions](http_responsewriter/transactions/main.go)
* [Miscellaneous](miscellaneous)
    * [Request Logger](http_request/request-logger/main.go)
    * [Localization and Internationalization](miscellaneous/i18n/main.go)
    * [Recovery](miscellaneous/recover/main.go)
    * [Profiling (pprof)](miscellaneous/pprof/main.go)
    * [Internal Application File Logger](miscellaneous/file-logger/main.go)
    * [Testing](testing/httptest/main_test.go)
    * [Caching](cache/simple/main.go)
* [Sessions](sessions)
    * [Overview](sessions/overview/main.go)
    * [Standalone](sessions/standalone/main.go)
    * [Secure Cookie](sessions/securecookie/main.go)
    * [Flash Messages](sessions/flash-messages/main.go)
    * [Database](sessions/database/main.go)
* [Websockets](websockets)
    * [Chat](websockets/chat/main.go)
    * [Native Messages](websockets/native-messages/main.go)
    * [Connection List](websockets/connectionlist/main.go)
    * [TLS Enabled](websockets/secure/main.go)
    * [Custom Raw Go Client](websockets/custom-go-client/main.go)
* [Experimental Handlers](experimental-handlers)
    * [Casbin wrapper](experimental-handlers/casbin/wrapper/main.go)
    * [Casbin middleware](experimental-handlers/casbin/middleware/main.go)
    * [Cloudwatch](experimental-handlers/cloudwatch/simple/main.go)
    * [CORS](experimental-handlers/cors/simple/main.go)
    * [JWT](experimental-handlers/jwt/simple/main.go)
    * [Newrelic](experimental-handlers/newrelic/simple/main.go)
    * [Prometheus](experimental-handlers/prometheus/simple/main.go)
    * [Secure](experimental-handlers/secure/simple/main.go)
    * [Tollboothic](experimental-handlers/tollboothic/limit-handler/main.go)


> Do not forget to [star or watch the project](https://github.com/kataras/iris/stargazers) in order to stay updated with the latest tech trends, it takes some seconds for the sake of go!


> Examples are tested using Windows 7, Ubuntu 16.04 with [LiteIDE](https://github.com/visualfc/liteide).

## Run

```sh
$ cd $GOPATH/src/github.com/iris-contrib/examples/overview
$ go run main.go
```

## Any troubles with examples?

    https://github.com/iris-contrib/examples/issues

## Su, 04 June 2017

This repository is just a minor of the github.com/kataras/iris/[version or master]/_examples folder.
