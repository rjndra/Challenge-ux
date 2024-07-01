#  App Analytics Usage Guide

The Zipped project contains workspace with demo app and package. 
1. AppAnalyticsUsage(Demo App)
2. AppAnalytics(Package)
3. AppAnalyticsUsage.xcworkspace
4. README.md

#### This app is build and tested in **Xcode 15.4** and **iOS 17.5** with **swift-tools-version: 5.10**

### This package provides three APIs(features)
1. start sessoin
2. end session
3. log event

### To use this package
1. `import AppAnalytics`
2. add `AppAnalytics.shared.startSession()` where ever you want to use this service basically in appdelegate/session during launch of app
3. user end service `AppAnalytics.shared.endSession()` during dismissal of app
4. log event where you want to log with public Event and Properties classes to provide your desired events using `AppAnalytics.shared.log(event: Event, properties: Properties)`

#### Note:
This app has used the dummy *baseurl* and *endpoint* with mock decoder for response.

This app has enabled user session and event logged locally with session start and event log and delete of log with end session locally.
For local storage have used UserDefaults as of now.
Every event are pushed to server using urlsession network


