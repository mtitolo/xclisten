# XCListen

A zero-configuration filesystem watcher for ObjectiveC. It determines your workspace and scheme automatically, and:

- runs tests each time you save a file
- runs `pod install` each time you save the Podfile
- formats your tests with RSpec-style output using [XCPretty](https://github.com/mneorr/xcpretty)


## Installation

```
$ gem install xclisten
```

## Usage

Run this command from the same directory as your `.xcworkspace`:
```
$ xclisten
```
Simple, huh?

![](http://i.imgur.com/JpsMMBW.gif)

If you have an OSX project, you'll want to run it with `--osx` flag.


## Something went wrong!

No worries, just `tail -f xcodebuild_error.log` and let us know what's happening.

## TODO

- Device flag (choose between iphone5s, iPad, iPad Air,...)
- Support non-cocoapods projects, when there's no .xcworkspace
- Acceptance tests
