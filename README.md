# rn-cljs-tools
Tooling for building React Native apps with Clojurescript

## Background

One may currently choose from two build tools when developing React Native with Clojurescript: 
- [re-natal](https://github.com/drapanjanas/re-natal)
- [boot-react-native](https://github.com/mjmeintjes/boot-react-native)

As of June 2016, both are actively developed. In these repo the aim is to collect tools that may be useful for both build systems. I use `re-natal` at the moment so please submit PR's for `boot-react-native`.

## Install

1. Clone this repo
2. Add the dir of the cloned repo to your PATH, [how-to](http://unix.stackexchange.com/a/26059)

_Note: I am not sure in what format this library should ideally be delivered, an npm module that can be installed globally might be the most convenient way assuming that everyone working with RN has npm and node installed. But for now I just wrote a bash script. Create an issue if you have any suggestions :)_

## Features

### Build iOS app for offline usage 
`build-ios-offline`

Requires [ios-deploy](https://github.com/phonegap/ios-deploy)

Start with building the project once from XCode to your device (to add team etc.) and use this from then on.

```
    Usage: build-ios-offline [-t re-natal] [-a <string>]
    
    -t Type of tool: re-natal
    -a The name of your app (<APPNAME>.xcodeproj)
    -s XCode build scheme, default scheme is app name (optional)
```



## Planned features

- Deploy app with [code-push](http://microsoft.github.io/code-push/)
- Build Android app for offline usage